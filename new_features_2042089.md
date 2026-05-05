



New\_Features - Design For Retrieval (DFR) Help




## Summary of New Features:


- Data 
 Developer – Better management of leading and trailing white space
- Classification 
 Manager – Category attribute supplemental description field and locking of 
 category attributes that are edited
- Attribute 
 Manager – Attachments for attributes, and attributes to support pictures 
 in SmartFind
- Allowed 
 Values Manager – Better management of leading and trailing white space
- General 
 – If a user accidently closes DFR window, they will be prompted with a 
 warning first
- Item 
 Key Changer – Allows users to change qualifiers and part numbers (optional 
 drop-in)

## DFR Module Specific Release Notes 
Attribute Manager:


 


Attachments for attributes can be set up in Attribute Manager to 
provide additional information on an attribute.  Attachments can be added to attributes 
on the new Attribute properties tab called Attachments.  User’s who have attribute 
edit privileges can add or remove attachments in this new field.  The Item Browser 
will display allowing a user to select an attachment out of the attachment’s 
category.  These attribute attachments will be accessible in other places in 
DFR and the web applications.  
  



![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/DFR_V3.6.8XX_Release_Notes_files/image001.jpg)




**Example of attachments for 
attributes in the attribute manager**



Once fully implemented, the attribute 
attachments will appear in the web applications including WebDFR and SmartFind as 
well as other modules in DFR.


This feature works similar to category 
attachments.  Both features work off of the URL attribute on the attachments 
category under non-parts (e.g. Root\Non-Parts\Attachments).  This category, in 
combination with the URL attribute, makes this feature work.


## ![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/DFR_V3.6.8XX_Release_Notes_files/image002.jpg)


**Example of attachments for 
attributes**


## 


## Classification Manager:


Each 
attribute has a description field that is created and maintained in the Attribute 
Manager as a global property.  A new supplemental description field can now be 
used to add additional information on an attribute specific to its use on a 
category in the Classification Manager.  This new extended description 
information can only be viewed for the category it is used on.  This 
information does not propagate to other instances of the attribute.


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/DFR_V3.6.8XX_Release_Notes_files/image003.jpg)




**Example of category attribute extended 
description field in the Classification Manager**


 


 


There 
is a new global attribute property that allows images (e.g. photos, drawings, 
etc.) to be displayed in SmartFind called ViewImageSize.  The size of the 
image can be configured from this attribute property (e.g. 800x1200).  Users 
can try different image size dimmensions until they determine their desired 
size.  See the attribute property help file for more information on this 
feature.


 


If a user is editing category attribute properties, only this 
category will be locked to other users trying to use it.  This includes WebDFR 
users.  In the past, all categories would be locked that used this attribute.  
This decreases the number of locking restrictions.


## Data Developer:


Data 
Developer now does a better job of managing unintended leading and trailing spaces.  
If a user happens to accidently include a space in a value field, (e.g. from a 
copy and paste), the Data Developer will recognize that space and prompt the 
user if it was intended.  


 


There 
is a global setting in the options manager that will allow this feature to be 
enabled or disabled.


## 


**![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/DFR_V3.6.8XX_Release_Notes_files/image004.jpg)**


**Example of leading and trailing white space 
warning message**



The same capability has been applied to the Allowed Values Manager 
when users are manually entered values for the allowed values list as shown 
below.


**![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/DFR_V3.6.8XX_Release_Notes_files/image005.jpg)**


**Example of trimming leading and trailing spaces in 
Allowed Values Manager**


  

# Rename Items


*Rename Items* allows users to rename an item including 
changing the item number, qualifier and the organization type.  This is a 
custom drop-in feature for DFR that is only available upon request.  Rename Item 
only processes one item at a time.  Here are some guidelines on this feature:


- Items have to be assigned to you in order to be able to 
 make changes to its primary key.
- You cannot change the qualifier type on an item.
- Only qualifiers that already exist in the database, not 
 necessarily used, are presented in the qualifier list for the renamed item 
 qualifier field.  This list is restricted to the qualifier type of the 
 original item.
- You cannot rename an item to another item’s exact primary 
 key.  This is recognized as a duplicate and will error out.
- The Try key allows a user to validate their change before 
 actually implementing the change.
- The OK key will implement the change as long as there are 
 no error conditions.
- There are only 2 possible error conditions including: (1) 
 item not assigned to user or (2) creating duplicate item.
- A user cannot make changes to an item while the Item 
 Loader is running.  A message will warn the user of this condition.
- The Cancel key can both cancel an operation or you select 
 cancel to exit out of the Rename Item application.
