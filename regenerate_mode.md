



Regenerate\_Mode - Design For Retrieval (DFR) Help



**Regenerate Mode**


 


**Regenerate Mode** allows a user to add items to an existing batch. This, in effect, adds new item master data to a batch that has already been loaded into the classification.


 


Regenerate operations require the following:


 


- New items added to the batch are added as news rows at the bottom of the original New Batch load file.

 


- All of the items from the original New Batch load operation must be present in the Regenerate load file.

 


- Root attributes from the original file may be modified, however, technical attributes cannot be modified.

 


**To add new items to an existing batch:**


 


- Select the **Regenerate** button from the Import Type box at the top of the Item Loader screen.

 


- Press the **Start...** button.

 


- Type in the file name for the import file in the Import File field, or select the **Browse…** button.

 


- Press the **down** arrow next to the Batch field, and select the name of the batch from the drop-down list that matches the previous load file that is being regenerated.

 


**Note:** If the item number, qualifier and revision of the load file do not match the items in the existing batch, the loader will generate an error message


 


- Press the **down** arrow next to the **Qualifier Type** field and select the Qualifier Type for the batch to be regenerated.

 


- Select an Import File Column Attribute from the left column and select the corresponding Product Attribute from the center column. Then press the **double arrow** button between the two columns.

 


Notice that the mapping relationship has been added to the list in the right column.


 


- To automatically select headings with identical names as the corresponding product attribute, press the **Auto Map** button. The Item Loader will find matching attributes to map to the columns in the load file.

 


A [Mapping Template](javascript:popuplink('hs3300.htm')) can be created to save commonly used attribute mapping schemes.


 


- Press the **Preview** **&** **Import** button in the lower right hand corner. The Item Loader will now update the batch.

 


 


Return to [Item Loader Operation](hs3060.md). 





