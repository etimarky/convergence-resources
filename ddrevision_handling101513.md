



DDRevision\_Handling101513 - Design For Retrieval (DFR) Help




**Revision 
Handling**



The 
DFR system has the capability to store multiple revisions of an item.  
Different revisions of an item are stored by the data in the Revision system 
attribute.  To determine the latest Revision the DFR system leverages the 
Release Date system attribute.  The Release Date system attribute is 
intended to store the date the revision of an item was finalized and released, 
hence the date it became the next revision.  The Release Date system 
attribute is also used to determine revision order.  


 


A 
setting in TblOptions has been added to make this functionality 
configurable.  This configuration will show all revisions or just the 
latest revision in Data Developer.  (See the Admin to 
configure.)   Note:  If the user has the Revision Manager role, 
it will override the system setting.  


 


If 
the setting is set for show only the latest revision, the user will just see 
the latest revision.  If the user has the Revision Manager role, the Show All Revisions link will display.  
Clicking this link will display all items, all revisions.


 


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DD-Revision_Handling101513_files/image001.jpg)




 


 


 


Clicking 
the Show All Revisions link below, 
the user can view all items.  To get back to the view of just latest revision, 
just click the Show Only Latest Revisions link.


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DD-Revision_Handling101513_files/image002.jpg)




 


 


 


 


Return 
to [Data Developer](/html/hs4000.md)


 




