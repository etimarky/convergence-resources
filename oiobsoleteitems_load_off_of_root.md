



OIObsoleteItems\_load\_off\_of\_root - Design For Retrieval (DFR) Help




**Obsolete 
Items**


 


 


*Obsolete 
Items* 
is a status for an item that has been ‘soft deleted’.  When DFR is in Sandbox 
mode, an item of any status will be deleted and therefore removed from the 
catalog.  (Sandbox mode is defined as a development/testing environment mode 
where hard deletes are allowed.)  


 


When 
Sandbox mode is off, only new items (items with status of New) can be hard 
deleted.  All other items with the status of Pending, Approved, or any User 
Defined status will be soft deleted.  These items will simply change the status 
to ‘Obsolete’ and will not show up in any searches in DFR, WebDFR or 
SmartFind.  This preserves the Item Number from being reused should it be 
related to any parent or child items.  


 


The 
user can specify a certain part to obsolete.  They can do this by Tools > 
Obsolete Part.  The Select Part to Obsolete dialog box displays.  Type in the 
Item Number, Revision (if applicable), and Qualifier Name and select the Root 
Qualifier.  Once those fields are filled in, click OK and the system will 
obsolete that Part.  


 


 


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/OI-ObsoleteItems_(load_off_of_root)_files/image001.jpg)




 


The 
User must be a Catalog Administrator to have the Find Obsolete Parts command 
available.  Go to the Main toolbar Tools > Find Obsolete Parts and it will 
automatically generate the list of obsolete parts.


 


 


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/OI-ObsoleteItems_(load_off_of_root)_files/image002.jpg)

  
  
 


 




