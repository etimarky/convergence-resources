



New\_Features - Design For Retrieval (DFR) Help




## Summary of New Features:


- Item 
 Loader – Added support for item number generation.
- Item 
 Loader – Added ability to import across categories.
- Item 
 Mapping – Improved smooth scrolling.  Ability to enter variant year 
 data from a grid for all variant years in a row and for all variants 
 assigned to a module.  Offers copy and paste across cells, shading to 
 show edits etc, in the grid.  Update a roadmap to show a view of all 
 data using a grid which is editable by users.
- User 
 Manager – Added 1 role – Super User role.  This allows anyone with 
 this privilege to modify the Base Year mapping data.
- Data 
 Developer – Combined Item Browser into Data Developer.  All features 
 from Item Browser and Data Developer are now available in one module.
- Data 
 Developer – Implemented regionalization within Data Developer for display, 
 validation and data entry of the decimal and digit grouping characters.
- Data 
 Developer – More exporting capabilities
- Classification 
 Manager – Configure Custom Tabs to display in SmartFind
- Classification 
 Manager – Added ability to add Images
- Classification 
 Manager – Added 2 roles independent of User Manager to edit/administer by 
 category.
- All 
 - ODP.net support using .net 4.0 has significantly improved performance 
 and demonstrated the ability to handle processing for a 40 million item 
 database.

## 


## DFR Module Specific Release Notes 
Item Loader:


Item 
Loader now enables auto item number generation.  Go to the Options Manager and look for 
the value used for option -  ItemLoadAutoGenText.  Here is where the value 
would be set.  It can be set to #, $, \* or whatever character is preferred.  
The load file must then have the correct corresponding value in the item number 
field for auto item number generation to work.  In the example below the value 
is “#”.  Also notice the qualifier set to work with this value is Auto.  It 
does not have to be Auto, this is just an example.


 


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DFR_V3.6.896a_Release_Notes_2011_files/image001.jpg)




**Example of a load file formatted for 
auto-item number generation – see highlighted fields**


 


Make 
sure to select the correct root qualifier when loading a file that requires 
auto-generation of item numbers.


 


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DFR_V3.6.896a_Release_Notes_2011_files/image002.jpg)




**Item Loader Import dialog box**


 


A 
user must remember to have the correct qualifier and root qualifier, as well as 
value for the auto generation of item number to work properly.  If you are not 
sure, contact your DFR administrator.


 


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DFR_V3.6.896a_Release_Notes_2011_files/image003.jpg)

   


**Note the value for the item number - <Auto 
Number> in the preview screen**


 


Guidelines on auto item number 
generation:


 


1.)   Configure 
this with help from your DFR Admin


2.)   Select a 
value to use as item number that will trigger auto item number generation, this 
value needs to be setup in the Options Manager


3.)   Remember 
to use the correct root qualifier and qualifier with each auto item number 
generation for both Item Loader and WebDFR.


4.)   This 
feature can support different items e.g. documents, parts, organizations, that 
can all have their own sequence of auto generated item numbers


5.)   Auto 
generated item numbers can have specific formats e.g. prefixes, suffixes, etc.  
Contact your DFR admin to setup.


6.)   It is ok 
if auto generated item numbers do not all get used in sequence, since users can 
delete parts or cancel creating a new part in WebDFR.


7.)   Auto 
generated numbers are tied to qualifiers.  Different qualifiers can use 
the same auto generated number sequence or they can have their own.  Item 
numbers generated for specific qualifiers will share the same number sequence 
no matter where they are generated from; WebDFR or through Item Loader.


8.)   WebDFR 
and DFR Item Loader all work off of the latest item number that is how they 
stay in sync.  It’s not possible for WebDFR and DFR Item Loader to try to use 
the same auto-generated item number, so you don’t need to worry about 
collisions.


## Item Loader:


## Through Item Loader, the user can import across categories.  
The attributes must exist in all categories.  Prepare the cdr loader file.  Map 
everything except for category path.


## Item Mapping:


Item 
Mapping now has the ability to enter variant year data from a grid for all 
variant years in a row and for all variants assigned to a module.  Like 
Data Developer, it offers copy and paste across cells, shading to show edits 
etc, in the grid.  Users can now update a roadmap to show a view of all 
data using a grid which is editable by users.  


## User Manager:


One 
role was added to the User manager for Item Mapping called Super User 
role.  This allows anyone with this privilege to modify the Base Year 
mapping data. 


 


**Read 
Only Data for Base Year**


