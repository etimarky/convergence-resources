



Convergence\_PIM\_to\_Teamcenter\_Checklist - Design For Retrieval (DFR) Help



# Convergence PIM to Teamcenter Checklist


**\*Note: the line items that require IT assistance are denoted by an "(IT)" at the end of the line. This checklist should be used for every category and every export.**


 


1. Run Teamcenter Environment Conversion Script on each necessary catalog (TeamCenterIntegrationProps.sql) **(IT)**
2. Ask customer which attribute and LOV IDs they want to start with


	- This needs to be done because the target Teamcenter environment will have some default attributes/LOVs and some manually created ones. The setting in Convergence PIM should account for the used ID range so that no clashes occur (e.g. Convergence PIM exports an attribute with an ID of 200 when the Teamcenter environment already has a non-Convergence PIM attribute with that ID, thus overwriting it or failing to import)
	- See "Settings for IDs" section in the First Time Setup article. Convergence PIM will assign Attribute IDs in a positive increment from the starting ID (e.g. 10000, 10001, etc.), while LOV IDs will be assigned in a negative increment from the starting ID (e.g. -10000, -10001, etc.)
3. Set starting LOV and Attribute IDs in the Export Manager > Classification Data > PLMXML > Settings
4. Obtain a Teamcenter Unit Definition Class export from the customer’s Teamcenter environment


	- One easy way this can be accomplished by selecting the Unit Definition Class and exporting it with the type "ICSExportSubtreeWithICOs"  
	
	![](assets/image(23).png)
5. Create mappings in the Export Manager PLMXML settings to link Convergence PIM UoMs to the Teamcenter UoM ICO IDs (also called Object IDs - see article "First Time Setup" for an example of this)


	- If any unique UoMs exist in the Teamcenter environment that will be used for data in Convergence PIM, they will need to be created in Convergence PIM first and then mapped afterwards
6. Set the uomSystems value to 1 or 2 on the UoMs in the Unit of Measure Editor (1 = Metric, 2 = Imperial)


	- If any UoMs need to toggle (e.g. mm to in), the default UoMs for that Unit of Measure Type needs to be set in the database **(IT)**