- The user needs to enter an item number first in the item 
 number field under the Original field.  Then hit tab to select the correct 
 qualifier.  In the example below, item number 100-222wib was entered and 
 qualifier Document.81205.ORG-ID was entered as the original item.

![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/DFR_V3.6.8XX_Release_Notes_files/image006.jpg)

  
**Rename Item user interface.**


The bottom of the Rename Item window displays an error 
message a user might receive.  The following chart summarizes the 2 error 
conditions:




<table border="0" cellpadding="0" cellspacing="0" class="MsoNormalTable" style="width:403.0pt;margin-left:5.15pt;border-collapse:collapse" width="537"><tr style="height:12.75pt"><td nowrap="nowrap" style="width:32.0pt;border:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="43"><p align="center" class="MsoNormal" style="text-align:center"><b>#</b></p></td><td style="width:188.0pt;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="251"><p class="MsoNormal"><b>Error 
  Conditions</b></p></td><td style="width:183.0pt;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="244"><p class="MsoNormal"><b>Notes</b></p></td></tr><tr style="height:25.5pt"><td nowrap="nowrap" style="width:32.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:25.5pt" valign="bottom" width="43"><p align="center" class="MsoNormal" style="text-align:center"><b>1</b></p></td><td style="width:188.0pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:25.5pt" valign="bottom" width="251"><p class="MsoNormal">Rename 
  field.  Ttype in an existing Item Number/Qualifier combination.</p></td><td style="width:183.0pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:25.5pt" valign="bottom" width="244"><p class="MsoNormal">Can 
  only rename an item to a new item (primary key).  No duplicates are allowed.</p></td></tr><tr style="height:25.5pt"><td nowrap="nowrap" style="width:32.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:25.5pt" valign="bottom" width="43"><p align="center" class="MsoNormal" style="text-align:center"><b>2</b></p></td><td style="width:188.0pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:25.5pt" valign="bottom" width="251"><p class="MsoNormal">Type 
  in Item Number not assigned to you in the Original field.</p></td><td style="width:183.0pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:25.5pt" valign="bottom" width="244"><p class="MsoNormal">Items 
  have to be assigned to you before you can rename them.</p></td></tr></table>

# 


# Reset Organizations


*Reset Organization* allows users to change a batch of 
items qualifiers in a single operation.  This is a custom drop-in feature that 
is available upon request.  It is not a core application.  Here are some 
guidelines to using this application.


- A user cannot make changes to an item while the Item 
 Loader is running.  A message will warn the user of this condition.
- You cannot change the qualifier type of a batch.
- Batches with different qualifier types do not show up in 
 the batch list to process.
- Batches that contain organizations from the organization 
 category do not show up in the batch list.  Any batch with organization as 
 the qualifier type cannot be processed.  To change these types of items, a 
 user can do this on a individual basis using the rename item function.
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
 no error conditions.
- There are only 2 possible error conditions including (1) 
 item not assigned to user or (2) creating duplicate item.
- The Cancel key can both cancel an operation or you select 
 cancel to exit out of this Rename Item application.
- The user needs to select a batch from the batch list then 
 select a qualifier to process a change of qualifier for the batch 
 selected.  See the screen shot below:

![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/DFR_V3.6.8XX_Release_Notes_files/image007.jpg)




**Reset Organization**


Items have to be assigned to you in order to be able to make 
changes.  If you try to change the qualifier on a batch of items not assigned 
to you, an error message will appear.  A list of items not assigned to you will 
also appear in the lower dialogue box.  You will notice the user field is 
either empty (see below) or has another user name listed.


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/DFR_V3.6.8XX_Release_Notes_files/image008.jpg)




**Reset Organization Error 
Message for un-assigned items**


If your user name does appear in 
the dialogue box next to each item, then the error condition you have 
experienced is due to creating duplicates.  The items listed would be duplicate 
items to what is already in the database if the operation where to have 
completed.  


 


See the screen shot below that 
shows the duplicated item error message.  
  



![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/DFR_V3.6.8XX_Release_Notes_files/image009.jpg)




**Reset Organization Error Message 
for duplicate items**  
 
Bugs Fixed and 
Enhancements in this Release:


 




