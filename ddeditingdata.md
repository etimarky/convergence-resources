



DDEditingData - Design For Retrieval (DFR) Help




**Editing 
Data**



The 
Data Developer module allows the user to edit item data in the spreadsheet 
format. Some fields are set to read-only and cannot be edited.  These 
fields include Master Item data such as Item Number, Legacy Item Number and 
Item Description.  Custom fields are also read only such as Ranges.  
These read the columns that the Ranges are set to in Classification 
Manager.  Item data types cannot be edited as they represent relationships 
as well as Detail Count.  All other fields that are shaded in blue can be 
edited.


 


**Only 
items assigned to the current user may be modified.**  (Items assigned 
to the current user logged in will be displayed in black.  Items not 
assigned to the current user will display in grey.)  


 


**General 
Editing**


To 
modify data, select the cell and press F2 to start typing or double click in 
the cell to replace the data. Modified data will appear in green.  This 
indicates that the field has been edited but not yet saved.  Press Return 
or select another cell to edit.


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DD-Editing-Data_files/image001.jpg)




Example: 
modified data appears in green.


 


**Hint**: A user can only 
modify items which are assigned to them.


 


After 
modifying data, you can commit your changes by selecting the “Save to DB” 
button.  The edited field is now shaded in blue indicating that the new 
value has been saved in the database.


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DD-Editing-Data_files/image002.jpg)




 


 


**Copy 
and Paste**


Use 
the Right click button to Copy…..


**![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DD-Editing-Data_files/image003.jpg)**



Use 
your right click button to Paste…


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DD-Editing-Data_files/image004.jpg)




 



**Change 
Multiple Fields to the Same Value**


To 
change multiple fields to the same value, double click…


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DD-Editing-Data_files/image005.jpg)




 


Select 
the **Alt key and drag** your cursor down the column.  This will paste 
that same value into multiple fields in the column.  The value will be 
copied to the selected items and they will be shaded green indicating that they 
have not been saved.  


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DD-Editing-Data_files/image006.jpg)




 


 


**Using 
Find and Replace**


To 
**Find** a value select Edit and Find (or press Ctrl+F), or to **Replace** 
one value with another, elect Edit and Replace (or press Ctrl+H). Enter 
the value to Find and the replacement value; select what to Search, Current 
Column, Entire Sheet, or Selected Area; then either click Replace or Replace 
All.  


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DD-Editing-Data_files/image007.jpg)




 


Clicking 
the Find: button will replace the Find what value with the value displayed on 
the button (352 in the example above).


 


By 
default, Find and Replace does a case insensitive contains search. For example, 
if you search for “motor”, the results will include “motor”, “Electric motors”, 
and “Motors and Engines”. 


 


If 
you select Exact Match and search for “motor”, results will include “motor” and 
“Motor”, but not “Electric motors” or “Motors and Engines”.


 


If 
you select Match Case and search for “motor”, results will include “motor”, and 
“Electric motors”, but not “Motors and Engines”.


 


Replace 
is only available if the currently selected cell is not read only.


 


If 
the currently selected cell has an Allowed Values List, the Replace With field 
will include a drop down list of Allowed Values for that cell. If Restrict To 
Allowed Values is selected, then the Replace With field is restricted to the 
Allowed Values for that cell.


 


**Viewing 
Additional Decimal Places**


Data 
Developer defaults on 2 decimal places for an attribute value for the first 
time.  To see the additional decimal places for an attribute value, select 
the attribute value by just clicking on any cell in the column.  Select 
the Format drop down menu from the top menu bar.  Select Decimal places 
> # of decimal places to be viewed.  The screen will repaint with the 
additional decimal place values for the entire column.  


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DD-Editing-Data_files/image008.jpg)




 


 


Return 
to [Data 
Developer](hs4000.md)


 




