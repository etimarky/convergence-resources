



Release\_Notes - Design For Retrieval (DFR) Help




## Summary of New Features:


- Data Developer (filtering/views) 
 – new filter boxes to support column filtering, including unique values 
 for sorting, setting allowed values, configure display order and hide 
 columns from the grid, and saving these new display configurations as 
 views that can be shared.  Data 
 Developer (Item Browser Features) – creating working batches, setting 
 assignment, reclassifying and changing item status from Data Developer.
- Data Developer (viewing links 
 via relationships) - Provide URL attachment viewing supporting complex 
 item relationships.  DNA – does not 
 apply can be set by attribute value field.
- Classification Manager – configure 
 the default attribute display order for Data Developer.
- User Manager – 2 new roles – 
 Item Approver to allow specific users to approve items and Vendor that 
 restricts data access in DFR.
- Attribute Manager – global 
 property to set read only attributes
- User Reports – now show % 
 complete
- DFR Help File – covers new 
 enhancements and all modules including User Manager, Item Clusters, Unit 
 of Measure Editor, Release Notes, and Options Manager
- Allowed Values Manager – 
 allowing editing of values across categories

## Module Specific Release Notes 
Data Developer:


- Provided the ability to 
 reduce records display with individual filter boxes per attribute.  Users can filter for an exact value, a 
 range, greater than, less than or similar too using wild cards.
- Unique values are displayed 
 for each column of data that can be used in a filter supporting all 
 attribute types including numeric, string, integer, etc.
- Allowed values can be set 
 from the data developer if the user has the allowed values role.
- Views can be save for a 
 category in the structure that will include any attribute filters applied, 
 sorting, hidden attributes and column and row formatting.  Views can be shared or not shared when 
 they are saved.
- Individual rows can now be 
 exported from data developer versus the entire grid.  The exported file will include column 
 formatting, attribute sequence and hidden columns.
- URLs can be viewed on an item 
 or through a collection of related items from the Data Developer.  E.g. Part to Document then Document to 
 Attachment.  Information on each 
 item in a collection, including descriptions and item numbers, can also be 
 viewed.
- Better copy and paste 
 capabilities including right click copy and paste of a single item and 
 drag copy for a column of data.
- Better find and replace 
 supporting numeric values and nulls.
- Ability to set a required 
 attribute value to DNA – does not apply.  
 Values with this setting allow nulls for required fields, bypassing 
 validations.

 




## Allowed Values Manager:


·         
Users can now edit allowed unique values across 
categories at a parent category level.  
The allowed values manager will now expose all of the string attributes 
at and below a parent category, regardless if they are shared by all the 
children categories.  Only the global 
allowed value list can be edited while not working at a terminal node level, 
the local allowed values list will be grayed out.  
  



## Classification Manager:


·         
The attribute display order will control the 
default order of attributes in the Data Developer.  The display order will serve as the global 
default display order in Data Developer for all users.


·         
Offer group selection of attributes to make it 
easier and more efficient to reconfigure the display order.


·         
Setting DNA – does not apply for category 
attributes by check the box, similar to setting required category attributes.


 




 




## User  
Manager:


- Created 
 2 new roles including Item Approver and Vendor.  The Item Approver allows non-catalog 
 admin to approve items, providing more flexibility.  The Vendor role restricts users to only 
 see the data assigned to them in Data Developer; these users can not 
 access other DFR module


## Bugs Fixed and Enhancements in this Release:


 






