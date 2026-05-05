



Approving\_Attributes - Design For Retrieval (DFR) Help




**Adding Images to an Item**


There 
is a new relationship attribute called Item Images that supports displaying 
single or multiple images for an item in the Item Details page in SmartFind.  
Users will be able to customize these images by selecting the location (on the 
summary page or by default the Images Tab) and customizing the size of each 
image.  Property settings are managed by DFR.


 


**Steps 
to adding images:**



1.     Using **WebDFR**, 
create an item /attachment remembering to change the qualifier to attachment.  
Classify image to Non-Parts\Attachments category.  The Attachments category has 
the appropriate attributes associated to it to define the location of the 
Image.  Enter the URL for the image and save.  The URL attribute should exist 
in the Attachments category.


2.     In **DFR**, open 
Attribute Manager.  Check to see if the attribute ‘Item Images’ exists.  It 
should be included with the Master Attribute list.  If not, create the relationship 
attribute Item Images setting the Type to Items, default Length to 4 and the UOM 
Type to General.  (see Attribute Manager help file)  Go to Classification 
Manager and right click the category which you will be adding the attribute.  
Select Edit Attributes and select Item Images.  Click the Assign To Category 
button.  This assigns this attribute to the designated category.    


3.     Once this is set in **DFR**, 
go back in to **WebDFR** and look up the item number to assign the images.  
On the Edit page, go to the bottom of the page where the Relationship 
Attributes section resides.  Load the attachment images to the Item Images 
collection.  


4.     In **DFR,** view and 
edit the new display properties by category to view and size the image.


 


\*NOTE:  Image files can only be Bitmap, JPEGs, 
PNGs and GIF files.  This feature does not support pdf files.  The image URLs 
need to point to images supported by the HTML “<IMG>” tag.  


The user will need to use DFR and WebDFR to set 
up images.   


Once 
steps 1 through 3 are complete, the user will need to edit the new display 
properties in Classification Manager.  Go to the category where the part resides that 
is associated with the image(s).  Select the category and then select Item 
Images attribute.  Right click and select Edit….


 


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/CM-Add_Images_files/image001.jpg)




Select the properties 
tab and set the Summary Attribute to True.  If the Summary attribute is set to 
True, the image will appear in the summary area.  If set to False or left blank, 
the image will be displayed on the Images tab.  The user can then size the 
image by entering a size in the ViewImageSize value.  This will control the 
size of the image on the Item Details page.  


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/CM-Add_Images_files/image002.jpg)




Adding multiple Image Items would 
display multiple images in SmartFind.  When the user mouses over an image, it 
would display the image larger.  


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/CM-Add_Images_files/image003.jpg)

 


By clicking on the image opens it 
up in a new window even larger.  All images will appear on the Relationship tab 
under the Images Relationship.


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/CM-Add_Images_files/image004.jpg)




 


Return to [Classification Manager](CM-Overview.md) 


 




