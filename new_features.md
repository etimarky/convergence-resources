



New\_Features - Design For Retrieval (DFR) Help




## Summary of New Features:


- Item 
 browser – one or more selected items can be deleted.  Users can more 
 easily remove an item from a working batch or all working batches it 
 belongs too.  Also protected batches can be created and protected from 
 deletion.
- Data 
 Developer – users can delete one or more items in DFR from Data Developer.
- Classification 
 Manager – users can select more than one category and submit those categories 
 selected for status change all at once.
- User 
 Manager – a new role has been added called protected batches.  Batches can 
 now be protected and only users with this new role can edit or delete 
 them.
- Attribute 
 Manager – 3 new custom attributes can now be used in DFR, WebDFR and 
 SmartFind including: multi-value, vector and range.
- Item 
 Loader – now supports items that have DNA – does not apply values
- Allowed 
 Values Manager – users can now request new allowed values from WebDFR and 
 the allowed values manager can process these requests.  Approved, modified 
 and rejected requests will be emailed back to the submitter of the allowed 
 values.  Special diagnostics protects against concurrency issues, 
 therefore multiple users can now use this application at once..

## DFR Module Specific Release Notes 
Item Browser: (Deleting Items)


 


To 
delete an item or multiple items from DFR open either the Data Developer or the 
Item Browser module and perform a search to match the desired items.  Once the 
results are displayed, select one or many returned rows (highlighting the 
entire row).  Right click the selected rows; in the context menu choose “Delete 
Item(s)”.


 


***Note***: The “Delete 
Items(s) context menu option will only be active if the current user is 
assigned to ALL the selected items.


 


![](images/DFR_V3.6.810_Release_Notes001.jpg)




**Example of deleting an item from 
the Item Browser in DFR**


 


 


***Note***: In sandbox mode, an 
item of any status will be deleted.  If not sandbox mode, only items of new 
status will be deleted, all others will be marked obsolete.


 


 


## Item Browser: (Removing Items from Working Batch)


 


To 
remove an item from a working batch via Data Developer or Item Browser open the 
corresponding module and perform a search to match the desired items.  Once the 
results are displayed, select the item to delete (highlighting the entire 
row).  Right click the selected row; in the context menu choose “Delete Item 
From Working Batches…”.


 


***Note***: The “Delete Item 
From Working Batches…” context menu option will only be active if one item is 
selected.  The item is not deleted from DFR database, just removed from the 
selected working batches.


 


![](images/DFR_V3.6.810_Release_Notes002.jpg)




**Example of removing an item from a working 
batch**


 


A 
resulting dialog will be displayed.  This dialog lists all the working batches 
for the selected item.  On this dialog, select one or multiple working batches 
which the item will be removed from.  Once the selection is made, click “OK”.


 


![](images/DFR_V3.6.810_Release_Notes003.jpg)




**Example of selecting working batches to 
remove a particular item**


***Note***: Upon removing the 
item from the selected working batches, Item Browser will not update the Batch 
totals until the search results are refreshed.  This can be performed by 
searching again.  In Data Developer, the batch totals are automatically updated 
if “Auto Retrieve After Filtering” is enabled.


 


If 
a user has protected batch role, set in the user manager, they can create 
protected batches in the item browser.  Only those with this role can delete or 
edit protected batches.  Users that do not have protected batch role will not 
see protected batches in the Manage Existing Working Batches screen.  All users 
will be able to use protected batches as a search batch filter.


 


![](images/DFR_V3.6.810_Release_Notes004.jpg)




**Example of setting protected batches in Item 
Browser**


## 



## Classification Manager:


Users 
with the correct privileges in Classification Manager can select more than one 
category and submit for status change.  The selected categories must be of the 
same status for this gang approval process to work properly.


 


![](images/DFR_V3.6.810_Release_Notes005.jpg)




**Example of gang category status change**


 


 



## Data Developer:


