



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
  



![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DFR_V3.6.8XX_Release_Notes_files/image001.jpg)




**Example of attachments for 
attributes in the attribute manager**



Once fully implemented, the attribute 
attachments will appear in the web applications including WebDFR and SmartFind as 
well as other modules in DFR.


This feature works similar to category 
attachments.  Both features work off of the URL attribute on the attachments 
category under non-parts (e.g. Root\Non-Parts\Attachments).  This category, in 
combination with the URL attribute, makes this feature work.


## ![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DFR_V3.6.8XX_Release_Notes_files/image002.jpg)


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


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DFR_V3.6.8XX_Release_Notes_files/image003.jpg)




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


**![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DFR_V3.6.8XX_Release_Notes_files/image004.jpg)**


**Example of leading and trailing white space 
warning message**



The same capability has been applied to the Allowed Values Manager 
when users are manually entered values for the allowed values list as shown 
below.


**![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DFR_V3.6.8XX_Release_Notes_files/image005.jpg)**


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

![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DFR_V3.6.8XX_Release_Notes_files/image006.jpg)

  
**Rename Item user interface.**


The bottom of the Rename Item window displays an error 
message a user might receive.  The following chart summarizes the 2 error 
conditions:




<table border="0" cellpadding="0" cellspacing="0" class="MsoNormalTable" style="width:403.0pt;margin-left:5.15pt;border-collapse:collapse" width="537"><tr style="height:12.75pt"><td nowrap="nowrap" style="width:32.0pt;border:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="43"><p align="center" class="MsoNormal" style="text-align:center"><b><span style='font-size:10.0pt;font-family:"Arial","sans-serif"'>#</span></b></p></td><td style="width:188.0pt;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="251"><p class="MsoNormal"><b><span style='font-size:10.0pt;font-family:"Arial","sans-serif"'>Error 
  Conditions</span></b></p></td><td style="width:183.0pt;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="244"><p class="MsoNormal"><b><span style='font-size:10.0pt;font-family:"Arial","sans-serif"'>Notes</span></b></p></td></tr><tr style="height:25.5pt"><td nowrap="nowrap" style="width:32.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:25.5pt" valign="bottom" width="43"><p align="center" class="MsoNormal" style="text-align:center"><b><span style='font-size:10.0pt;font-family:"Arial","sans-serif"'>1</span></b></p></td><td style="width:188.0pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:25.5pt" valign="bottom" width="251"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial","sans-serif"'>Rename 
  field.  Ttype in an existing Item Number/Qualifier combination.</span></p></td><td style="width:183.0pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:25.5pt" valign="bottom" width="244"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial","sans-serif"'>Can 
  only rename an item to a new item (primary key).  No duplicates are allowed.</span></p></td></tr><tr style="height:25.5pt"><td nowrap="nowrap" style="width:32.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:25.5pt" valign="bottom" width="43"><p align="center" class="MsoNormal" style="text-align:center"><b><span style='font-size:10.0pt;font-family:"Arial","sans-serif"'>2</span></b></p></td><td style="width:188.0pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:25.5pt" valign="bottom" width="251"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial","sans-serif"'>Type 
  in Item Number not assigned to you in the Original field.</span></p></td><td style="width:183.0pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:25.5pt" valign="bottom" width="244"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial","sans-serif"'>Items 
  have to be assigned to you before you can rename them.</span></p></td></tr></table>

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

![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DFR_V3.6.8XX_Release_Notes_files/image007.jpg)




**Reset Organization**


Items have to be assigned to you in order to be able to make 
changes.  If you try to change the qualifier on a batch of items not assigned 
to you, an error message will appear.  A list of items not assigned to you will 
also appear in the lower dialogue box.  You will notice the user field is 
either empty (see below) or has another user name listed.


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DFR_V3.6.8XX_Release_Notes_files/image008.jpg)




**Reset Organization Error 
Message for un-assigned items**


If your user name does appear in 
the dialogue box next to each item, then the error condition you have 
experienced is due to creating duplicates.  The items listed would be duplicate 
items to what is already in the database if the operation where to have 
completed.  


 


See the screen shot below that 
shows the duplicated item error message.  
  



![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DFR_V3.6.8XX_Release_Notes_files/image009.jpg)




**Reset Organization Error Message 
for duplicate items**  
Bugs Fixed and 
Enhancements in this Release:


 




