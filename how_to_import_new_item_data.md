



How\_to\_Import\_New\_Item\_Data - Design For Retrieval (DFR) Help



# How to Import New Item Data


The Import Manager is used to import new data, update existing data, and import or update images or data structure. There are two types of data that can be imported: Item Data and Classification data. Item Data refers to parts information such as an item number or attribute information while Classification Data refers to a data structure such as categories where the parts exist. 


 


 




<iframe src="https://www.youtube.com/embed/m7C8AgUjncs/?wmode=transparent" width="560" height="315" frameborder="0" allowfullscreen></iframe>


 


Importing new data using the "Create" operation is a process that is used when the user has information specific to an item number that has never existed in Convergence PIM. 


 


Select Import Manager from the CDS Toolset and then select Item Data.


 


![](assets/image(334)_1.png)




 


Select the file to be imported.


 


![](assets/image(337)_1.png)




 


Select the Excel format from the drop-down menu. 


 


![](assets/image(338)_1.png)




 


Select Item Options from the drop-down, and type or paste the category where you want to place the new parts like the following "Root\Parts\Electronic Devices and Controls\Actuators".


Also, name your Import under new batch. If not renamed, the batch will automatically be imported in as "DEFAULT\_BATCH". 


 


![](assets/image(486)_1.png)




 


Select "Create" for new part imports or Update for imports updating current part information.


The column on the left represents the list of available attributes to choose from. The column on the right will automatically map to the left columns if there is a header with the same name.


Otherwise, this can be done manually by selecting from the drop-down, which contains all original document headers.


 


![](assets/image(341)_1.png)




 


Select Next, and then select validate


 


Once Validation has cleared with no errors, select Next.


 


![](assets/image(342)_1.png)




Some common errors are listed below: 


- **Item Not Found** *( e.g.  "Item not found in database")* - this is self-explanatory and will only generate when the Update operation is chosen on the mapping screen.  To correct this error, import using the "Create" operation which will create the part that did not already exist. This error may also exist if the Item Number contains a revision number and "Revision" isn't selected and mapped on the mapping screen. Without the revision number, Convergence PIM cannot locate that part and will display an "Item Not Found" code.
- **Invalid Category** *(e.g***. "***Category 0 and Path Root\Parts\Heating Elements\Coils do not resolve to a valid category")* - This can appear through any of the functions. This error message is stating that the category mapped does not exist. To correct this error, check your load document and make sure that the category path does exist in Convergence PIM and if it does not, that category will need to be created before you may import data using that pathway.


 


Select Import. The import is complete.


 


 

