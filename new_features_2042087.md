



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


 


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/DFR_V3.6.896a_Release_Notes_2011_files/image001.jpg)




**Example of a load file formatted for 
auto-item number generation – see highlighted fields**


 


Make 
sure to select the correct root qualifier when loading a file that requires 
auto-generation of item numbers.


 


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/DFR_V3.6.896a_Release_Notes_2011_files/image002.jpg)




**Item Loader Import dialog box**


 


A 
user must remember to have the correct qualifier and root qualifier, as well as 
value for the auto generation of item number to work properly.  If you are not 
sure, contact your DFR administrator.


 


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/DFR_V3.6.896a_Release_Notes_2011_files/image003.jpg)

   


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


 


![Description: Capture.JPG](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/DFR_V3.6.896a_Release_Notes_2011_files/image004.jpg)




**Example 
of read only data for the base year 2009**


 


**Super 
User Role**


A 
user with the *Super User* role is able to make changes to the base year, 
as well as any other variant year regardless of its owner group.


 


 


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/DFR_V3.6.896a_Release_Notes_2011_files/image005.jpg)




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


 


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/DFR_V3.6.896a_Release_Notes_2011_files/image006.jpg)




**Example: 
To display the 8 items indicated in the “Link Part to Document” attribute, 
double click.**


 


Once 
the user double clicks this cell, the detail grid will be populated.


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/DFR_V3.6.896a_Release_Notes_2011_files/image007.jpg)




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


 


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/DFR_V3.6.896a_Release_Notes_2011_files/image008.jpg)




**Example:  
Region and Language Tab**



Click 
on the Additional Settings… button to set the Decimal symbol and Digit grouping 
symbol specifically.  You must set both settings on the Numbers tab and 
Currency tab.


 


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/DFR_V3.6.896a_Release_Notes_2011_files/image009.jpg)




**Example:  
Numbers tab**



**![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/DFR_V3.6.896a_Release_Notes_2011_files/image010.jpg)**


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


 


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/DFR_V3.6.896a_Release_Notes_2011_files/image011.jpg)




**Right 
click menu to set filters**



Use 
the Show/Hide Columns… to finish your view.  



![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/DFR_V3.6.896a_Release_Notes_2011_files/image012.jpg)




**View 
> Show/Hide Columns…**



Once 
you have the view you want, click on the Views button.  ![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/DFR_V3.6.896a_Release_Notes_2011_files/image013.jpg)




 


Use 
the View Manager to set it to Public or Private and save it as a name.  Your 
view can only be saved and used to a specific category.  Use this View Manager 
to load the view by using the Load View button.  


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/DFR_V3.6.896a_Release_Notes_2011_files/image014.jpg)




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


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/DFR_V3.6.896a_Release_Notes_2011_files/image015.jpg)




Select 
the properties tab and set the Summary Attribute to True.  If the Summary 
attribute is set to True, the image will appear in the summary area.  If set to 
False or left blank, the image will be displayed on the Images tab.  The user 
can then size the image by entering a size in the ViewImageSize value.  This 
will control the size of the image on the Item Details page.  


 


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/DFR_V3.6.896a_Release_Notes_2011_files/image016.jpg)




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


 


 


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/DFR_V3.6.896a_Release_Notes_2011_files/image017.jpg)




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


 


**![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/DFR_V3.6.896a_Release_Notes_2011_files/image018.jpg)**


**Action 
> Assign Role**