<table border="0" cellpadding="0" cellspacing="0" class="MsoNormalTable" style="width:509.0pt;margin-left:4.65pt;border-collapse:collapse" width="679"><thead><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><b><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>CDS#</span></b></p></td><td style="width:60.55pt;border:solid windowtext 1.0pt; 
   border-left:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><b><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>Customer#</span></b></p></td><td style="width:265.45pt;border:solid windowtext 1.0pt; 
   border-left:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><b><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Issue Title</span></b></p></td><td nowrap="nowrap" style="width:92.0pt;border:solid windowtext 1.0pt; 
   border-left:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><b><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Application Module</span></b></p></td><td nowrap="nowrap" style="width:46.55pt;border:solid windowtext 1.0pt; 
   border-left:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><b><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Type</span></b></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1856</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>NG-168</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Implement Port Item Key Changer Dropin for new release</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>All</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Enh</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1855</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>NG-171</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Scrub Mechanical Part Attributes (remove nulls)</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Classification MGR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Enh</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1809</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-196</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Confirm window close</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>All</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Enh</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1945</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-314</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Ability to delete item(s) with SandboxMode off</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Item Browser</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1793</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>IB Relationship Tab Search Issue</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Item Browser</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1160</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Logfile beep: Category: Attachments is missing (see 1063)</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Classification MGR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1905</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Attribute Editor access for certain attributes inconsistent</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Classification MGR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1737</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>WebDFR Attribute Drop-Downs - due to AVM request failing</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Allowed Values MGR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1912</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Validation of Batch with No Required Attributes/Errors  
   Confusing</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Validator</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1932</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Category Tree window resize not working correctly</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Allowed Values MGR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1910</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Saving in Attribute Editor causes description to disappear</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Classification MGR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1805</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Prevent leading/trailing whitespace</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Enh</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1804</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Prevent leading/trailing whitespace</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Allowed Values MGR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Enh</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1790</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Classifying an Item in Item Browser</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Item Browser</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1866</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>DD- Application Error when using the horizontal scroll bar</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>159</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Search strings are case sensitive</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Item Browser</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1871</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>AM - attribute status does not show change</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Attribute MGR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1904</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Combo boxes are empty/invalid when first entering</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Attribute MGR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1877</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>AVM - Changes to Required Only check box does not update 
   attribute list</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Allowed Values MGR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1891</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Change to status of Required Does Not Register</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Classification MGR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1900</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Creating New Batch causes application error</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1569</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Change year design for Item Mapping</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Item Mapping</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Enh</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1886</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Change of Status is not registering</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Attribute MGR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1875</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>DD - Attribute Filters and Sorting Not Working - number values 
   registering as Null (Fix Class Mgr-UOM issue first #1861)</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1843</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>AVM and DD allows derivations of same value</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>All</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1798</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Stack Trace Error on Accept With Modification  </span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Allowed Values MGR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1836</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>AVM - Requests tab Application Error</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Allowed Values MGR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1667</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Module summary report</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Item Mapping</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1786</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Update date not getting set</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>All</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1776</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>IB Rt click Detail Items - Application Error</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Item Browser</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1173</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Items values can be deleted while approved or pending</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1236</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Allowed Values mgr not completely reconciling sentence case</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Allowed Values MGR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1240</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Any user can edit an approve attribute</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Attribute MGR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1245</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Oracle doesn't load more than 178 new relationships SQL does</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Item Loader</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1382</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Category Attachment URL is not showing up in attachments tab</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Classification MGR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1452</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>UOM in Oracle not working - not saving changes, etc</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>UOM Editor</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1890</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>SF Not Handling MultiVal Attrs Correctly</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>SmartFind</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1938</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>SmartFind Range Operation not working</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>SmartFind</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1872</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>IB BWI - Delete Working Batch not functioning properly</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Item Browser</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1924</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Create new stylesheet that contains base implementations for 
   customers</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>WebDFR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Enh</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1923</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Create new stylesheet that contains base implementations for 
   customers</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>SmartFind</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Enh</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1937</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Save Search only visible in advanced view</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>SmartFind</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1842</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>DD - Added Value Not Showing Up</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1892</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-299</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Replace the title "Collections/Relationships" with 
   "Relationship Attributes"</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>WebDFR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Enh</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1817</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-273</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Attribute barely visible in list window</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Attribute MGR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1723</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-267</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>UOM not set for general uom (SF and webDFR issue)</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>WebDFR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1929</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Cancel Button Not Reacting Properly: 'Beep CancelEdit'</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Attribute MGR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1807</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-237</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Change to attribute locking</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>All</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Enh</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1831</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>CDS client and remoting server hang forever after DB upgrade</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>All</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1823</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-62</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Provide ability to signal remoting server to refresh (reload) 
   its data without restarting</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>All</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Enh</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1844</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-292</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Implement read only for these controls – delete item year and 
   no replacement  </span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Item Mapping</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Enh</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1883</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Edit Item 'Item does not exist' message when the item does</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>WebDFR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1663</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-218</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Alignment missing between the variant no's and the roadmap when 
   mouse center button is used to scroll the page up and down  </span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Item Mapping</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1845</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-293</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Only have new items in 2010 appear in 2010 and not in 2009 
   (base year)</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Item Mapping</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Enh</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1846</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-294</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Investigate module map issues – copying to new year for large 
   road map causes application/computer to freeze  </span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Item Mapping</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1577</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Get Bob's DD view fixes into SQL for DFR</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1053</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Item Number for description template - Whirlpool request</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Classification MGR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Enh</span></p></td></tr></thead></table>

 