The 
Item Mapping tool does not allow normal users to edit variant year data for the 
base year by setting certain fields to read only.  A user will notice a 
gray background that says “Read-only data” in the baseline column, as shown 
below.  Certain right click menu fields have been grayed out for the read 
only data to protect it from any editing.


 


![Description: Capture.JPG](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DFR_V3.6.896a_Release_Notes_2011_files/image004.jpg)




**Example 
of read only data for the base year 2009**


 


**Super 
User Role**


A 
user with the *Super User* role is able to make changes to the base year, 
as well as any other variant year regardless of its owner group.


 


 


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DFR_V3.6.896a_Release_Notes_2011_files/image005.jpg)




 **Example of read/write data for the base year 
2009**


 


## Data Developer:


Combined 
Item Browser into Data Developer.  All features from Item Browser and Data 
Developer are now available in one module.


 


**Relationship 
Editing**


Relationships 
can now be edited a cell at a time on the same screen simply by double clicking 
on the relationship attribute.


 


To 
populate the lower grid with Relationship data, double click the cell that 
contains the Relationship data you wish to retrieve.


 


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DFR_V3.6.896a_Release_Notes_2011_files/image006.jpg)




**Example: 
To display the 8 items indicated in the “Link Part to Document” attribute, 
double click.**


 


Once 
the user double clicks this cell, the detail grid will be populated.


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DFR_V3.6.896a_Release_Notes_2011_files/image007.jpg)




**Example: 
Detail grid populated with the 8 items from the previous example.**


 


*Note*: 
You can use the arrow keys to populate the grid with the details for other 
rows. For example, with the <count=8> row selected, pressing the down 
arrow will retrieve the detail info for the next row.


## Data Developer:


## Implemented regionalization within Data Developer for 
display, validation and data entry of the decimal and digit grouping characters.  The user can 
set the region and DFR will display according to what region and settings are 
set in Region and Language.  No digit grouping symbols are ever saved to the 
database and a decimal is always saved to the database for the Decimal symbol.  
Whatever is set in Region and Language settings is what is displayed to the 
user.


 


Go 
to Control Panel Region and Language.  Set the region to where you are working 
on the Format tab.  (i.e. Brazil would be Portuguese (Brazil)).


 


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DFR_V3.6.896a_Release_Notes_2011_files/image008.jpg)




**Example:  
Region and Language Tab**



Click 
on the Additional Settings… button to set the Decimal symbol and Digit grouping 
symbol specifically.  You must set both settings on the Numbers tab and 
Currency tab.


 


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DFR_V3.6.896a_Release_Notes_2011_files/image009.jpg)




**Example:  
Numbers tab**



**![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DFR_V3.6.896a_Release_Notes_2011_files/image010.jpg)**


**Example:  
Currency tab**



 


 


## Data Developer:


## Implemented more exporting capabilities.  Excel and text 
export options exist along with pick list and attribute item options.  These 
can all be found in the Report menu options.


 


## Data Developer:


## Ability to create and save views.  Users can create public or 
private views for their workflows by show/hiding columns and using filters.  
These can be saved and viewed by just that user or by everyone.  Use filters by 
the right click menu to set the criteria.


 


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DFR_V3.6.896a_Release_Notes_2011_files/image011.jpg)




**Right 
click menu to set filters**



Use 
the Show/Hide Columns… to finish your view.  



![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DFR_V3.6.896a_Release_Notes_2011_files/image012.jpg)




**View 
> Show/Hide Columns…**



Once 
you have the view you want, click on the Views button.  ![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DFR_V3.6.896a_Release_Notes_2011_files/image013.jpg)




 


Use 
the View Manager to set it to Public or Private and save it as a name.  Your 
view can only be saved and used to a specific category.  Use this View Manager 
to load the view by using the Load View button.  


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DFR_V3.6.896a_Release_Notes_2011_files/image014.jpg)




**View 
Manager Dialog**


## Classification Manager:


**Adding Images**


There is a new collection attribute called 
Item Images that supports displaying single or multiple images for an item in 
the Item Details page in SmartFind.  Users will be able to customize these 
images by selecting the location (on the summary page or by default the Images 
Tab) and customizing the size of each image.  Property settings are managed by 
DFR.   


**Steps to adding images:**


1.     Using **WebDFR**, 
create an item /attachment remembering to change the qualifier to attachment.  
Classify image to Non-Parts\Attachments category.  Enter the URL for the image 
and save.


2.     In **DFR**, create 
the collection attribute Item Images and add to the category you will be 
assigning your part.  


3.     Once this is set in **DFR**, 
go back in to **WebDFR** and look up the item number to assign the images.  
On the Edit page, go to the bottom of the page where there Relationship 
Attributes section resides.  Load the attachment images to the Item Images 
collection.  


