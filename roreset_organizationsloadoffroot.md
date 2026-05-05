



ROReset\_Organizationsloadoffroot - Design For Retrieval (DFR) Help




**Reset 
Organizations**


 


 


*Reset Organization* allows users to change a batch of 
items qualifiers in a single operation.  Here are some guidelines on this 
feature:


- A user cannot make changes to an item while the Item 
 Loader is running.  A message will warn the user of this condition.
- You cannot change the qualifier type of a batch.
- Batches that contain items with different qualifier types 
 do not show up in the batch list to process.
- Batches that contain organizations from the organization category 
 do not show up in the batch list.  Any batch with organization as the 
 qualifier type cannot be processed.  To change these types of items, a 
 user can do this on an individual basis using the rename item function.
- Both working batches and load batches can be processed.
- Only qualifiers that already exist in the database, not 
 necessarily used, are presented in the Qualifier list.  The list is 
 restricted to the qualifier type for the batch selected.
- You cannot rename an item to another item’s exact primary 
 key.  This is recognized as a duplicate and will error out.  Each 
 duplicate item will be listed in the error message box.
- The Try key allows a user to validate their change before 
 actually implementing the change.
- The OK key will implement the change as long as there are 
 no error conditions.  Please note you will have to refresh your data in 
 DFR to see the change in the database.
- There are only 2 possible error conditions, (1) item not 
 assigned to user or (2) creating duplicate item.
- The Cancel key can both cancel an operation or you select 
 cancel to exit out of this Rename Item application.

 


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/RO-Reset_Organizations(loadoffroot)_files/image001.jpg)




**Assign a 
New Organization dialog box**


Select a batch from the Batch drop down list.  Select the 
qualifier from the Qualifier drop down list to update it.  Select Ok.   
  



![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/RO-Reset_Organizations(loadoffroot)_files/image002.jpg)




The dialog box will display any 
Item Numbers that have an error.   
 


 




