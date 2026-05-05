



Editing\_the\_Data - Design For Retrieval (DFR) Help




**Does 
Not Apply**


 


 


Users can set Does Not Apply for each 
category attribute, as a category property, in the Classification Manager.  
Once this is set for a particular category attribute, users have the ability to 
identify which items in this category do not require values for an attribute in 
the Data Developer, even if the attribute maybe required for that category.  See 
the Classification Manager help file for more information on enabling Does Not 
Apply.


**Using 
Does Not Apply in Data Developer:**


To 
use Does Not Apply, once it has been enabled in Classification Manager, you must 
have items assigned in Data Developer for that category.  From Data Developer, 
a user can right click on an attribute field and select **Set Does Not Apply - 
Set**.  Only attributes that have Does Not Apply enabled in Classification Manager 
will offer this option.  The user will need to save this change just like an 
attribute value change, in order for this setting to work.  When Does Not Apply 
has been set, the user should see <DNA> in the attribute value field.  
Attributes that are shaded in brown have DNA enabled.  Only attributes that are 
required can have DNA enabled.


Looking 
at the data in Data Developer, you will see the <DNA> in the fields as 
place holders as shown below.  Right clicking on the field gives you the option 
to clear the Does Not Apply value in which the field would be empty yet 
displayed in green.  Right clicking again gives you the option to add the Does 
Not Apply value.  


A 
user can not copy and paste the <DNA> value or drag copy the <DNA> 
value.  If a user wants to set <DNA> for multiple fields, highlight the 
fields first, then you can right click to set <DNA> for the highlighted 
fields.  You also can not filter on DNA using the filtering capabilities of 
Data Developer.


If 
a user exports DNA data to excel, the <DNA> symbol will show up in the 
export file.


To 
remove Does Not Apply for an attribute field you right click and select **Does 
Not Apply – Clear**.


## To preview the data result in Data Developer, set batch to 
the name of the file you just imported.  Retrieve the records that were imported, 
select the rows and assign all rows to you.  Right click on the attribute to 
get the Does Not Apply – Clear or Does Not Apply – Add option.  (See below)


 


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DD-Does-Not-Apply_files/image001.jpg)




## Right click to get 
the Does Not Apply – Clear or Does Not Apply – Add option


When 
running validations, required attribute fields that are blank with Does Not 
Apply set, will not create a validation error.


When 
loading data from the Item Loader (via Import Mode), if your load file has 
values in a field that has Does Not Apply Set, it will automatically reset that 
field or clear the Does Not Apply.  


 


 


Return 
to [Data Developer](hs4000.md)


 


 


 




