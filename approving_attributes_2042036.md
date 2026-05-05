



Approving\_Attributes - Design For Retrieval (DFR) Help




**System 
Attributes - Hiding and Setting Aliases**


 


 


There is a set of properties in 
Classifiication Manager which not only drives the aliasing of system attributes 
but also whether or not they appear in SmartFind.  This is set by category and 
this option is only available to a user with the Category Administrator role.


 


**Setting up Aliases:**


1.    Right click on the 
category and select Update Category making sure Browse is not checked


 


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/CM-SystemAttr92013_files/image001.jpg)

.


 


2.    
Select 
the Properties tab.  This lists the system attributes as well as a few other 
properties.  You will see the system attribute properties with the word Alias 
after it.  Whatever you type in the value value field for that alias, will 
display in SmartFind, DFR and WebDFR for that attribute.  Inheritance will take 
this setting to the bottom leaf category so any alias you set should inherit 
down.  


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/CM-SystemAttr92013_files/image002.jpg)




 


3.    In SmartFind, the 
result will appear as this, Item Description (Part Description).  The alias 
will just display as is in Classification Manager.    


4.    Release Date has been 
added as a system attribute.  This attribute stores the date the item 
information was finalized and released which also defines the date it became 
the next revision.  It acts as the other system attributes.  This can be 
aliased by typing in a name into the Value field.  Removing the <EMPTY> 
value will remove the attribute from display hence removing it from use.  


 


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/CM-SystemAttr92013_files/image003.jpg)




**Hiding System Attributes:**


System attributes can now be hidden in 
SmartFind to allow for more screen space.  The attributes will still however be 
included in the export.  This setting used to hide it only from DFR’s Data 
Developer and Classification Manager.  


1.    If the user would 
like to hide any system attribute from display in SmartFind, this is done in 
the Properties window as well.  Again, right click on the category and select 
Update Category.  


2.    You will see either 
<empty> in the Value field or a typed in Alias.  If the Value field 
contains <empty>, the attribute has no special properties set on it.  If 
there is a value typed in, that is the ‘Alias’ value set.  


3.    To make the system 
attribute hide from Data Developer, Classification Manager and SmartFind, simply 
delete the <EMPTY> value from the Value column and save.  


4.    When adding attribute 
filters to SmartFind, do not select the system attribute that you have hidden.  
It will be available in the list.  If you select it, it will display.  If it is 
not on the list, it will be hidden from view.


 


 


  
  



 


Return 
to [Classification Manager](CM-Overview.md) 


 




