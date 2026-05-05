



DDEditingCustomAttributes - Design For Retrieval (DFR) Help




**Editing 
Custom Attributes**


 


 


An attribute can have special properties to achieve certain 
functions.  This section describes some examples of DFR’s custom attributes and 
how to create, edit and use them in Data Developer.


 


 


**Vectors**


 


A vector attribute can be edited in Data Developer.  When you 
click on a vector attribute in Data Developer to edit, the user is presented 
attribute fields for each attribute in the vector as columns.  If you right 
click on a column, a user can change the Unit of Measure for individual numeric 
attributes.  The rows of data combined represent a vector that a user can enter 
values against.


 


You can only filter Vectors, you cannot sort them, and all sorting 
options will be grayed out.  If you select Filter, you will be presented with a 
custom dialog that will allow the user to filter on different vector values.  
As the user enters values for the filter, a contextual explanation of the 
filter will appear in the bottom of the dialog box.  This explanation will help 
guide the user to select only valid filter values.


 


Users can use both copy and paste and drag copy (using the Alt 
key) on vector values, it works just like the normal attribute values.  The 
find and replace function only has find enabled, users will not be able to use 
the replace, that feature has been disabled.


  
  



**Ranges**


 


Range attributes are read only in Data Developer.  They will only 
display the minimum and maximum value in a range along with the units of 
measure.  If a user changes either a minimum and/or maximum attribute value, 
the range attribute will automatically update to reflect this change.


 


You can filter ranges but you cannot sort ranges, sorting options 
will be grayed out.  When you pull up the filter dialog, you will notice the 
only operation choice is Test.  A user can only enter a test value for 
filtering, if that value fits in an existing range, it will bring back those 
ranges in the filter result.  For example, if the user enters 50 Deg C (for 
temperature range attribute) it will display all of the ranges that 50 Deg C 
would fit inside e.g. 0 to 100 Deg C.


 


Copy and paste and drag copy have been disabled for ranges.  A 
user can still access these operations on the fields used to create the range.  
(E.g. max temperature or min temperature)  Find and replace has also been 
disabled on range values, as with copy and paste, these can still be done on 
the fields used to create the range.  (E.g. max temperature or min 
temperature)  


 


 


**MultiVal  (Multi-Value Attributes)**


 


MultiVal attributes can have multiple attribute values for a 
single field in Data Developer.  A user first has to create an allowed values 
list using the allowed values manager that contains all the possible 
multi-values.  When you click on a MultiVal attribute in Data Developer, a menu 
will appear allowing a user to select any or all of the possible values for the 
MultiVal attribute.  Once the values are selected they will appear in the 
single attribute field in Data Developer separated by vertical lines e.g. 
4:value1|value2|value3|value4.  You will also notice the total number of values 
appears first in the field followed by the individual values.


 


Since MultiVal works off of the allowed values list, any new 
values can be added to the MultiVal list by right clicking in Data Developer 
and selecting Add allowed value.  Only users with allowed values rights can do 
this on the fly.


 


You can filter on MultiVal attributes but you cannot sort them, 
all sorting options have been grayed out.  The filter uses the Like operator.  
A user has the option of sorting on an existing value using the drop down list 
or they can filter on just an individual value in a set of values e.g. steel.  
The user must remember to use the wild card value % around filter values to 
obtain the filter result they desire.  For example, enter %steel% and the user 
will see items with multi-values like carbon steel, cold rolled steel, etc.  If 
they just enter steel, they will not get see these values in the filter result.


 


A user can copy and paste MultiVal attribute values from one field 
to another field (s) as long as it’s in the same column of data.  User can also 
drag copy MultiVal attributes, using the alt key on your keyboard, to populate 
multiple fields below or above a selected MultiVal value.


 


Users can use find and replace on MultiVal attributes just like 
normal attribute values.


 


Users can validate MultiVal attributes just like allowed values 
validation.  The validation should find any MultiVal attribute values that are 
not on the allowed values list.


 


 


Return 
to [Data Developer](hs4000.md)


 




