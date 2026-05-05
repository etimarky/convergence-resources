



Approving\_Attributes - Design For Retrieval (DFR) Help




**Does Not Apply**


 


All 
attributes are global throughout DFR and SmartFind.  Setting them to Required 
may be a data requirement for some instances.  However, in some modules, this 
“Required” may not apply.  The application allows you to set an instance of it 
to Allow:”Does Not Apply”.  With this setting, the field is not required.  The 
application sets the value to <DNA> as its value.  This acts as a place 
holder in the field.  


 


Users 
can set Does Not Apply for each category attribute, as a category property, in 
the Classification Manager.  Once this is set for a particular category 
attribute, users have the ability to identify which items in this category do 
not require values for an attribute in the Data Developer, even if the 
attribute may be required for that category.  This capability will support the 
case where there maybe a few items in a category where certain attribute does 
not apply.  This property is enabled just like required attributes, with a check 
box that has to be selected from the attribute editor field in Classification 
Manager for a particular attribute.


 


Only category approvers and developers can set 
this property in the Classification Manager.  You can only set DNA for required 
attributes.


 


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/CM-Does_Not_Apply_files/image002.jpg)




**Note the Allow: “Does Not Apply” check box**



**To set “Does Not Apply”:**


·         
Double 
click on a category attribute as a category approver or developer.


·         
From 
the Attribute Editor page, Allow: “Does Not Apply” is an option you will see 
displayed below next to the Required option in the Validation section.  Check 
the Allow: “Does Not Apply” box.  If the attribute is not set to required, 
select that first so you can then enable DNA.


·         
Select 
Save



**Using 
Does Not Apply in Data Developer:**


To 
use Does Not Apply, once it has been enabled in Classification Manager, you 
must have items assigned in data developer for that category.  From Data 
Developer a user can right click on an attribute field and select **Set Does 
Not Apply - Set**.  Only attributes that have Does Not Apply enabled in 
Classification Manager will offer this option.  The user will need to save this 
change, just like an attribute value change, in order for this setting to work.


To 
remove Does Not Apply for an attribute field you right click and select **Does 
Not Apply – Clear**.


When 
running validations, required attribute fields that are blank, with Does Not 
Apply set, will not create a validation error.


When 
loading data from the Item Loader (via Import Mode), if your load file has 
values in a field that has Does Not Apply Set, it will automatically reset that 
field or clear the Does Not Apply.  
  



 


Return 
to [Classification 
Manager](CM-Overview.md) 




