



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
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="center" class="MsoNormal" style="text-align:center"><b>CDS 
   Issue #</b></p></td><td style="width:56.45pt;border:solid windowtext 1.0pt; 
   border-left:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="center" class="MsoNormal" style="text-align:center"><b>Whirlpool 
   Issue #</b></p></td><td style="width:269.25pt;border:solid windowtext 1.0pt; 
   border-left:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal"><b>Issue Description</b></p></td><td nowrap="nowrap" style="width:92.0pt;border:solid windowtext 1.0pt; 
   border-left:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><b>Application</b></p></td><td nowrap="nowrap" style="width:46.55pt;border:solid windowtext 1.0pt; 
   border-left:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><b>Type</b></p></td></tr></thead><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1638</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Release Lock in DFR</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">All</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1548</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">149</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Mouse-Over extended info (Batch names)</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">All</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1543</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">SF "Item Number" Attribute "Ignore" filter 
  (SearchAPI)</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">All</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1380</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Invalid URL for home page fails poorly</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">All</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1231</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Protection from items stored under non-terminal nodes</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">All</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">434</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Cannot see buttons in 120 DPI; Editing Load Templates</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">All</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">80</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Add info to notification email</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">All</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">126</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Provide protected batches with associated role</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">All</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">131</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Right click removal of item from working batch</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">All</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">179</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Item number sorting</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">All</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">191</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Need to understand locking scenarios  </p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">All</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Support</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">229</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">DFR Client only displaying Data Developer</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">All</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Support</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">204</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Oracle timeout - VPN connection</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">All</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Support</p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">170</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal">Expand size allowed values list names [Cannot set 'VchName']</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Allowed Values</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1685</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">234</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Stack Trace Error - Null Values  </p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Allowed Values</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1668</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Offer a Restrict to Category Attributes check box</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Allowed Values</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1651</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">AVM not handling multivals - find the values</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Allowed Values</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1643</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">213</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal">Local Allowed Values saving to Category which is selected next</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Allowed Values</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">189</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Allow concurrent users  </p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Allowed Values</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">245</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal">More than one person working with Allowed Values (Replaced by 
  issues 189/194)</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Allowed Values</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">115</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Allow concurrent users  </p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Allowed Values</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">236</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">"Unnamed" as heading for "Global" AVM List</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Allowed Values</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Support</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1117</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">UOM Type = None reported issue by Brad at Whirlpool</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Attribute Manager</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">47</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Do not reset filter after editing an attribute</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Attribute Manager</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1697</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">252</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Cannot Delete Subcategories or Parent Category</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Classification MGR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1506</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Submit on any key attribute causes application to close.</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Classification MGR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1492</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Approvers cannot change display order</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Classification MGR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1162</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">74</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Notification users do not get notified</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Classification MGR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1056</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Cannot reset a qualifier alias name (full qualifier)</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Classification MGR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1053</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal">Item Number for description template - Whirlpool request</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Classification MGR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">165</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Disallow "\" in category names</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Classification MGR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">176</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">"Gang" category status editing</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Classification MGR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">186</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Disallow leading and trailing spaces on category names  </p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Classification MGR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">166</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Unexpected Column Error</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1711</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal">Data Developer Batch resets to ALL after Manage Working Batches 
  dialog box</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1708</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal">Data Developer Views... dialog box Delete button becomes grayed 
  out</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1707</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Data Developer Changing Assigned User</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1700</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Unable to Retrieve Sort Data on Create Date. </p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1698</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Blank columns </p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1683</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Regional data entry issue </p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1662</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Vector issues to resolve - double click, etc.</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1646</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">216</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Exports from DD missing Category Path information  </p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1639</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Data Developer doesn't save</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1607</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal">Update warning message in DD after attrs been removed to use 
  Reset Columns</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1563</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Batch name over 50 chars has ugly failure</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1342</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal">Switching from validation to normal mode doesn’t update title in 
  application header</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1320</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Sort order changes in export file</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1173</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">84</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Can delete attribute value from pending item</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1041</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal">Paste from excel with no UOM column creates stack trace oracle</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">87</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Provide pull down for Boolean</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">120</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal">Provide ability to flag an attribute value as "does not 
  apply" for an item</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">138</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Provide ability to get to relationship data</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">169</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Set browse mode on by default</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">193</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Readability improvement</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">195</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Save and Restored WIP</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">25</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">DV is not handling values with embedded spaces</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Validator</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1703</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Data Validator - Batch set to ALL</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Validator</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1259</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">URL validations only for http - should cover all URLs</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Validator</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1132</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Uom conversion errors</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Database</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1635</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Have PingDFR display mode (SIMPLE, LOGIN, ORACLE, etc.)</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Installation</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1710</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal">Item Browser Batch drop down text disappears after Manage 
  Working Batches dialog box</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Browser</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1666</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Item Browser Search for a String is Case Sensitive </p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Browser</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1621</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Item Browser wrt Oracle and case-in/sensitivity </p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Browser</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1507</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal">Canceling Collections tab search causes application to close. 
  (Rich cant replicate in SQL or Oracle)</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Browser</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">171</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Ability to delete single item or group of items</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Browser</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">206</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Blank Item Browser</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Browser</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Support</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1592</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">DNA for Item Loader</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Loader</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1475</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal">Unknown Error loading template in item loader </p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Loader</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1287</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Cant load a new batch of items, limited diagnostics why</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Loader</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">235</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal">Relationship Load File Error Report -&gt; Shows Incorrect 
  Results (Missing Load Files)</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Loader</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Support</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">209</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Owner group not updated in item mapping tool</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Mapping</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">219</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Error while generating module type summary report</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Mapping</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">262</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal">large Space between one variant to other variant within a given 
  module  </p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Mapping</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">263</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Module Summary Report Error</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Mapping</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1673</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">226</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Module summary report - error</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Mapping</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1672</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">227</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal">Extremely long save time &amp; Frequent crashes or system hang 
  ups</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Mapping</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:45.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:45.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1663</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:45.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">218</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:45.0pt" valign="bottom" width="359"><p class="MsoNormal">Alignment missing between the variant no's and the roadmap when 
  mouse center button is used to scroll the page up and down</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:45.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Mapping</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:45.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1699</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">259</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Module summary report  error  </p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Mapping</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Support</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1667</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">222</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Module summary report</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Mapping</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Support</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1692</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Import Issues</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">NGAPI</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1584</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Attribute name: "Material Code" should be configurable</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">NGAPI</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1169</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal">NGAPI should use full qualifier paths as supported by v3.6</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">NGAPI</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">81</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Provide ability to update item description and legacy PN</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">NGAPI</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">136</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Manage category roles</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">NGAPI</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">160</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal">Provide ability to flag an attribute value as "does not 
  apply" for an item</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">NGAPI</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1527</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Reports not working</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">Reports</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">147</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Text wrap across multiple columns</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">SmartFind</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1712</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">SmartFind Attribute Filter MATERIAL GRADE</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">SmartFind</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1702</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Lists not handling duplicates correctly</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">SmartFind</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1688</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal">Selected Template name disappears on category filter change</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">SmartFind</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1679</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Error message for case sensitive logins - SF Oracle</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">SmartFind</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1677</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Alias names not showing up in Item Detailed info page</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">SmartFind</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1675</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">We need a better way to build/test wrt WSSO files</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">SmartFind</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1674</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal">New SF not stretching search result to right with many attribute 
  column</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">SmartFind</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1669</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">225</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">XML file has no items in it  in Whirlpool version of SF</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">SmartFind</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1657</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Range values not showing up in SF</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">SmartFind</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1647</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">LiveUpdate not handling data model changes</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">SmartFind</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1626</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Find similar returns blank page</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">SmartFind</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1624</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">List Fails under Oracle containing more than 100 items</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">SmartFind</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1620</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">SmartFind Attribute Values for Item: AA03023WIB4</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">SmartFind</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1618</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">SmartFind Item Cart Add Items Issue</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">SmartFind</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1612</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">New Build Scripts Issue SmartFind</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">SmartFind</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1538</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Attribproperty Key error</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">SmartFind</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:45.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:45.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1518</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:45.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:45.0pt" valign="bottom" width="359"><p class="MsoNormal">Cannot view an item from the Item Cart after running a Custom 
  Search if it was not a result of the Custom Search</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:45.0pt" valign="bottom" width="123"><p class="MsoNormal">SmartFind</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:45.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1511</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal">SmartFind: Loading values for Attribute filter causes internal 
  server error. (search API issue)</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">SmartFind</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1355</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">DataReader discipline</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">SmartFind</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1333</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">SmartFind Service Broker and DB Movement</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">SmartFind</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1226</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">List-filter has performance issues when very large.</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">SmartFind</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1213</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal">Fix the Search Criteria Grid so it does not create large gap to 
  right</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">SmartFind</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1193</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal">Cannot sort a category with a Numeric attr set as General 
  (Search API issue?)</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">SmartFind</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">244</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Docs for 3 New Operators in SmartFind Attribute Filters </p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">SmartFind</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Doc</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">157</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Display "does not apply" attribute values</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">SmartFind</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">168</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Allow "*" as wildcard</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">SmartFind</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">201</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Ability to edit search text in advanced search</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">SmartFind</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1670</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">SF Export from within Search Results</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">SmartFind</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">145</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Custom search issue</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">SmartFind</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Support</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1605</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Uom Editor vs SmartFind </p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">UOM Editor</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1601</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Unit type changes don't really save</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">UOM Editor</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1678</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">User Manager Issue</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">User Manager</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">152</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Unable to Re-Classify an Item</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">WebDFR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">253</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Item Classification Help does not work</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">WebDFR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1719</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">WebDFR Edit Item 'Item does not exits'</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">WebDFR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1717</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">WebDFR Help Link</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">WebDFR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1681</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">232</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Items not in terminal categories</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">WebDFR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1680</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">230</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Item Classification internal error</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">WebDFR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1671</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">162</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Read only relationship attributes can be edited</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">WebDFR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1661</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal">Ensure that incorrect filtered category paths are being logged</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">WebDFR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1655</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal">Adding items to more than one collection in a single edit 
  creates load issue</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">WebDFR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1654</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Creating an item from a clone with relationships</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">WebDFR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1650</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Filtered Categories don't handle bad paths</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">WebDFR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1649</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">WebDFR Installation Issue</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">WebDFR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1611</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">New Build Script Issue with WebDFR</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">WebDFR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1558</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Descriptions using '#' get truncated</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">WebDFR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1533</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Cannot use a webDFR created clone (vs. SF created clone)</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">WebDFR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">1476</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal">Item Type Code comparison shouldn’t be case sensitive for clones</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">WebDFR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">158</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="359"><p class="MsoNormal">Provide ability to flag an attribute value as "does not 
  apply" for an item</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">WebDFR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">190</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Category attachments exposed on attribute entry screen  </p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">WebDFR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">224</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Expose category attachments on attribute entry page</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">WebDFR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:15.0pt"><td style="width:44.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="60"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:56.45pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="75"><p align="right" class="MsoNormal" style="text-align:right">250</p></td><td style="width:269.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="359"><p class="MsoNormal">Request allowed value</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="123"><p class="MsoNormal">WebDFR</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:15.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr></table>

 




