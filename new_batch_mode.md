



New\_Batch\_Mode - Design For Retrieval (DFR) Help



**New Batch Mode**


 


**New Batch** mode is used to load a list of unique item identifiers that will define a new batch of items.  This initial load of information will be referred to as the **Item Master Load** and will contain basic information for each item. 


 


**To load a new batch**:


 


- Select **Item Loader Module** icon from the Applications Toolbox.

 


- Select **New Batch** radio button in the Import Type box.

 


- Press the **Start…** button to begin the load operation.

 


- Type in the file name for the item master load file name in the **Import File:** field or select the **Browse…** button and select the load file from the drop down list.

 


- Enter a name for the batch in the **Batch**: field. The batch name will identify this group of items in all future operations.

 


- Select the **Qualifier Type** from the drop down list. The default qualifier type is PART.

 


- Press **Ok** when the batch import file information is complete.

 


The Import operation button will change from **Start...** to **New...**, indicating that a new batch is to be loaded. The windo will be divided into three columns. The Left column will list the attribute labels imported from the import file columns. 


 


- Select an Import File Column attribute from the left column and select the corresponding Product Attribute from the center column. Then press the **double arrow** button between the two columns.

 


Notice that the mapping relationship has been added to the list in the right column.


 


- To automatically select headings with identical names as the corresponding product attribute, press the **Auto Map** button. The Item Loader will find matching attributes to map to the columns in the load file.

 


A [Mapping Template](javascript:popuplink('hs3300.htm')) can be created to save commonly used attribute mapping schemes.


 


- Select the **Preview & Import** button in the lower right corner.

 


If a duplicate part number exists in the batch, Item Loader will display an error message at the bottom of the screen stating how many duplicate records were found. To correct the duplicate records, edit the batch import text file, removing the duplicate records or further differentiating the items using the Revision, Qualifier or Qualifier Type attributes.


 


When the Item Loader has determined that no duplicate item numbers or other errors have occurred, the "PREVIEW - UNIQUE PART LIST IMPORT MAPPING" window will appear.


 


- Review the data and select the "**Import**" button. The import will proceed.

 


A box will appear and display the overall progress including:


 


§ Creating category


§ Loading item master


§ Scanning for naming conflicts


§ Loading data


§ Items loaded


 


- When the process is complete, a category will have been created in the "To Be Classified" category with the name of the batch.

 


The items must now be assigned to a responsible user and be sorted into the destination categories using the Item Browser Module.


 


 


Return to [Item Loader Operation](hs3060.md).


 


 


 


 