<table border="0" cellpadding="0" cellspacing="0" class="MsoNormalTable" style="width:509.0pt;margin-left:4.65pt;border-collapse:collapse" width="679"><thead><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><b>CDS#</b></p></td><td style="width:60.55pt;border:solid windowtext 1.0pt; 
   border-left:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><b>Customer#</b></p></td><td style="width:265.45pt;border:solid windowtext 1.0pt; 
   border-left:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><b>Issue Title</b></p></td><td nowrap="nowrap" style="width:92.0pt;border:solid windowtext 1.0pt; 
   border-left:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><b>Application Module</b></p></td><td nowrap="nowrap" style="width:46.55pt;border:solid windowtext 1.0pt; 
   border-left:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><b>Type</b></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1856</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">NG-168</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Implement Port Item Key Changer Dropin for new release</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">All</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1855</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">NG-171</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Scrub Mechanical Part Attributes (remove nulls)</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Classification MGR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1809</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-196</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Confirm window close</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">All</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1945</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-314</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Ability to delete item(s) with SandboxMode off</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Browser</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1793</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">IB Relationship Tab Search Issue</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Browser</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1160</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Logfile beep: Category: Attachments is missing (see 1063)</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Classification MGR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1905</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Attribute Editor access for certain attributes inconsistent</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Classification MGR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1737</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">WebDFR Attribute Drop-Downs - due to AVM request failing</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Allowed Values MGR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1912</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Validation of Batch with No Required Attributes/Errors  
   Confusing</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Validator</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1932</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Category Tree window resize not working correctly</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Allowed Values MGR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1910</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Saving in Attribute Editor causes description to disappear</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Classification MGR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1805</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Prevent leading/trailing whitespace</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1804</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Prevent leading/trailing whitespace</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Allowed Values MGR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1790</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Classifying an Item in Item Browser</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Browser</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1866</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">DD- Application Error when using the horizontal scroll bar</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">159</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Search strings are case sensitive</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Browser</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1871</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">AM - attribute status does not show change</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Attribute MGR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1904</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Combo boxes are empty/invalid when first entering</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Attribute MGR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1877</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">AVM - Changes to Required Only check box does not update 
   attribute list</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Allowed Values MGR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1891</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Change to status of Required Does Not Register</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Classification MGR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1900</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Creating New Batch causes application error</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1569</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Change year design for Item Mapping</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Mapping</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1886</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Change of Status is not registering</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Attribute MGR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1875</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">DD - Attribute Filters and Sorting Not Working - number values 
   registering as Null (Fix Class Mgr-UOM issue first #1861)</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1843</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">AVM and DD allows derivations of same value</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">All</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1798</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Stack Trace Error on Accept With Modification  </p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Allowed Values MGR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1836</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">AVM - Requests tab Application Error</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Allowed Values MGR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1667</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Module summary report</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Mapping</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1786</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Update date not getting set</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">All</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1776</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">IB Rt click Detail Items - Application Error</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Browser</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1173</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Items values can be deleted while approved or pending</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1236</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Allowed Values mgr not completely reconciling sentence case</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Allowed Values MGR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1240</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Any user can edit an approve attribute</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Attribute MGR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1245</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Oracle doesn't load more than 178 new relationships SQL does</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Loader</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1382</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Category Attachment URL is not showing up in attachments tab</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Classification MGR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1452</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">UOM in Oracle not working - not saving changes, etc</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">UOM Editor</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1890</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">SF Not Handling MultiVal Attrs Correctly</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">SmartFind</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1938</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">SmartFind Range Operation not working</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">SmartFind</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1872</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">IB BWI - Delete Working Batch not functioning properly</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Browser</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1924</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Create new stylesheet that contains base implementations for 
   customers</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">WebDFR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1923</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Create new stylesheet that contains base implementations for 
   customers</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">SmartFind</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1937</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Save Search only visible in advanced view</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">SmartFind</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1842</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">DD - Added Value Not Showing Up</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1892</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-299</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Replace the title "Collections/Relationships" with 
   "Relationship Attributes"</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">WebDFR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1817</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-273</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Attribute barely visible in list window</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Attribute MGR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1723</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-267</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">UOM not set for general uom (SF and webDFR issue)</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">WebDFR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1929</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Cancel Button Not Reacting Properly: 'Beep CancelEdit'</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Attribute MGR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1807</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-237</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Change to attribute locking</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">All</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1831</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">CDS client and remoting server hang forever after DB upgrade</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">All</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1823</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-62</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Provide ability to signal remoting server to refresh (reload) 
   its data without restarting</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">All</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1844</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-292</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Implement read only for these controls – delete item year and 
   no replacement  </p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Mapping</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1883</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Edit Item 'Item does not exist' message when the item does</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">WebDFR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1663</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-218</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Alignment missing between the variant no's and the roadmap when 
   mouse center button is used to scroll the page up and down  </p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Mapping</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1845</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-293</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Only have new items in 2010 appear in 2010 and not in 2009 
   (base year)</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Mapping</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1846</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-294</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Investigate module map issues – copying to new year for large 
   road map causes application/computer to freeze  </p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Mapping</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1577</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Get Bob's DD view fixes into SQL for DFR</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center">1053</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Item Number for description template - Whirlpool request</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Classification MGR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr></thead></table>

 