7. Ensure that there are no null values on required attributes or items will not load
8. Limit String values to 99 characters
9. Ensure that no LOV values are longer than 63 characters.  Items will not load if a value is not on the LOV list
10. If abstract classes are being used, LOV list integrity needs to be checked. This includes things like making sure a shared LOV list accounts for all potential values across multiple categories. See article "Best Practices - Setting up Abstract Classes" for more information
11. Scale and precision need to be set to a number that allows space for both metric and imperial numeric values


	1. Scale = the number of total digits in the number. For example, the scale of 10.25 is 4
	
	
		- Teamcenter requires adding two digits to the scale to account for the decimal itself and the sign +/-. In the case of the number above (10.25), the final scale we'd settle on is 6. Total number of digits (4) + 1 for the decimal + 1 for the sign (even if it's positive) = 6
	2. Precision (also called 'Default Decimal Places' in Convergence PIM) = the number of total digits after the decimal point. For example, the precision of 10.25 is 2
	3. The values set for scale and precision need to account for the largest values in the category/categories they cover. For example, if the Length attribute values for a category are 1.7855, 110.225, and 0.33, you'd need to look at all values to find the proper value for scale and precision. For scale, the value with the most total digits is 110.225 (6), so the scale would need to be set to 8 (6 digits + 1 decimal + 1 sign). In the case of precision, the value with the most digits after the decimal is 1.7855, so the precision would be set to 4.
	
	
		1. The example above presents an edge case that needs to be recalculated due to how Teamcenter's scale works. See the next bullet for an explanation and afterwards this edge case will be explained.
		2. Teamcenter takes scale and precision a step further and instead of looking at them as scale/precision, it views it as # of digits allowed before the decimal and # of digits allowed after the decimal. Because they account for the decimal point and the sign, we "lose" 2 from our scale, and Teamcenter takes it off from the digits before the decimal. This means that Teamcenter's final reading, formatted as "#.#", is scale - precision -1 for the decimal, -1 for the sign, and then # of digits after the decimal. In the case of the example value 10.25, the scale is 6 (4 digits + 1 decimal + 1 sign) and the precision is 2 (2 digits are after the decimal). Teamcenter will backwards engineer this and put it in the format just mentioned, #.#. We know that if the second digit needs to be the precision, then we will insert that and we now have #.2. To get the first number, as mentioned before we will take the scale (6) - the precision (2) - 1 for the decimal - 1 for the sign. This calculation ends up being 6-2-1-1, which leaves us with 2. That final answer goes before the decimal, which gives us 2.2, the maximum number of digits before and after the decimal that a value can have. This leaves us room to insert our example value of 10.25.
		3. Now, as for the edge case, in the example listed above in 11.3, the largest scale of the values was 8, and the largest precision of the values was 4 - these settings came from two different attribute values, 1.7855 and 110.225. While in Convergence PIM that scale and precision would cover it, we need to reverse calculate it to figure reveal why this doesn't work. Using the same method as above, we convert scale/precision to the way Teamcenter really looks at it. Our precision was set to 4, so we can input that into the right side and now we have #.4. To calculate the # of digits allowed before the decimal, we take our scale (8) - precision (4) - 1 for the decimal - 1 for the sign. This results in 8-4-1-1 = 2. However, this presents a problem. What Teamcenter sees is 2.4, in other words, Teamcenter will allow up to 2 digits before the decimal and up to 4 digits after the decimal for that category attribute. The issue is that one of our values is 110.225, which has 3 digits before the decimal. The precision requirement is met, but the import will error out because the number of allowed digits before the decimal has been exceeded. In that case, the scale in Convergence PIM would need to change to account for this. In conclusion, the original values of 8 for scale and 4 for precision would need to be changed to 9 for the scale and 4 for precision.
	4. At the time of writing this, scale can only be set at the master attribute level.  Precision, however, can and should be set at a category attribute level (low in the tree) because setting it on the master attribute level or high in the tree will cause padding zeros in Teamcenter. For example, consider a structure with twp different categories, Bolts and Screws, each a child of a category Fasteners. If the values in Screws only require a maximum precision of 2 (e.g. the attribute value with the most decimal places is 10.25), then you can set precision to 2 on Screws and have no padding zeros. However, if Bolts has a value such as 10.2575, then the precision for Bolts needs to be set to 4, and that would leave no unnecessary padding zeros for the parts in Bolts. This sets up an example case for why you don't want to set Precision too high in the tree. If in this same case, Precision was set at the parent level (Fasteners), then the value would have to account for all attribute values/categories under it. Screws needs a precision of 2, but Bolts needs a precision of 4. Therefore, the precision/default decimal places for the numeric attribute would have to be set to 4 if it was done at the Fasteners level. For Bolts, this looks no different. For Screws, it has now inherited a precision/default decimal place of 4, so values will now be padded, and a number like 10.25 will now display 10.2500 in Teamcenter.
12. If data in a category is mixed, it will normalize to whichever "Default ICO UoM System" button is selected on the first screen of the Item Data export. This can also be used to force an all-Imperial category to Metric, for example, by changing one of the inch values to millimeters.
13. Populate the Legacy Part Number Field with the Part IDs the parts should tie to once in Teamcenter. Sometimes the ID will be the same as the Convergence PIM Part Number, but confirm that with the customer. If not, they will need to provide a mapping file of current Convergence PIM Part Numbers to Target Teamcenter Part IDs, and the Legacy Part Number field in Convergence PIM can then be populated with the proper TC Part IDs (and the revision if they use them) for each Convergence PIM Part Number (format for the LPN field is "<Teamcenter Part ID>/<Revision>", but if there are no revisions, it would just be "<Teamcenter Part ID>")
14. Add NA (or customer-decided placeholder) to LOV Lists
15. If doing multivals, the attribute type needs to change to Custom, the CustomData property needs to be set to MultiVal, and the TC ArraySize needs to be set to however many fields they want to see in the part search screen
16. If certain attributes need to be left out of the export, set different statuses on them so you can filtering them out in each export
17. Run final validations in Data Developer
18. Run the Teamcenter PLMXML Export - Classification export has to be done first, then Item Data


	- Do not select the option to "regenerate Teamcenter IDs" unless you confirm with IT/Chris that the situation calls for it
19. Do a test import into Teamcenter - Load LOVs, Attributes, Classes, and then Items (see article Loading Convergence PIM Export into Teamcenter)
20. After importing successfully, send a zip package of the 5 files (LOVs, Attributes, Classes, Items, ICO Mappings) to customer (exclude the log files)



