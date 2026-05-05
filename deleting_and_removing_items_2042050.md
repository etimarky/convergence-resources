



Deleting\_And\_Removing\_Items - Design For Retrieval (DFR) Help




**Deleting 
and Removing Items**


 


Users 
can delete items that are assigned to them in Data Developer as long as the DFR 
catalog is in sandbox mode.  Sandbox mode gives the user the option to choose 
whether or not to allow items to be deleted from no matter what the status or 
to set the status to obsolete making the item appear deleted to the interface.


 


**Note**:  If the catalog is 
configured in Sandbox mode (Sandbox = true), items can be deleted no matter 
what the status.  It would not be recommended to have this set to true in a 
production environment.  If the catalog is not in Sandbox mode (Sandbox = 
false), items can be deleted where the status is New only.  If the status is 
Pending, Approved, or any User Defined status, the item will be ‘soft deleted’ 
meaning the status will be set to obsolete and the item number cannot be 
reused.  If the item status is set to Obsolete, it will not show up in the 
search results.


## 


***![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/DD-Deleting-And-Removing-Items_files/image001.jpg)***


**Example of deleting items in Data Developer**


 


Return 
to [Data 
Developer](mk:@MSITStore:C:\PROGRA~2\CONVER~1\CDSTOO~1\Core\DESIGN~1.CHM::/html/hs4000.md)


 




