



Approving\_Attributes - Design For Retrieval (DFR) Help




**Relationship 
Attributes**


 


**Items Data Type**


Relationship attributes define a one to many relationship or many 
values associated with it.  An example of this would be the Part to Documents 
relationship attribute would display many documents for each part.  The Part to 
Document would be defined as a relationship attribute.  



Relationship attributes should have the Type Items.  This flags 
the attribute as a relationship attribute.  Create an attribute as described 
above.  However, input Type = Items.  Length defaults to 4 and UOM Type 
defaults to general.  


 


Assign the relationship attribute to the desired category.  Once 
this is done, items can be added in either WebDFR or DFR.  If additional 
attributes need to be defined, define a group.


 


**File Data Type**


File data type attributes define a one to many relationship 
or many values associated with it.  An example of this would be anything the 
user names the file data type relationship.  The individual files are stored as 
DFR Items with an Item Number.  This Item Number will include a URL attribute 
link to the document location.  This file data type is treated similar to the 
data type Items.  



**Define a group**


To define attributes about a relationship, 
the attribute group and the attribute properties functions are used in the 
Attribute Manager.


 


While in Attribute Manager, select the Groups tab in the Default 
section.  Click on the Define Group button.  Enter the name of the desired 
group and a description.  The dates will be filled in automatically.  If the 
group already exists, then the attributes can just be added to the group.  


 


**Assign the group to the Relationship Attribute**


Select the relationship attribute. Edit and select the Properties 
tab.  Type in to the RelAttribGroup in the Value column the name of the desired 
group.  The name has to match exactly.  Save.


 


**Assign attributes to the group**


Edit the attribute to assign it to the desired group.  If the 
attribute is Approved or Pending, right click to Rework.  On the Groups tab, 
select the dropdown button and choose which group to add to the attribute.  An 
attribute can be in multiple groups.  Once you have selected a group, click the 
add button.  Save the attribute.  To delete a group from the attribute, select 
the remove button and save.  


 


When this is complete, you will see all attributes in the group 
when you add an item to the relationship.  


 


**Item Images**


Item Images is a Items relationship type.  When adding images to a 
category, the user does not necessarily need to add a group to define 
attributes.  Images are added via WebDFR as Items to the Attachments category.  
This category includes all attributes such as the URL attributes defining the 
physical location of the image.  


 


When adding an image to the Item Image relationship, the user can 
add 1 or more images.  


  
  



 


Return to [Attribute 
Manager](hs2000.md)