Users 
can delete items that are assigned to them in Data Developer as long as the DFR 
catalog is in sandbox mode.


## 


***![](images/DFR_V3.6.810_Release_Notes006.jpg)***


**Example of deleting items in Data Developer**



  

Users 
can also remove items from multiple working batches from the Data Developer.



**![](images/DFR_V3.6.810_Release_Notes007.jpg)**


**Example of deleting/removing an item from 
multiple working batches**


 


Once 
an item is selected for working batch removal, a list of working batches that 
it is in gets displayed.  From here the user can select what working batches to 
remove the item.



**![](images/DFR_V3.6.810_Release_Notes008.jpg)**


**Example of selecting which working batches to 
remove an item** 



## Item Loader:


The item loader will allow users to load data that includes 
DNA settings.  This will only work if the attribute in DFR has been DNA 
enabled.  The value the user can enter into a load file, for a DNA enabled 
attribute, is <DNA>.


## 


## Allowed Values Manager: (Multi-user)


More 
than one user can now use and edit data in the allowed values manager.  Special 
diagnostics have been put in place to keep users from saving changes for the 
same attribute value list.


 


![](images/DFR_V3.6.810_Release_Notes009.jpg)




**Example of managing concurrency when users 
are modifying the same allowed values list**


 


Restrict 
to category will limit the attributes displayed in allowed values manager to 
the attributes for the selected category.  If you do not select ‘restrict to 
category’, the allowed values manager will show you all the attributes for that 
category and all the attributes for the subcategories below.


## ![](images/DFR_V3.6.810_Release_Notes010.jpg)


**Example 
of restrict to category, limits attributes displayed to selected category**


## Allowed Values Manager: (Request for attribute value)


From 
WebDFR (Whirlpool calls Item Classification) users can request new allowed 
values from the view below.


 


![](images/DFR_V3.6.810_Release_Notes011.jpg)




**Example of submitting new allowed values from 
WebDFR (Item Classification)**



All 
allowed values requests can be processed in the Allowed Values Manager.  There 
is a tab called Requests which the user can select this tab to view the 
requests as shown below.  It does not matter what category you have selected, 
all requests can be viewed and processed from any category.


 


**![](images/DFR_V3.6.810_Release_Notes012.jpg)**


**Example** **of viewing allowed values requests in 
the Allowed Values Manager**


## 


The 
Allowed Values Manager has 5 options for accepting requested allowed values 
including:


1. Add 
 them as-is to the global list
2. Add 
 them as-is to the local list (Note: for the category it came from only)
3. Modify 
 them then assign to global list
4. Modify 
 them then assign to local list (Note: for the category it came from only)
5. Assign 
 them to an existing value (local or global)

 


For 
the first two options, an acceptance email will be sent out to the requestor, 
letting them know their allowed value has been approved.


 


***Note***: a user can only add 
an allowed values request to existing lists, if there is not a global or local 
list for the attribute, otherwise those options will be grayed out.


 


![](images/DFR_V3.6.810_Release_Notes013.jpg)




**Example of accepting new allowed values 
requests**



  

If 
the user chooses to modify an Allowed Values Request, they can type in the new 
value in the drop down list and choose to add it to a local or global list.  
The user may also want to type a note describing why a change was made.  This 
note will go out in an email to the original allowed values requestor.



**![](images/DFR_V3.6.810_Release_Notes014.jpg)**


**Example of modifying an Allowed Value Request**




  

A user can reject changes submitted by the 
requester.  They will be presented with a notes field to enter their comments 
describing why they rejected the request.  This will be emailed to the 
requester.***![](images/DFR_V3.6.810_Release_Notes015.jpg)***


**Example of rejecting an Allowed Values 
Request**



In 
some cases users may submit the same Allowed Values Request for the same 
attribute and category.  These requests will be grouped together so they can be 
processed together.  Those that have a request count greater than 1 have been 
grouped, as displayed below.



![](images/DFR_V3.6.810_Release_Notes016.jpg)




