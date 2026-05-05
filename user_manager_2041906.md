



User\_Manager - Design For Retrieval (DFR) Help




**Unit of 
Measure Editor**


 


Unit of Measure (UOM) Editor Module 
allows users to maintain UOM data for each DFR database including creating new 
UOM’s; editing existing UOM’s and deleting UOM’s.  Only DFR Catalog Administrators can use this 
module; all other users will not be able to access them.  This module can be accessed from the Tools 
menu.  If you’re not a Catalog 
Administrator then this module will be grayed out.  
  



## Features 
of the UOM Editor:


The UOM Editor allows users to edit 
the UOM data in their DFR database.  This 
dropin module allows users to edit existing UOM data, add new UOM data and 
delete UOM information as long as there are no validation warnings.  When you open the UOM Editor you will be 
presented with a small grid of units of measure for each unit of measure type.


 




**DFR UOM Editor – Main Screen 
Controls**


 




Check Out – 
Allows a user to make local changes to UOM data (Note: you’re not actually 
changing the UOM data in DFR yet)


 




Save – if 
you want to log out of DFR and not check in your changes until another session 
you can save you UOM file locally.  The 
file is saved as an XML format.  You will 
not be able to load a saved file from an old session if some other user has done 
other editing in the UOM editor.  Saves 
come in handy when you come across validation errors that require you to leave 
the UOM Editor to make changes in the DFR database.


 




Load – if 
you log into DFR and UOM editor and you want to resume editing of UOM data from 
a previous session; you can load a previously edited XML file that had not been 
checked in yet.    
  



Try – if 
you just made some changes or a change and you want to validate that the change 
will work; select Try.  Any validation 
error messages will appear if there is an issue.


 




Check in – 
when you check in, you are officially implementing your changes to the DFR 
database.  You will always be prompted 
(reminded) to save any data that has not been loaded after you check in.


 




Un-Checkout 
– allows other users to log into the UOM editor; if you didn’t save any of your 
changes in a previous session; then you will loose them all


 




Done – Exit 
the UOM Editor; it will prompt you to save changes as a reminder; if you don’t 
save your last changes they will be lost.  
  
  



Score – 
this feature will track the changes you make between saves and loads.  The first # represents the number of changes 
to Unit of Measure Types and the second # represents the number of changes to 
UOM’s.  The score will not track 
cumulative changes between check-ins; only changes within a single session; it 
will reset to 0 after a check in.


 




Note:  you will notice in the bottom left corner you 
can see conversion comparisons between a selected UOM and its base UOM  
  




**DFR UOM Editor – Guidelines**


·         
Editing 
UOM data – if a user right clicks on a UOM Name they are presented with three 
editing options including: set as Base UOM, Add UOM and Delete UOM.  The user also four other options which 
included editing the UOM Name, UOM Description, Conversion Factor or creating a 
Conversion Offset.  
  



·         
When 
you select a UOM Name the cell highlights in blue; now select F-2; the user can 
edit the UOM name without writing over the existing name  
  



·         
Changing 
the Base UOM – the base UOM is highlighted in bold text and has a conversion 
factor of 1.  A user can right click on 
another UOM and change it to a new base UOM.  
**The UOM Editor will automatically 
update the conversion factors to reflect the change of Base UOM**.    
  



·         
Changing 
the **Conversion Factors** – a user can 
type in any conversion factor for a new UOM just by typing it in.  This value is displayed in scientific 
notation only.  They can also include a 
Conversion Offset if the conversion formula lends itself to a value other than 
zero.  These conversion values are 
automatically changed if the base UOM is changed  
  



·         
**Moving UOM’s between UOM Types** – a user can move a UOM from one 
UOM type to another assuming it passes validations.  To move an UOM; select the UOM and drag the 
selected UOM to another UOM Type in the list.  
Once you’re over that UOM Type; you can release the UOM.  (same process as reclassifying in Item 
Browser)  You will notice as you’re 
selecting a new UOM type the cursor changes its display to indicate your moving 
a UOM.  If you are moving a UOM from 
General to a new UOM type you will have no validation issues to address; if 
your moving between UOM types other than General you may come across validation 
errors to fix prior to executing this change.


·         
**Editing UOM type data** – A user can create a new UOM Type; 
change the name of an existing UOM Type or delete a UOM type if they right 
click on the UOM list.


·         
Once 
you create a new UOM Type; you will have the option of creating the first UOM 
for that new UOM Type.  You will notice a 
new UOM is auto-created that has an auto generated unique name (GUID).  A user can type over that name to create a 
new UOM.


·         
**Saving UOM changes** – you can save UOM changes you make 
in your editing session to an XML file by selecting save.  This is useful if you have to leave the UOM 
tool to make edits.  When you check back 
into the UOM tool you will be prompted to load your past changes; if you choose 
not to load past changes you may loose them with future edits.



**DFR UOM Editor – Error Conditions**


·         
Creating 
duplicate UOM and UOM Type’s  
  



·         
Uploading 
an old saved XML file that conflicts with previous editing  
  



·         
Deleting 
UOM and UOM type that is used generates a warning and lists all its usages in 
DFR including: category attributes, attribute values and master attributes  
  



·         
Moving 
a UOM; that is used; from a non-General UOM Type to another UOM Type  
  



·         
Checking 
in changes while your in edit mode or while other DFR users are logged in




