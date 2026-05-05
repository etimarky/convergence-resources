



RIRename\_Item - Design For Retrieval (DFR) Help




**Rename 
Items**


 


 


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

![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/RI-Rename%20Item_files/image001.jpg)

  
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
  field.  Type in an existing Item Number/Qualifier combination.</p></td><td style="width:183.0pt;border-top:none;border-left: 
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

  
  



 


 