4.     In **DFR,** view 
and edit the new display properties by category to view and size the image.


\*NOTE:  Image files can only be Bitmap, 
JPEGs, PNGs and GIF files.  This feature does not support pdf files.  The image 
URLs need to point to images supported by the HTML “<IMG>” tag.  


The user will need to use DFR and WebDFR to 
set up images.   


Once 
steps 1 through 3 are complete, the user will need to edit the new display 
properties in Classification Manager.  Go to the category where the part resides 
that is associated with the image(s).  Select the category and then select Item 
Images attribute.  Verify that browse mode is unchecked.  Right click and 
select Edit….


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DFR_V3.6.896a_Release_Notes_2011_files/image015.jpg)




Select 
the properties tab and set the Summary Attribute to True.  If the Summary 
attribute is set to True, the image will appear in the summary area.  If set to 
False or left blank, the image will be displayed on the Images tab.  The user 
can then size the image by entering a size in the ViewImageSize value.  This 
will control the size of the image on the Item Details page.  


 


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DFR_V3.6.896a_Release_Notes_2011_files/image016.jpg)




**Example:  Properties to set Item Images**


  
  



**Configure 
Custom Tags to get a tab to display**


SmartFind provides the feature of Custom Tabs.  Custom Tabs enable 
the user to create tabs and define different types of functionality.  Many 
configurations of custom tabs are done in DFR Configuration Manager. 


  


Once in Classification Manager, select the category from the 
Category Tree.  You will see the list of attributes on the Attributes Tab.  
Uncheck the Browse box.  Right click the attribute and select Edit.  It will 
bring you to the Attribute Editor.  (see below)


 


 


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DFR_V3.6.896a_Release_Notes_2011_files/image017.jpg)




**Attribute 
Editor:  Set properties on the properties tab**


 


. 



- ViewImageSize -  Set this to the size of 
 an image display.  i.e. 200x200
- Display Tab – The exact name of the 
 custom tab the attribute will appear on.  i.e. Input is in the SmartFind config 
 file as the customName of the tab.
- Summary Attribute – Set to True, the 
 attribute will display in the summary section.  If set to false or left 
 blank, the attribute will be left on the item details tab.


## Classification Manager:


**Adding Roles**


There 
are 2 more roles added by category that can be seen in the Responsible User’s 
tab in Classification Manager.  These are Category Developer and Category 
Approver.  Select a category.


 


**![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DFR_V3.6.896a_Release_Notes_2011_files/image018.jpg)**


**Action 
> Assign Role**



**![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DFR_V3.6.896a_Release_Notes_2011_files/image019.jpg)**


**Assign 
Category Roles dialog box**



Select 
Category Developer or Category Approver from the dropdown.  Then check off the 
user’s name.  Click Apply and then Ok.  This user’s name will appear on the 
Responsible User’s tab in Classification Manager and will be given that 
privilege only for that category.  




## All:


CDS 
toolset uses ODP.net to improve performance of DFR with the new ODP.net 
provider.  Searching and scrolling in Data Developer are improved areas of 
performance.  Item Mapping performance will improve significantly with ODP.net 
turned on.  CDS is currently working with a production database that is 
successfully handling 40 million items.  


 


Bugs Fixed and Enhancements in this Release:


 