**Example of the same attribute value request 
for the same category and attribute****Bugs 
Fixed and Enhancements in this Release:**


 




<table border="0" cellpadding="0" cellspacing="0" class="MsoNormalTable" style="width:509.0pt;margin-left:4.65pt;border-collapse:collapse" width="679"><thead><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="center" class="MsoNormal" style="text-align:center"><b><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>CDS 
   Issue #</span></b></p></td><td style="width:56.45pt;border:solid windowtext 1.0pt; 
   border-left:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="center" class="MsoNormal" style="text-align:center"><b><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>Whirlpool 
   Issue #</span></b></p></td><td style="width:269.25pt;border:solid windowtext 1.0pt; 
   border-left:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal"><b><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Issue Description</span></b></p></td><td nowrap="nowrap" style="width:92.0pt;border:solid windowtext 1.0pt; 
   border-left:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><b><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Application</span></b></p></td><td nowrap="nowrap" style="width:46.55pt;border:solid windowtext 1.0pt; 
   border-left:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><b><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Type</span></b></p></td></tr></thead><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1638</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Release Lock in DFR</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>All</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1548</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>149</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Mouse-Over extended info (Batch names)</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>All</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1543</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>SF "Item Number" Attribute "Ignore" filter 
  (SearchAPI)</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>All</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1380</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Invalid URL for home page fails poorly</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>All</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1231</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Protection from items stored under non-terminal nodes</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>All</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>434</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Cannot see buttons in 120 DPI; Editing Load Templates</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>All</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>80</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Add info to notification email</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>All</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Enh</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>126</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Provide protected batches with associated role</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>All</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Enh</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>131</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Right click removal of item from working batch</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>All</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Enh</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>179</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Item number sorting</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>All</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Enh</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>191</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Need to understand locking scenarios  </span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>All</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Support</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>229</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>DFR Client only displaying Data Developer</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>All</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Support</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>204</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Oracle timeout - VPN connection</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>All</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Support</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>170</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Expand size allowed values list names [Cannot set 'VchName']</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Allowed Values</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1685</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>234</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Stack Trace Error - Null Values  </span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Allowed Values</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1668</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Offer a Restrict to Category Attributes check box</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Allowed Values</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1651</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>AVM not handling multivals - find the values</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Allowed Values</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1643</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>213</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Local Allowed Values saving to Category which is selected next</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Allowed Values</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>189</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Allow concurrent users  </span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Allowed Values</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Enh</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>245</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>More than one person working with Allowed Values (Replaced by 
  issues 189/194)</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Allowed Values</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Enh</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>115</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Allow concurrent users  </span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Allowed Values</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Enh</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>236</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>"Unnamed" as heading for "Global" AVM List</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Allowed Values</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Support</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1117</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>UOM Type = None reported issue by Brad at Whirlpool</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Attribute Manager</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>47</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Do not reset filter after editing an attribute</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Attribute Manager</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Enh</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1697</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>252</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Cannot Delete Subcategories or Parent Category</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Classification MGR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1506</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Submit on any key attribute causes application to close.</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Classification MGR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1492</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Approvers cannot change display order</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Classification MGR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1162</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>74</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Notification users do not get notified</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Classification MGR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1056</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Cannot reset a qualifier alias name (full qualifier)</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Classification MGR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1053</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Item Number for description template - Whirlpool request</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Classification MGR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>165</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Disallow "\" in category names</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Classification MGR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Enh</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>176</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>"Gang" category status editing</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Classification MGR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Enh</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>186</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Disallow leading and trailing spaces on category names  </span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Classification MGR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Enh</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>166</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Unexpected Column Error</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1711</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Data Developer Batch resets to ALL after Manage Working Batches 
  dialog box</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1708</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Data Developer Views... dialog box Delete button becomes grayed 
  out</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1707</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Data Developer Changing Assigned User</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1700</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Unable to Retrieve Sort Data on Create Date. </span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1698</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Blank columns </span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1683</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Regional data entry issue </span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1662</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Vector issues to resolve - double click, etc.</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1646</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>216</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Exports from DD missing Category Path information  </span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1639</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Data Developer doesn't save</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1607</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Update warning message in DD after attrs been removed to use 
  Reset Columns</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1563</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Batch name over 50 chars has ugly failure</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1342</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Switching from validation to normal mode doesn’t update title in 
  application header</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1320</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Sort order changes in export file</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1173</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>84</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Can delete attribute value from pending item</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1041</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Paste from excel with no UOM column creates stack trace oracle</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>87</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Provide pull down for Boolean</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Enh</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>120</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Provide ability to flag an attribute value as "does not 
  apply" for an item</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Enh</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>138</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Provide ability to get to relationship data</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Enh</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>169</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Set browse mode on by default</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Enh</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>193</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Readability improvement</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Enh</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>195</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Save and Restored WIP</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Enh</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>25</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>DV is not handling values with embedded spaces</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Data Validator</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1703</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Data Validator - Batch set to ALL</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Data Validator</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1259</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>URL validations only for http - should cover all URLs</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Data Validator</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1132</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Uom conversion errors</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Database</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1635</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Have PingDFR display mode (SIMPLE, LOGIN, ORACLE, etc.)</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Installation</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1710</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Item Browser Batch drop down text disappears after Manage 
  Working Batches dialog box</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Item Browser</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1666</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Item Browser Search for a String is Case Sensitive </span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Item Browser</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1621</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Item Browser wrt Oracle and case-in/sensitivity </span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Item Browser</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1507</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Canceling Collections tab search causes application to close. 
  (Rich cant replicate in SQL or Oracle)</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Item Browser</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>171</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Ability to delete single item or group of items</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Item Browser</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Enh</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>206</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Blank Item Browser</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Item Browser</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Support</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1592</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>DNA for Item Loader</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Item Loader</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Enh</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1475</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Unknown Error loading template in item loader </span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Item Loader</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1287</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Cant load a new batch of items, limited diagnostics why</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Item Loader</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>235</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Relationship Load File Error Report -&gt; Shows Incorrect 
  Results (Missing Load Files)</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Item Loader</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Support</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>209</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Owner group not updated in item mapping tool</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Item Mapping</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>219</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Error while generating module type summary report</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Item Mapping</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>262</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>large Space between one variant to other variant within a given 
  module  </span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Item Mapping</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>263</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Module Summary Report Error</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Item Mapping</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1673</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>226</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Module summary report - error</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Item Mapping</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1672</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>227</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Extremely long save time &amp; Frequent crashes or system hang 
  ups</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Item Mapping</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:45.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:45.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1663</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:45.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>218</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:45.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Alignment missing between the variant no's and the roadmap when 
  mouse center button is used to scroll the page up and down</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:45.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Item Mapping</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:45.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1699</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>259</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Module summary report  error  </span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Item Mapping</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Support</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1667</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>222</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Module summary report</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Item Mapping</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Support</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1692</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Import Issues</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>NGAPI</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1584</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Attribute name: "Material Code" should be configurable</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>NGAPI</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1169</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>NGAPI should use full qualifier paths as supported by v3.6</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>NGAPI</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>81</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Provide ability to update item description and legacy PN</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>NGAPI</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Enh</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>136</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Manage category roles</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>NGAPI</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Enh</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>160</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Provide ability to flag an attribute value as "does not 
  apply" for an item</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>NGAPI</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Enh</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1527</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Reports not working</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Reports</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>147</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Text wrap across multiple columns</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>SmartFind</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1712</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>SmartFind Attribute Filter MATERIAL GRADE</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>SmartFind</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1702</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Lists not handling duplicates correctly</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>SmartFind</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1688</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Selected Template name disappears on category filter change</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>SmartFind</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1679</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Error message for case sensitive logins - SF Oracle</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>SmartFind</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1677</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Alias names not showing up in Item Detailed info page</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>SmartFind</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1675</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>We need a better way to build/test wrt WSSO files</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>SmartFind</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1674</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>New SF not stretching search result to right with many attribute 
  column</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>SmartFind</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1669</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>225</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>XML file has no items in it  in Whirlpool version of SF</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>SmartFind</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1657</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Range values not showing up in SF</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>SmartFind</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1647</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>LiveUpdate not handling data model changes</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>SmartFind</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1626</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Find similar returns blank page</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>SmartFind</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1624</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>List Fails under Oracle containing more than 100 items</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>SmartFind</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1620</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>SmartFind Attribute Values for Item: AA03023WIB4</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>SmartFind</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1618</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>SmartFind Item Cart Add Items Issue</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>SmartFind</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1612</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>New Build Scripts Issue SmartFind</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>SmartFind</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1538</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Attribproperty Key error</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>SmartFind</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:45.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:45.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1518</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:45.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:45.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Cannot view an item from the Item Cart after running a Custom 
  Search if it was not a result of the Custom Search</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:45.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>SmartFind</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:45.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1511</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>SmartFind: Loading values for Attribute filter causes internal 
  server error. (search API issue)</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>SmartFind</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1355</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>DataReader discipline</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>SmartFind</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1333</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>SmartFind Service Broker and DB Movement</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>SmartFind</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1226</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>List-filter has performance issues when very large.</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>SmartFind</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1213</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Fix the Search Criteria Grid so it does not create large gap to 
  right</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>SmartFind</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1193</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Cannot sort a category with a Numeric attr set as General 
  (Search API issue?)</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>SmartFind</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>244</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Docs for 3 New Operators in SmartFind Attribute Filters </span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>SmartFind</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Doc</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>157</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Display "does not apply" attribute values</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>SmartFind</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Enh</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>168</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Allow "*" as wildcard</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>SmartFind</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Enh</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>201</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Ability to edit search text in advanced search</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>SmartFind</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Enh</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1670</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>SF Export from within Search Results</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>SmartFind</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Enh</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>145</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Custom search issue</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>SmartFind</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Support</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1605</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Uom Editor vs SmartFind </span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>UOM Editor</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1601</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Unit type changes don't really save</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>UOM Editor</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1678</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>User Manager Issue</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>User Manager</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>152</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Unable to Re-Classify an Item</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>WebDFR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>253</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Item Classification Help does not work</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>WebDFR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1719</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>WebDFR Edit Item 'Item does not exits'</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>WebDFR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1717</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>WebDFR Help Link</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>WebDFR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1681</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>232</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Items not in terminal categories</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>WebDFR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1680</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>230</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Item Classification internal error</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>WebDFR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1671</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>162</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Read only relationship attributes can be edited</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>WebDFR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1661</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Ensure that incorrect filtered category paths are being logged</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>WebDFR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1655</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Adding items to more than one collection in a single edit 
  creates load issue</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>WebDFR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1654</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Creating an item from a clone with relationships</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>WebDFR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1650</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Filtered Categories don't handle bad paths</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>WebDFR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1649</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>WebDFR Installation Issue</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>WebDFR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1611</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>New Build Script Issue with WebDFR</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>WebDFR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1558</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Descriptions using '#' get truncated</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>WebDFR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1533</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Cannot use a webDFR created clone (vs. SF created clone)</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>WebDFR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1476</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Item Type Code comparison shouldn’t be case sensitive for clones</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>WebDFR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>158</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Provide ability to flag an attribute value as "does not 
  apply" for an item</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>WebDFR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Enh</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>190</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Category attachments exposed on attribute entry screen  </span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>WebDFR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Enh</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>224</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Expose category attachments on attribute entry page</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>WebDFR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Enh</span></p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>250</span></p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Request allowed value</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>WebDFR</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
  color:black'>Enh</span></p></td></tr></table>

 




