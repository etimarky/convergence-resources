



How\_to\_Create\_an\_Export\_File\_for\_Teamcenter - Design For Retrieval (DFR) Help



# How to Create an Export File for Teamcenter


 


 


Locate the Export Manager in the ThickClient


 


It is important to export in order: classification and then item data. 
Classification will export attributes, LOVs and classification, while the item data will export just that. 


 


Select Classification Data in the export manager.


![](assets/image(105).png)




 


Choose your export name and destination.


Choose the PLM XML export type. This is specific to Teamcenter and will be the only export that will work for a Teamcenter load.
 


![](assets/image(106).png)




Once "PLM XML" is selected, an option for "Settings" will appear to the right side of the export type selection. 


This will prompt additional settings such as starting LOV Teamcenter IDs and more importantly, the Unit of Measure Mappings. 


 


Unit of Measure mappings is only important if the Convergence PIM UoM does not match what the destination attribute dictionary says.   

For example, if CDS PIM has amp as "a" but Teamcenter reflects "A" for the same amp attribute, it needs to be mapped so that Convergence PIM can make the changes for the file and the file will import into Teamcenter correctly. 
Additionally, there will be an option to "regenerate Teamcenter IDs." 
When exporting, CDS PIM automatically creates IDs for Teamcenter to tell the program where the categories need to exist.   

If a user regenerates IDs, it completely wipes all of the existing IDs and starts from scratch. 
If a user is changing a category to Abstract from non-abstract or adding to the structure, choose to regenerate IDs. Otherwise do not. 
![](assets/image(107).png)




 


The next screen will give the user an opportunity to select specific attributes and attribute groups or statuses. 


If nothing is selected on this screen, CDS PIM assumes that everything is selected. This is the most common practice. 


Select Next when finished. 


 


![](assets/image(108).png)




The next screen will allow the user to select the area of the classification tree that needs to be exported. At least one category must be selected on this screen, otherwise nothing will export. 


The user can also choose category statuses and category attribute statuses on this screen too. 


 


![](assets/image(109).png)




The next screen will begin the export. 


 


![](assets/image(110).png)




One the export is complete, the user will need to do the same thing with the Item Data export. 


These steps will be the same for Item data, except that the user will also be able to choose an overall part status as well as a batch or deliverable to choose to export from. 


 


Once the exports are complete, the user should have 5 files:   

 


![](assets/image(112).png)




The ICS file is not needed to load into Teamcenter. 


 


When loading the files into Teamcenter, the user must load in the following order:  

LOVs  

Attributes  

Class  

Items
 


 



