



External\_Data\_Model\_Management - Design For Retrieval (DFR) Help



# External Data Model Management


The **External Data Model Management** feature allows you to easily manage mappings between your CDS PIM data model and any external data model.


This is useful when importing data from another source system that may not have fields exactly matching your attributes in CDS PIM.


 


To access External Data Model Management, navigate through the **Catalog Administration** menu.


 


**The main page of the External Data Model Management module is split into two sections.** 


A. On the left you can see all existing external data models.


B. A checkmark in the Import Mapping column indicates that the data model has successfully been mapped to your CDS PIM data model.


C. You can view any existing mappings and add new mappings by clicking the Manage Mappings icon for the respective data model.


D. Clicking on any data model will display details on the right side of the page.


![](assets/image(118).png)




 


 


## **Creating a New External Data Model**


1. Click the + icon at the top center of the screen.  

![](assets/image(119).png)




2. Name your data model.


3. Your new data model has been added and is available to edit now.


 


 


 


## **Managing Mappings**


1. Select the desired data model that you want to edit.


2. Click on the Manage Mappings icon.


![](assets/image(120).png)




 


3. On the left side of the screen are **Source Fields**: these are the fields from your external data model. If this is a new external data model, this section will appear blank at first, and you will need to add them using the + icon.


 


![](assets/image(122).png)




 


4. Add the Source Field names. Name the attribute as it would appear in your source.  

For example, if you are planning to import data via spreadsheet, use the column headers as the attribute names.


Name is the only required field; the others can be populated at your discretion.


 


![](assets/image(123).png)




 


5. Once you've added your Source Field attributes, they will appear on the left side of the page and will be available for mapping.


6. On the right side of the page you will see **Target Fields**, which are your CDS PIM attributes.


  

![](assets/image(125).png)




 


7. To make a mapping, simply select a source attribute and a target attribute.


8. The middle section of the page will display the **Mapping Details**.


9. To confirm the mapping, click the orange **Map** icon (![](assets/image(130).png)

).


 


![](assets/image(124).png)




 


10. Continue this activity until you have mapped all desired fields. Source fields that have already been mapped will display a yellow checkmark.  

![](assets/image(126).png)




 


11. **Important: Select a default value for the Operation target field.**


After selecting the Operation field, click **Map with Default Value**under the Mapping Details section. This functions like the Operation in the Thick Client Import Manager. You need to tell the data model what operation should be taken when importing these items.


 


![](assets/image(134).png)




 


When you click Map with Default Value, the default is set to **Update**, meaning any feed will update existing items with the details included in your import file.


![](assets/image(135).png)




This step **must**be completed in order to execute an import using this data model.


 


12. To view a summary of the mappings for this data model, click on the scroll icon (![](assets/image(131).png)

) at the top right of the page.


 


![](assets/image(132).png)




 


 


13. Review mapping summary to confirm your mappings are correct.


![](assets/image(133).png)




 


**Related Pages:**


- **[SmartFeeds Overview](smartfeeds)**
- **[Feed Manager](default-template-4)**- How to view and manage import feeds
	- **[Deliverable Import Feeds](deliverable-import-feeds)**- How to set up a deliverable import feed
	- **[Import Feeds](default-template-1730124762)** - How to set up an import feed
- **[EndPoint Management](endpoint-management)** - How to view, manage, and edit configured endpoints