<table border="0" cellpadding="0" cellspacing="0" class="MsoNormalTable" style="width:509.0pt;margin-left:4.65pt;border-collapse:collapse" width="679"><thead><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   background:#D9D9D9;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><b><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>CDS#</span></b></p></td><td style="width:60.55pt;border:solid windowtext 1.0pt; 
   border-left:none;background:#D9D9D9;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><b><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>Customer#</span></b></p></td><td style="width:265.45pt;border:solid windowtext 1.0pt; 
   border-left:none;background:#D9D9D9;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><b><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Issue Title</span></b></p></td><td nowrap="nowrap" style="width:92.0pt;border:solid windowtext 1.0pt; 
   border-left:none;background:#D9D9D9;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><b><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Application Module</span></b></p></td><td nowrap="nowrap" style="width:46.55pt;border:solid windowtext 1.0pt; 
   border-left:none;background:#D9D9D9;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><b><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Type</span></b></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>B-2607</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-471</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Filter dropdown is not displaying decimals</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>B-2611</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Filter issue gives object instance bug inconsistently</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>B-2628</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Validation is flagging multival issues that shouldn’t be 
   flagged</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Validator</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>B-2629</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-473</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Stack trace error displays when click show category path button 
   in Views</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>B-2621</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-476</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Item Mapping throwing a null</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Item Mapping</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>B-2568/ 
   2606</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Cannot add attachments in CM</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Classification Manager/Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>B-2529/ 
   2529</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Cannot add items to a newly created working batch </span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>B-2520/ 
   2556</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>After entering a Portuguese numeric value – when returning to 
   the cell to edit the , disappears</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>B-2524/ 
   2560</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>After deleting cell with value – entering new value in cell – 
   after saving to DB cell is blank</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>B-2552/ 
   2588</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Category Attachments won’t attach to non terminal category</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>B-2553</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Category Attachments have to be assigned to you to assign</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2520</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Obsolete records showing up with Sandbox mode off</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2500</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-432</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Line invisible and should be showing</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2531</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Slowness when searching</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2530</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Slowness when assigning</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2495</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-429</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Retrieving Items from a category</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2501</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-427</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Excel export does not show the "DNA" values in 
   cells </span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2481</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-426</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Can’t assign items</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2496</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-424</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Developer assign item to user</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>All</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-381</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Exporting – description problem</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>All</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-425</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Module Summary Report Error</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Item Mapping</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2496</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-428</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Search in Data Developer</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1945</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-314</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Able to Delete Item(s) with Sand Box Mode Off, regardless of 
   state. </span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Item Browser/ Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2383</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-407</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>MultiVal Attribute Values Can Be Updated in Browse Mode </span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2539</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-435</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Stack Trace Error upon attempting to view the Validation 
   Report </span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2539</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-436</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Stack Trace Error upon attempting to view the Validation Report 
   within Worklog-Dev </span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-126</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Provide protected batches with associated role</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>All</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Enh</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1815</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-228</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Regional Data Entry Issue</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2415</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Relationship item load file had problems loading files</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Item Loader</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2416</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>DFR crash due to unhandled exception</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2417</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-406</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Add “Delete Confirmation” pop up after “Delete Item is selected 
   in DD</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Enh</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2414</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>UOM Editor not showing up</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>All</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2434</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Lower half of right click menu gone</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-415</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Attributes not inheriting down hierarchy structure</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Classification Manager</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2386</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-329</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Retrieve button not retrieving on 1<sup>st</sup> click</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2230</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-360</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Variant and year column don’t align </span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Item Mapping</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2324, 
   2271, 2272</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-388</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>WebDFR accepts the MM/DD/YYYY format</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>All</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2352</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-408</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Module Summary report error</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Item Mapping</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2324, 
   2271, 2272</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-377</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Date validation accepts MM/DD/YYYY format</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Validator</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2301</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-401</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>System.Data version error</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>User Manager</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2288</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-398</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Attributes will not pass validation with &lt;DNA&gt; or without 
   a pick list / AVM Use list is grayed out for No List</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Validator / Allowed Values Manager</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2273</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>WP-365</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>WL - DNA does not pass Non-Null Validation in DD &amp; DV</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2351</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Added index for item stats calls.</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Database</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2380</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Duplicate Collection Entries report broken</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2377</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Cannot create a new template</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Item Loader</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2358</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Trying to Remove Batch causes Application Error</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Remove Batch</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2372</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Using Find/Replace causing Application Error.</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Allowed Values Manager</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2370</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Admin cannot save changes to user account settings</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>User Manager</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2357</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Sorting columns causes search results to go blank</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2355</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Clicking View Report after validation causes application error</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Validator</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2371</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Cannot add item to relationship with count = 0 until a cell 
   with count&gt;0 is clicked</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2364</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Edit attribute causes users to get kicked off in CM</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Classification Manager</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2290</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Sandbox Mode OFF - Delete actually deletes (should obsolete)</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Options Manager</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2289</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Obsolete' not status option for Admin User</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Item Browser</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2260</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Application Error after delete value, then click another cell</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2263</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Loader seems to require full path</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Item Loader</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2255</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Not Retrieving Data (SQL)</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Data Developer</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2246</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Road map save error</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Item Mapping</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>1871</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Attribute status does not show change</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Attribute Manager</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2250</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Edit Attributes not adding attributes</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Classification Manager</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2248</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Apply filter button not working</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Attribute Manager</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>2247</span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'>N/A</span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Can't change update category</span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Classification Manager</span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'>Bug</span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'> </span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'> </span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'> </span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'> </span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'> </span></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'> </span></p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif";color:black'> </span></p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'> </span></p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'> </span></p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><span style='font-size:11.0pt;font-family:"Calibri","sans-serif"; 
   color:black'> </span></p></td></tr></thead></table>

 




