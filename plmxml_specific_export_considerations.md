



PLMXML\_Specific\_Export\_Considerations - Design For Retrieval (DFR) Help



# PLMXML Specific Export Considerations


 


Once you have completed your [(First Time Setup)](#) you still may need to take a few things into account when doing a PLMXML Export, that are different from the standard Export Process.


 


The following Items will need to be considered in order to have a successful PLMXML Load into Teamcenter:


 


**Regenerate IDs**


If you are exporting to an existing Teamcenter instance, you will most likely NOT want to regenerate IDs when doing an export. 


This will cause the Convergence PIM tool to systematically go through the Classification and re-assign all IDs, to Attributes, LOVs, and Classes.


It will create Abstract classes with the  "Is Abstract" Flag set to TRUE on Classes.


It will separate out attributes into multiples if there are instances of the same attribute name with a different value at the Class-Attribute level. IE different length, UoM Type, or LOV list.


 


**Define Top level of Structure and Select Classes in the correct order**


When selecting what to export, make sure you choose the highest level of item you want to export, then UNCHCEK any items you don't want to export.


If you only select the lower level items, Convergence PIM will not export any of the inherited data from the classification structure above. This can create collisions regarding the Attribute IDs and Class IDs, especially if you are using abstract classes.


Once you export is complete, you will also need to modify the Class.plmxml. You will need to make sure that the top level of your classification structure is like to "ICM' as it's parent in order to operate correctly in Teamcenter Classification.


 


**Convergence PIM Validations**


In order to have a successful export/import, you will need to first make sure that the data is correctly formatted. Running Data Validations in Convergence PIM will allow you to find and fix any of the issues in the data. It is important to make sure that in particular, there are no Nulls in any fields marked as Mandatory. 


 


**Check for Duplicate Attributes**


Because of the common issue of having duplicate Attributes due to collisions, it is advised that you check the data for duplicates before loading into Teamcenter in order to keep your Teamcenter environment clean.


The easiest way to do this is to open the PLMXML file in Excel. 


 


Once you have that set up, sort the file by Attribute Name, and highlight that entire column. 


Go to conditional formatting and apply the duplicate rule.


 


![](assets/image(1003).png)




 


This will highlight any duplicate attributes you may have in the system, allowing you to fix and re-export the data. 


The likely causes are: LOV conflicts, Data Type mismatch, Required Attribute mismatch, or manually assigned ID.


Once you resolve these issues, re-run your export and test again for duplicates.


 


**Check for Blank Values(Item Files)**


Another possible problem you may encounter while working with the XML Files, is missing values in the Item PLMXML File. This can cause errors in uploading, as Required Fields are not allowed to be blank upon import. If the fields that are missing are not mandatory, you will not see any errors from Teamcenter and will need to manually make sure the data has made it. 


The main reason for this occurring is for exporting an item file with conflicting Attribute information. If you have made changes to the existing data structure and there are multiple attributes with the same ID that are not supposed to, Convergence PIM will not be able to correctly place the data in the Items PLMXML file. 


The other time you may encounter this issue is when using abstract classes. If the Parent Class that contains the defined attribute has a different ID than the attribute on the storage class, the items will be exported incorrectly.


 


 


**Look out for file mismatches**


When exporting multiple files, you must make sure you keep track of which files are exported when. If you are importing Item files that are newer/older than the rest of the classification files, you will very quickly encounter errors. By default the Convergence PIM Export will name the file with the Date and Time which can help you track this. Consider using this, or adding additional information to your files names in order to prevent any mismatches.


 



