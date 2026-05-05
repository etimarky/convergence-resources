



Import\_Mode - Design For Retrieval (DFR) Help



**Import Mode**


 


The **Import** button is used to update items in a batch with additional attribute values, usually known as **technical attributes**. An import operation is performed on batch that has already been loaded and its items placed in the appropriate classification categories using the Item Browser Module.


 


This operation can only be performed when


 


- The Item Masters have been loaded as a new batch
- The items have been assigned to a responsible user
- The user has classified the items into their destination categories

 


Once the items for an item master batch have been classified into their destination categories, the item import operations must be sorted to reflect the different destination categories. The Item Loader will check to see that all items in an import file are in the same category. The attributes listed in the import file header must also match the attributes in the destination category. If not, an error message will be produced. 


 


Prepare to import attributes by creating a tab-delimited file that includes the items' Item Number, Revision and Qualifier.  Add columns to the file to represent the additional attributes and populate each item with the attribute values.


 


Ensure the column headers in the file match the attributes assigned to the category or add the attributes to the category using the Classification Manager.


 


**To load the attribute values:**


 


- Select the **Import** button from the Import Type box at the top of the screen.

 


- Press the **Start...** button.

 


- Type in the file name for the import file in the **Import File** field, or select the **Browse…** button.

 


- Press the **down** **arrow** next to the Qualifier Type field and select the Qualifier Type for the batch to be regenerated.

 


- Press the **Ok** button.

 


The Item Loader Preview window will display the contents of the import load file. After reviewing the contents, press the **Import** button to map the import file attributes to the available product attributes.


 


The headings for the import columns of the tab-delimited load file appear in the "Import File Columns" window.


 


- Select an Import File Column attribute from the left column and select the corresponding Product Attribute from the center column. Then press the **double arrow** button between the two columns.

 


Notice that the mapping relationship has been added to the list in the right column.


 


All import file columns do not have to be mapped to attributes; a subset of attributes can be mapped. 


 


- To automatically select headings with identical names as the corresponding product attribute, press the **Auto Map** button. The Item Loader will find matching attributes to map to the columns in the load file.

 


A [Mapping Template](javascript:popuplink('hs3300.htm')) can be created to save commonly used attribute mapping schemes.


 


- Select "**Preview & Import.**

 


- A preview screen will appear. Check the data and press **Import** to complete the Item Loader operation.

 


The Item Loader will review the items to insure that all mapped attributes are assigned to the destination category. If not, an error will be displayed. To correct this error, review the attributes assigned to the target category to make sure that all of the mapped attributes are assigned.


 


The Item Loader will review the items in the batch import file and the category to see that they are all classified in the same category.  If not, an error message is produced. To correct this error, edit the batch import file to separate the batch items into separate import files for each destination category


 


When the batch import file has been modified, perform the import operation again.


 


Return to [Item Loader Operation](hs3060.md). 