**![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/DFR_V3.6.896a_Release_Notes_2011_files/image019.jpg)**


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
   background:#D9D9D9;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"><b>CDS#</b></p></td><td style="width:60.55pt;border:solid windowtext 1.0pt; 
   border-left:none;background:#D9D9D9;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"><b>Customer#</b></p></td><td style="width:265.45pt;border:solid windowtext 1.0pt; 
   border-left:none;background:#D9D9D9;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"><b>Issue Title</b></p></td><td nowrap="nowrap" style="width:92.0pt;border:solid windowtext 1.0pt; 
   border-left:none;background:#D9D9D9;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"><b>Application Module</b></p></td><td nowrap="nowrap" style="width:46.55pt;border:solid windowtext 1.0pt; 
   border-left:none;background:#D9D9D9;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"><b>Type</b></p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">B-2607</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-471</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Filter dropdown is not displaying decimals</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">B-2611</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">N/A</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Filter issue gives object instance bug inconsistently</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">B-2628</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">N/A</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Validation is flagging multival issues that shouldn’t be 
   flagged</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Validator</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">B-2629</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-473</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Stack trace error displays when click show category path button 
   in Views</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">B-2621</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-476</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Item Mapping throwing a null</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Mapping</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">B-2568/ 
   2606</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">N/A</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Cannot add attachments in CM</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Classification Manager/Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">B-2529/ 
   2529</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">N/A</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Cannot add items to a newly created working batch </p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">B-2520/ 
   2556</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">N/A</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">After entering a Portuguese numeric value – when returning to 
   the cell to edit the , disappears</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">B-2524/ 
   2560</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">N/A</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">After deleting cell with value – entering new value in cell – 
   after saving to DB cell is blank</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">B-2552/ 
   2588</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">N/A</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Category Attachments won’t attach to non terminal category</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">B-2553</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">N/A</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Category Attachments have to be assigned to you to assign</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2520</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">N/A</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Obsolete records showing up with Sandbox mode off</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2500</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-432</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Line invisible and should be showing</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2531</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">N/A</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Slowness when searching</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2530</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">N/A</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Slowness when assigning</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2495</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-429</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Retrieving Items from a category</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2501</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-427</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Excel export does not show the "DNA" values in 
   cells </p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2481</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-426</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Can’t assign items</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2496</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-424</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Data Developer assign item to user</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">All</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-381</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Exporting – description problem</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">All</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-425</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Module Summary Report Error</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Mapping</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2496</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-428</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Search in Data Developer</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">1945</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-314</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Able to Delete Item(s) with Sand Box Mode Off, regardless of 
   state. </p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Browser/ Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2383</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-407</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">MultiVal Attribute Values Can Be Updated in Browse Mode </p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2539</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-435</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Stack Trace Error upon attempting to view the Validation 
   Report </p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2539</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-436</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Stack Trace Error upon attempting to view the Validation Report 
   within Worklog-Dev </p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-126</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Provide protected batches with associated role</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">All</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">1815</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-228</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Regional Data Entry Issue</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2415</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">N/A</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Relationship item load file had problems loading files</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Loader</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2416</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">N/A</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">DFR crash due to unhandled exception</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2417</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-406</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Add “Delete Confirmation” pop up after “Delete Item is selected 
   in DD</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Enh</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2414</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">N/A</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">UOM Editor not showing up</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">All</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2434</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">N/A</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Lower half of right click menu gone</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">N/A</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-415</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Attributes not inheriting down hierarchy structure</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Classification Manager</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2386</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-329</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Retrieve button not retrieving on 1<sup>st</sup> click</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2230</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-360</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Variant and year column don’t align </p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Mapping</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2324, 
   2271, 2272</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-388</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">WebDFR accepts the MM/DD/YYYY format</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">All</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2352</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-408</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Module Summary report error</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Mapping</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2324, 
   2271, 2272</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-377</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Date validation accepts MM/DD/YYYY format</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Validator</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2301</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-401</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">System.Data version error</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">User Manager</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2288</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-398</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Attributes will not pass validation with &lt;DNA&gt; or without 
   a pick list / AVM Use list is grayed out for No List</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Validator / Allowed Values Manager</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2273</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">WP-365</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">WL - DNA does not pass Non-Null Validation in DD &amp; DV</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2351</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">N/A</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Added index for item stats calls.</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Database</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2380</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">N/A</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Duplicate Collection Entries report broken</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2377</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">N/A</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Cannot create a new template</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Loader</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2358</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">N/A</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Trying to Remove Batch causes Application Error</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Remove Batch</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2372</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">N/A</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Using Find/Replace causing Application Error.</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Allowed Values Manager</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2370</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">N/A</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Admin cannot save changes to user account settings</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">User Manager</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2357</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">N/A</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Sorting columns causes search results to go blank</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2355</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">N/A</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Clicking View Report after validation causes application error</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Validator</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2371</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">N/A</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Cannot add item to relationship with count = 0 until a cell 
   with count&gt;0 is clicked</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2364</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">N/A</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Edit attribute causes users to get kicked off in CM</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Classification Manager</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2290</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">N/A</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Sandbox Mode OFF - Delete actually deletes (should obsolete)</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Options Manager</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2289</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">N/A</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Obsolete' not status option for Admin User</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Browser</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2260</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">N/A</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Application Error after delete value, then click another cell</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2263</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">N/A</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Loader seems to require full path</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Loader</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2255</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">N/A</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Not Retrieving Data (SQL)</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Data Developer</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2246</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">N/A</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Road map save error</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Item Mapping</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">1871</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">N/A</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Attribute status does not show change</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Attribute Manager</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2250</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">N/A</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Edit Attributes not adding attributes</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Classification Manager</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2248</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">N/A</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Apply filter button not working</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Attribute Manager</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="right" class="MsoNormal" style="text-align:right">2247</p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center">N/A</p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal">Can't change update category</p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal">Classification Manager</p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal">Bug</p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"> </p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"> </p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"> </p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"> </p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"> </p></td></tr><tr style="height:30.0pt"><td style="width:44.45pt;border:solid windowtext 1.0pt; 
   border-top:none;padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="59"><p align="center" class="MsoNormal" style="text-align:center"> </p></td><td style="width:60.55pt;border-top:none;border-left: 
   none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="81"><p align="center" class="MsoNormal" style="text-align:center"> </p></td><td style="width:265.45pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="354"><p class="MsoNormal"> </p></td><td nowrap="nowrap" style="width:92.0pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="123"><p class="MsoNormal"> </p></td><td nowrap="nowrap" style="width:46.55pt;border-top:none; 
   border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
   padding:0in 5.4pt 0in 5.4pt;height:30.0pt" valign="bottom" width="62"><p class="MsoNormal"> </p></td></tr></thead></table>

 




