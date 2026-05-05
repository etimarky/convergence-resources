



Editing\_the\_Data - Design For Retrieval (DFR) Help




**Assignment 
and Editing Rights**



**Assignments**


All modules are owned by a particular owner group.  All 
product groups contain one or more owners, who are permitted to modify variant 
years within a module in a module type.


**![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/IM-Assign_Edit_files/image001.jpg)**


**Example: the logged in user is the owner for *Food 
Stream Solutions* product group for the above module type, and is therefore 
allowed to save changes made to that module.**



**![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/IM-Assign_Edit_files/image002.jpg)**


**Example: the logged in user is the not the owner for the *Refrigeration* 
product group for the above module type, and therefore is not allowed to save 
changes made to that module.**


 


**Current 
Users**


There is a new link on the item mapping to get a listing of 
users currently logged on, who are permitted to make changes to the currently 
open map. ![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/IM-Assign_Edit_files/image003.png)




 


When a user first starts a mapping session, they have a 
couple of options including: Option 1: Editing a road map saved to the DFR 
database or Option 2: Loading a what-if road map


### Option 1: Editing Maps in the Database


To work on road map that has been saved to the database, you 
will first need to select *Open* in the Map-DB menu (see below).  The 
user will have a choice of what road map to work on.  The name of the last 
road map last worked on will already be selected.


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/IM-Assign_Edit_files/image004.png)




 


**Map-DB menu is used to access roadmaps saved in DFR**


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/IM-Assign_Edit_files/image005.png)




**Selecting a road map saved 
in the DFR database (last roadmap worked in shows selected)**


Description of the Map-DB menu selections:


Open – displays the list of road maps in the DFR 
database.  Typically this will select the last road map a user 
edited.  The names of the road map files come from the names of the Module 
Type categories stored in DFR.


Save – save changes to a production road map to the DFR 
database.  A warning will be provided if a user selects save to confirm 
the changes that are about to be made in the DFR database.


 


### Option 2: Loading “what-if” Maps


Load a “what-if” road map from the file menu (see 
below).  This will allow users to work on road map data without 
over-riding the current road map saved in the DFR database.  Any DFR user 
will be able to create what-if road maps.  When a user is done making 
changes to the “what-if” road map, they have the option to save changes to an 
XML file on their hard drive or save changes to the database.  Only users 
that are assigned to the modules can save changes to the DFR database, which 
will override the current production roadmap.  
  
![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/IM-Assign_Edit_files/image006.png)




**Example of File menu choices**


The menu choices under the File menu (see above) are 
primarily for loading and managing what-if road maps, not production road 
maps.  Changes to production road map functions are under the menu Map-DB. 



Here are the descriptions for the new menu offerings under 
the File menu.


Load – Load a previously created “what-if” file.  This 
is only for loading a previously created XML file.


Save As – Save “what-if” road map changes to a file on a 
user’s hard drive.  This save is not used from production road maps.  
User can change the file name during the save process if they want to save a 
separate what-if file.  


Print – Prints only the current road map on display.  
Print out will include roll-up metrics for the road map at the bottom.


Print Small – Prints a smaller, less detailed version of the 
road map.


 


### Determining who can modify a 
variant in a module



![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/IM-Assign_Edit_files/image007.jpg)




Assuming 
the module shown above:


 


1.      Find the 
OWNER\_GROUP NAME for this module:


 


**select 
OWNER\_GROUP from SJTCAPP.BOM\_OWNER\_GROUP where NAME = 'Fabric Care';**



**Returns**: **laun**


 


2.      Find the product 
group name for this module


 


Map 
the owner group name to the product group. By looking in the WHR\_PROD\_GROUP 
table



**select 
PROD\_GROUP from sjtcapp.WHR\_PROD\_GROUP where PROD\_GROUP = 'laun'** 



**Returns: laun**



**Note: 
In the case that the name does *not* map up, we use the name mapping in 
the Options Manager.**


 


3.      Query the 
ECR\_APPROVERS table for each module to determine owners this product group


 


**select 
EMP\_ID\_KEY from sjtcapp.ECR\_APPROVER** 


**where CATEGORY\_ID = 13551 and ROLE\_CODE 
= 'ga' and PROD\_GROUP='laun'**



**Returns:  193803**


 


‘ga’ 
is the role code for “Owner” as described in the ECR\_APPROVER\_ROLE table


‘13551’ 
is the category id corresponding to the module shown in the screen capture 
above.


‘laun’ 
is the product group name value calculated in step 2.


 


Note: 
depending on the product group, this could return more than one owner.  In the 
case of multiple owners, any one of the owners has permission to modify the 
map.


 


4.      Determine the 
dfr id of the owner from step 3


 


**select 
USERID from SJTCAPP.EMPLOYEE where emp\_id\_key = 193803;**



**Returns: 
‘kbaron’**



Thus, 
the user kbaron is allowed to modify this module.


### 


 


 


 


Return 
to [Item 
Mapping](IM-Item_Mapping.md)


 