<table border="1" cellpadding="0" cellspacing="0" class="MsoTableGrid" style="width:6.2in;border-collapse:collapse;border:none;mso-border-alt:solid windowtext .5pt; 
 mso-yfti-tbllook:480;mso-padding-alt:0in 5.4pt 0in 5.4pt;mso-border-insideh: 
 .5pt solid windowtext;mso-border-insidev:.5pt solid windowtext" width="595"><tr style="mso-yfti-irow:0;mso-yfti-firstrow:yes"><td style="width:23.3pt;border:solid windowtext 1.0pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="31"><p align="center" class="MsoNormal" style="text-align:center"><b style="mso-bidi-font-weight:normal">#<p></p></b></p></td><td style="width:252.1pt;border:solid windowtext 1.0pt; 
  border-left:none;mso-border-left-alt:solid windowtext .5pt;mso-border-alt: 
  solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="336"><p align="center" class="MsoNormal" style="text-align:center"><b style="mso-bidi-font-weight:normal">Description<p></p></b></p></td><td style="width:45.0pt;border:solid windowtext 1.0pt; 
  border-left:none;mso-border-left-alt:solid windowtext .5pt;mso-border-alt: 
  solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="60"><p align="center" class="MsoNormal" style="text-align:center"><b style="mso-bidi-font-weight:normal">Module<p></p></b></p></td><td style="width:1.75in;border:solid windowtext 1.0pt; 
  border-left:none;mso-border-left-alt:solid windowtext .5pt;mso-border-alt: 
  solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="168"><p align="center" class="MsoNormal" style="text-align:center"><b style="mso-bidi-font-weight:normal">CDS/IHS <p></p></b></p>
<p align="center" class="MsoNormal" style="text-align:center"><b style="mso-bidi-font-weight:normal">Tracking #<p></p></b></p></td></tr><tr style="mso-yfti-irow:1"><td style="width:23.3pt;border:solid windowtext 1.0pt; 
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="31"><p class="MsoNormal">1</p></td><td style="width:252.1pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="336"><p class="MsoNormal">Column Filtering – offer filters with different operators, 
  present a list of unique values to filter against, setting allowed values.</p></td><td style="width:45.0pt;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="60"><p align="center" class="MsoNormal" style="text-align:center">DD</p></td><td style="width:1.75in;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="168"><p align="center" class="MsoNormal" style="text-align:center">Enh</p>
<p align="center" class="MsoNormal" style="text-align:center">CDS#1189</p></td></tr><tr style="mso-yfti-irow:2"><td style="width:23.3pt;border:solid windowtext 1.0pt; 
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="31"><p class="MsoNormal">2</p></td><td style="width:252.1pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="336"><p class="MsoNormal">Attribute Display Order – configure default attribute display 
  order for DD from CM.</p></td><td style="width:45.0pt;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="60"><p align="center" class="MsoNormal" style="text-align:center">CM</p></td><td style="width:1.75in;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="168"><p align="center" class="MsoNormal" style="text-align:center">Enh</p></td></tr><tr style="mso-yfti-irow:3"><td style="width:23.3pt;border:solid windowtext 1.0pt; 
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="31"><p class="MsoNormal">3</p></td><td style="width:252.1pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="336"><p class="MsoNormal">Views – save any filters, moved or hidden columns, 
  formatting, etc in a view that can be shared or not shared.</p></td><td style="width:45.0pt;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="60"><p align="center" class="MsoNormal" style="text-align:center">DD</p></td><td style="width:1.75in;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="168"><p align="center" class="MsoNormal" style="text-align:center">Enh</p></td></tr><tr style="mso-yfti-irow:4"><td style="width:23.3pt;border:solid windowtext 1.0pt; 
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="31"><p class="MsoNormal">4</p></td><td style="width:252.1pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="336"><p class="MsoNormal">Column Display Management – configure columns by selecting 
  and dragging or hiding right from the DD grid.</p></td><td style="width:45.0pt;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="60"><p align="center" class="MsoNormal" style="text-align:center">DD</p></td><td style="width:1.75in;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="168"><p align="center" class="MsoNormal" style="text-align:center">Enh</p>
<p align="center" class="MsoNormal" style="text-align:center">CDS#1188</p></td></tr><tr style="mso-yfti-irow:5"><td style="width:23.3pt;border:solid windowtext 1.0pt; 
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="31"><p class="MsoNormal">5</p></td><td style="width:252.1pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="336"><p class="MsoNormal">Exporting Options – export selected rows in a grid while 
  maintaining hidden columns and column order.</p></td><td style="width:45.0pt;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="60"><p align="center" class="MsoNormal" style="text-align:center">DD</p></td><td style="width:1.75in;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="168"><p align="center" class="MsoNormal" style="text-align:center">Enh</p></td></tr><tr style="mso-yfti-irow:6"><td style="width:23.3pt;border:solid windowtext 1.0pt; 
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="31"><p class="MsoNormal">6</p></td><td style="width:252.1pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="336"><p class="MsoNormal">Viewing Attachments URL Links – view the list of URL 
  references via an Item Collection or series of Item Collections.</p></td><td style="width:45.0pt;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="60"><p align="center" class="MsoNormal" style="text-align:center">DD</p></td><td style="width:1.75in;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="168"><p align="center" class="MsoNormal" style="text-align:center">Enh</p></td></tr><tr style="mso-yfti-irow:7"><td style="width:23.3pt;border:solid windowtext 1.0pt; 
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="31"><p class="MsoNormal">7</p></td><td style="width:252.1pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="336"><p class="MsoNormal">Right Click Copy Paste – copy a single item and paste 
  multiple places</p></td><td style="width:45.0pt;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="60"><p align="center" class="MsoNormal" style="text-align:center">DD</p></td><td style="width:1.75in;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="168"><p align="center" class="MsoNormal" style="text-align:center">CDS#951/IHS#46</p></td></tr><tr style="mso-yfti-irow:8"><td style="width:23.3pt;border:solid windowtext 1.0pt; 
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="31"><p class="MsoNormal">8</p></td><td style="width:252.1pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="336"><p class="MsoNormal">Find and replace better handling of numeric data including 
  nulls</p></td><td style="width:45.0pt;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="60"><p align="center" class="MsoNormal" style="text-align:center">DD</p></td><td style="width:1.75in;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="168"><p align="center" class="MsoNormal" style="text-align:center">CDS#882/IHS#54</p></td></tr><tr style="mso-yfti-irow:9"><td style="width:23.3pt;border:solid windowtext 1.0pt; 
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="31"><p class="MsoNormal">9</p></td><td style="width:252.1pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="336"><p class="MsoNormal">Offer drag copy by selecting a single cell and using 
  control key to drag copy</p></td><td style="width:45.0pt;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="60"><p align="center" class="MsoNormal" style="text-align:center">DD</p></td><td style="width:1.75in;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="168"><p align="center" class="MsoNormal" style="text-align:center">Enh</p></td></tr><tr style="mso-yfti-irow:10"><td style="width:23.3pt;border:solid windowtext 1.0pt; 
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="31"><p class="MsoNormal">10</p></td><td style="width:252.1pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="336"><p class="MsoNormal">Create working batches, change item status and set 
  assignment in DD.</p></td><td style="width:45.0pt;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="60"><p align="center" class="MsoNormal" style="text-align:center">DD</p></td><td style="width:1.75in;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="168"><p align="center" class="MsoNormal" style="text-align:center">Enh-CDS#804/IHS#66</p></td></tr><tr style="mso-yfti-irow:11"><td style="width:23.3pt;border:solid windowtext 1.0pt; 
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="31"><p class="MsoNormal">11</p></td><td style="width:252.1pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="336"><p class="MsoNormal">Run validations from Data Developer</p></td><td style="width:45.0pt;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="60"><p align="center" class="MsoNormal" style="text-align:center">DD</p></td><td style="width:1.75in;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="168"><p align="center" class="MsoNormal" style="text-align:center">Enh-CDS#1186/IHS#67</p></td></tr><tr style="mso-yfti-irow:12"><td style="width:23.3pt;border:solid windowtext 1.0pt; 
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="31"><p class="MsoNormal">12</p></td><td style="width:252.1pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="336"><p class="MsoNormal">Group selecting and sizing of rows and columns</p></td><td style="width:45.0pt;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="60"><p align="center" class="MsoNormal" style="text-align:center">DD</p></td><td style="width:1.75in;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="168"><p align="center" class="MsoNormal" style="text-align:center">CDS#1147/IHS#68</p></td></tr><tr style="mso-yfti-irow:13"><td style="width:23.3pt;border:solid windowtext 1.0pt; 
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="31"><p class="MsoNormal">13</p></td><td style="width:252.1pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="336"><p class="MsoNormal">Set read-only attributes from the Attribute Manager</p></td><td style="width:45.0pt;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="60"><p align="center" class="MsoNormal" style="text-align:center">AM</p></td><td style="width:1.75in;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="168"><p align="center" class="MsoNormal" style="text-align:center">CDS#1187/IHS#69</p></td></tr><tr style="mso-yfti-irow:14"><td style="width:23.3pt;border:solid windowtext 1.0pt; 
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="31"><p class="MsoNormal">14</p></td><td style="width:252.1pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="336"><p class="MsoNormal">Vendor role – new role where the user can only see their 
  data to work on in Data Developer.</p></td><td style="width:45.0pt;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="60"><p align="center" class="MsoNormal" style="text-align:center">UM</p></td><td style="width:1.75in;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="168"><p align="center" class="MsoNormal" style="text-align:center">Enh</p></td></tr><tr style='mso-yfti-irow:15;mso-prop-change:"Richard W\. Turner" 20060905T1012'><td style="width:23.3pt;border:solid windowtext 1.0pt; 
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt;border:solid windowtext 1.0pt !msorm;border-top: 
  none !msorm;mso-border-top-alt:solid windowtext .5pt !msorm;mso-border-alt: 
  solid windowtext .5pt !msorm;padding:0in 5.4pt 0in 5.4pt !msorm" valign="top" width="31"><p class="MsoNormal">15</p></td><td style="width:252.1pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt;border-top: 
  none !msorm;border-left:none !msorm;border-bottom:solid windowtext 1.0pt !msorm; 
  border-right:solid windowtext 1.0pt !msorm;mso-border-top-alt:solid windowtext .5pt !msorm; 
  mso-border-left-alt:solid windowtext .5pt !msorm;mso-border-alt:solid windowtext .5pt !msorm; 
  padding:0in 5.4pt 0in 5.4pt !msorm" valign="top" width="336"><p class="MsoNormal">Item Approver – new role that allows non-catalog admin to 
  approve items</p></td><td style="width:45.0pt;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt;border-top: 
  none !msorm;border-left:none !msorm;border-bottom:solid windowtext 1.0pt !msorm; 
  border-right:solid windowtext 1.0pt !msorm;mso-border-top-alt:solid windowtext .5pt !msorm; 
  mso-border-left-alt:solid windowtext .5pt !msorm;mso-border-alt:solid windowtext .5pt !msorm; 
  padding:0in 5.4pt 0in 5.4pt !msorm" valign="top" width="60"><p align="center" class="MsoNormal" style="text-align:center">UM</p></td><td style="width:1.75in;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt;border-top: 
  none !msorm;border-left:none !msorm;border-bottom:solid windowtext 1.0pt !msorm; 
  border-right:solid windowtext 1.0pt !msorm;mso-border-top-alt:solid windowtext .5pt !msorm; 
  mso-border-left-alt:solid windowtext .5pt !msorm;mso-border-alt:solid windowtext .5pt !msorm; 
  padding:0in 5.4pt 0in 5.4pt !msorm" valign="top" width="168"><p align="center" class="MsoNormal" style='text-align:center;mso-prop-change: 
  "Richard W\. Turner" 20060905T1013'>Enh</p></td></tr><tr style='mso-yfti-irow:16;mso-prop-change:"Richard W\. Turner" 20060905T1012'><td style="width:23.3pt;border:solid windowtext 1.0pt; 
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt;border:solid windowtext 1.0pt !msorm;border-top: 
  none !msorm;mso-border-top-alt:solid windowtext .5pt !msorm;mso-border-alt: 
  solid windowtext .5pt !msorm;padding:0in 5.4pt 0in 5.4pt !msorm" valign="top" width="31"><p class="MsoNormal">16</p></td><td style="width:252.1pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt;border-top: 
  none !msorm;border-left:none !msorm;border-bottom:solid windowtext 1.0pt !msorm; 
  border-right:solid windowtext 1.0pt !msorm;mso-border-top-alt:solid windowtext .5pt !msorm; 
  mso-border-left-alt:solid windowtext .5pt !msorm;mso-border-alt:solid windowtext .5pt !msorm; 
  padding:0in 5.4pt 0in 5.4pt !msorm" valign="top" width="336"><p class="MsoNormal">Copy-paste limitation of 70 excel to DD</p></td><td style="width:45.0pt;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt;border-top: 
  none !msorm;border-left:none !msorm;border-bottom:solid windowtext 1.0pt !msorm; 
  border-right:solid windowtext 1.0pt !msorm;mso-border-top-alt:solid windowtext .5pt !msorm; 
  mso-border-left-alt:solid windowtext .5pt !msorm;mso-border-alt:solid windowtext .5pt !msorm; 
  padding:0in 5.4pt 0in 5.4pt !msorm" valign="top" width="60"><p align="center" class="MsoNormal" style="text-align:center">DD</p></td><td style="width:1.75in;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt;border-top: 
  none !msorm;border-left:none !msorm;border-bottom:solid windowtext 1.0pt !msorm; 
  border-right:solid windowtext 1.0pt !msorm;mso-border-top-alt:solid windowtext .5pt !msorm; 
  mso-border-left-alt:solid windowtext .5pt !msorm;mso-border-alt:solid windowtext .5pt !msorm; 
  padding:0in 5.4pt 0in 5.4pt !msorm" valign="top" width="168"><p align="center" class="MsoNormal" style='text-align:center;mso-prop-change: 
  "Richard W\. Turner" 20060905T1013'>CDS#1164</p></td></tr><tr style='mso-yfti-irow:17;mso-prop-change:"Richard W\. Turner" 20060905T1012'><td style="width:23.3pt;border:solid windowtext 1.0pt; 
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt;border:solid windowtext 1.0pt !msorm;border-top: 
  none !msorm;mso-border-top-alt:solid windowtext .5pt !msorm;mso-border-alt: 
  solid windowtext .5pt !msorm;padding:0in 5.4pt 0in 5.4pt !msorm" valign="top" width="31"><p class="MsoNormal">17</p></td><td style="width:252.1pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt;border-top: 
  none !msorm;border-left:none !msorm;border-bottom:solid windowtext 1.0pt !msorm; 
  border-right:solid windowtext 1.0pt !msorm;mso-border-top-alt:solid windowtext .5pt !msorm; 
  mso-border-left-alt:solid windowtext .5pt !msorm;mso-border-alt:solid windowtext .5pt !msorm; 
  padding:0in 5.4pt 0in 5.4pt !msorm" valign="top" width="336"><p class="MsoNormal">Update reports to show % complete</p></td><td style="width:45.0pt;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt;border-top: 
  none !msorm;border-left:none !msorm;border-bottom:solid windowtext 1.0pt !msorm; 
  border-right:solid windowtext 1.0pt !msorm;mso-border-top-alt:solid windowtext .5pt !msorm; 
  mso-border-left-alt:solid windowtext .5pt !msorm;mso-border-alt:solid windowtext .5pt !msorm; 
  padding:0in 5.4pt 0in 5.4pt !msorm" valign="top" width="60"><p align="center" class="MsoNormal" style="text-align:center">RPTs</p></td><td style="width:1.75in;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt;border-top: 
  none !msorm;border-left:none !msorm;border-bottom:solid windowtext 1.0pt !msorm; 
  border-right:solid windowtext 1.0pt !msorm;mso-border-top-alt:solid windowtext .5pt !msorm; 
  mso-border-left-alt:solid windowtext .5pt !msorm;mso-border-alt:solid windowtext .5pt !msorm; 
  padding:0in 5.4pt 0in 5.4pt !msorm" valign="top" width="168"><p align="center" class="MsoNormal" style='text-align:center;mso-prop-change: 
  "Richard W\. Turner" 20060905T1013'>CDS#1088</p></td></tr><tr style='mso-yfti-irow:18;mso-prop-change:"Richard W\. Turner" 20060905T1012'><td style="width:23.3pt;border:solid windowtext 1.0pt; 
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt;border:solid windowtext 1.0pt !msorm;border-top: 
  none !msorm;mso-border-top-alt:solid windowtext .5pt !msorm;mso-border-alt: 
  solid windowtext .5pt !msorm;padding:0in 5.4pt 0in 5.4pt !msorm" valign="top" width="31"><p class="MsoNormal">18</p></td><td style="width:252.1pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt;border-top: 
  none !msorm;border-left:none !msorm;border-bottom:solid windowtext 1.0pt !msorm; 
  border-right:solid windowtext 1.0pt !msorm;mso-border-top-alt:solid windowtext .5pt !msorm; 
  mso-border-left-alt:solid windowtext .5pt !msorm;mso-border-alt:solid windowtext .5pt !msorm; 
  padding:0in 5.4pt 0in 5.4pt !msorm" valign="top" width="336"><p class="MsoNormal">Item relationship limitation of 178 new relationships</p></td><td style="width:45.0pt;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt;border-top: 
  none !msorm;border-left:none !msorm;border-bottom:solid windowtext 1.0pt !msorm; 
  border-right:solid windowtext 1.0pt !msorm;mso-border-top-alt:solid windowtext .5pt !msorm; 
  mso-border-left-alt:solid windowtext .5pt !msorm;mso-border-alt:solid windowtext .5pt !msorm; 
  padding:0in 5.4pt 0in 5.4pt !msorm" valign="top" width="60"><p align="center" class="MsoNormal" style="text-align:center">IL</p></td><td style="width:1.75in;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt;border-top: 
  none !msorm;border-left:none !msorm;border-bottom:solid windowtext 1.0pt !msorm; 
  border-right:solid windowtext 1.0pt !msorm;mso-border-top-alt:solid windowtext .5pt !msorm; 
  mso-border-left-alt:solid windowtext .5pt !msorm;mso-border-alt:solid windowtext .5pt !msorm; 
  padding:0in 5.4pt 0in 5.4pt !msorm" valign="top" width="168"><p align="center" class="MsoNormal" style='text-align:center;mso-prop-change: 
  "Richard W\. Turner" 20060905T1013'>CDS#1245/WHL#127</p></td></tr><tr style='mso-yfti-irow:19;mso-prop-change:"Richard W\. Turner" 20060905T1012'><td style="width:23.3pt;border:solid windowtext 1.0pt; 
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt;border:solid windowtext 1.0pt !msorm;border-top: 
  none !msorm;mso-border-top-alt:solid windowtext .5pt !msorm;mso-border-alt: 
  solid windowtext .5pt !msorm;padding:0in 5.4pt 0in 5.4pt !msorm" valign="top" width="31"><p class="MsoNormal">19</p></td><td style="width:252.1pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt;border-top: 
  none !msorm;border-left:none !msorm;border-bottom:solid windowtext 1.0pt !msorm; 
  border-right:solid windowtext 1.0pt !msorm;mso-border-top-alt:solid windowtext .5pt !msorm; 
  mso-border-left-alt:solid windowtext .5pt !msorm;mso-border-alt:solid windowtext .5pt !msorm; 
  padding:0in 5.4pt 0in 5.4pt !msorm" valign="top" width="336"><p class="MsoNormal">Category attachment URL now showing up in attachments tab</p></td><td style="width:45.0pt;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt;border-top: 
  none !msorm;border-left:none !msorm;border-bottom:solid windowtext 1.0pt !msorm; 
  border-right:solid windowtext 1.0pt !msorm;mso-border-top-alt:solid windowtext .5pt !msorm; 
  mso-border-left-alt:solid windowtext .5pt !msorm;mso-border-alt:solid windowtext .5pt !msorm; 
  padding:0in 5.4pt 0in 5.4pt !msorm" valign="top" width="60"><p align="center" class="MsoNormal" style="text-align:center">CM</p></td><td style="width:1.75in;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt;border-top: 
  none !msorm;border-left:none !msorm;border-bottom:solid windowtext 1.0pt !msorm; 
  border-right:solid windowtext 1.0pt !msorm;mso-border-top-alt:solid windowtext .5pt !msorm; 
  mso-border-left-alt:solid windowtext .5pt !msorm;mso-border-alt:solid windowtext .5pt !msorm; 
  padding:0in 5.4pt 0in 5.4pt !msorm" valign="top" width="168"><p align="center" class="MsoNormal" style='text-align:center;mso-prop-change: 
  "Richard W\. Turner" 20060905T1013'>CDS#1382/WHL#134</p></td></tr><tr style='mso-yfti-irow:20;mso-prop-change:"Richard W\. Turner" 20060905T1012'><td style="width:23.3pt;border:solid windowtext 1.0pt; 
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt;border:solid windowtext 1.0pt !msorm;border-top: 
  none !msorm;mso-border-top-alt:solid windowtext .5pt !msorm;mso-border-alt: 
  solid windowtext .5pt !msorm;padding:0in 5.4pt 0in 5.4pt !msorm" valign="top" width="31"><p class="MsoNormal">20</p></td><td style="width:252.1pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt;border-top: 
  none !msorm;border-left:none !msorm;border-bottom:solid windowtext 1.0pt !msorm; 
  border-right:solid windowtext 1.0pt !msorm;mso-border-top-alt:solid windowtext .5pt !msorm; 
  mso-border-left-alt:solid windowtext .5pt !msorm;mso-border-alt:solid windowtext .5pt !msorm; 
  padding:0in 5.4pt 0in 5.4pt !msorm" valign="top" width="336"><p class="MsoNormal">Cant create new UOM types and assigned new UOM’s or move 
  UOM’s to another UOM type</p></td><td style="width:45.0pt;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt;border-top: 
  none !msorm;border-left:none !msorm;border-bottom:solid windowtext 1.0pt !msorm; 
  border-right:solid windowtext 1.0pt !msorm;mso-border-top-alt:solid windowtext .5pt !msorm; 
  mso-border-left-alt:solid windowtext .5pt !msorm;mso-border-alt:solid windowtext .5pt !msorm; 
  padding:0in 5.4pt 0in 5.4pt !msorm" valign="top" width="60"><p align="center" class="MsoNormal" style="text-align:center">UOM Editor</p></td><td style="width:1.75in;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt;border-top: 
  none !msorm;border-left:none !msorm;border-bottom:solid windowtext 1.0pt !msorm; 
  border-right:solid windowtext 1.0pt !msorm;mso-border-top-alt:solid windowtext .5pt !msorm; 
  mso-border-left-alt:solid windowtext .5pt !msorm;mso-border-alt:solid windowtext .5pt !msorm; 
  padding:0in 5.4pt 0in 5.4pt !msorm" valign="top" width="168"><p align="center" class="MsoNormal" style='text-align:center;mso-prop-change: 
  "Richard W\. Turner" 20060905T1013'>CDS#1452/WHL#140</p></td></tr><tr style='mso-yfti-irow:21;mso-yfti-lastrow:yes;mso-prop-change:"Richard W\. Turner" 20060905T1012'><td style="width:23.3pt;border:solid windowtext 1.0pt; 
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt;border:solid windowtext 1.0pt !msorm;border-top: 
  none !msorm;mso-border-top-alt:solid windowtext .5pt !msorm;mso-border-alt: 
  solid windowtext .5pt !msorm;padding:0in 5.4pt 0in 5.4pt !msorm" valign="top" width="31"><p class="MsoNormal">21</p></td><td style="width:252.1pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt;border-top: 
  none !msorm;border-left:none !msorm;border-bottom:solid windowtext 1.0pt !msorm; 
  border-right:solid windowtext 1.0pt !msorm;mso-border-top-alt:solid windowtext .5pt !msorm; 
  mso-border-left-alt:solid windowtext .5pt !msorm;mso-border-alt:solid windowtext .5pt !msorm; 
  padding:0in 5.4pt 0in 5.4pt !msorm" valign="top" width="336"><p class="MsoNormal">Default UOM not being stored correctly</p></td><td style="width:45.0pt;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt;border-top: 
  none !msorm;border-left:none !msorm;border-bottom:solid windowtext 1.0pt !msorm; 
  border-right:solid windowtext 1.0pt !msorm;mso-border-top-alt:solid windowtext .5pt !msorm; 
  mso-border-left-alt:solid windowtext .5pt !msorm;mso-border-alt:solid windowtext .5pt !msorm; 
  padding:0in 5.4pt 0in 5.4pt !msorm" valign="top" width="60"><p align="center" class="MsoNormal" style="text-align:center">UOM Editor</p></td><td style="width:1.75in;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt;border-top: 
  none !msorm;border-left:none !msorm;border-bottom:solid windowtext 1.0pt !msorm; 
  border-right:solid windowtext 1.0pt !msorm;mso-border-top-alt:solid windowtext .5pt !msorm; 
  mso-border-left-alt:solid windowtext .5pt !msorm;mso-border-alt:solid windowtext .5pt !msorm; 
  padding:0in 5.4pt 0in 5.4pt !msorm" valign="top" width="168"><p align="center" class="MsoNormal" style='text-align:center;mso-prop-change: 
  "Richard W\. Turner" 20060905T1013'>CDS#1453/WHL#77</p></td></tr></table>

 






