



Approving\_Attributes - Design For Retrieval (DFR) Help




**Range 
Validation**


 


 


Users can set Range Validations for number 
datatypes.  This would include Numerics, Decimals and Integers.  This would 
prevent users from entering data out of range in Data Developer and WebDFR.  


 


Right Click on the attribute to set up the 
range validation.  The Attribute Editor will display.  On the Settings tab, 
click on Range Validation enabling both the Lower limit and Upper limit 
fields.  Set the limits to the desired values.  If the only values that should 
be entered is 3 to 5 feet, enter in 3 for the Lower limit and 10 for the Upper 
limit.  Make sure to select a Unit of Measure from the dropdown.  Click Save.


 


 


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/CM-RangeValidationUOM_files/image001.jpg)




 


When entering data on this field, Data 
Developer will provide an error during Validation.  WebDFR will not allow an update 
if the data in the field does not fall within the Upper and Lower limits.  When 
entering data, the user can enter data in a different UOM than the field 
validation is configured.   Both DFR and WebDFR will look for the default UOM 
and do a conversion prior to saving to the database.  For example, Diameter 
(Inner) is set to 3-5 feet, the user can enter 24 inches in WebDFR as long as 
the UOM equals 3-5 feet.  The validation looks at the base UOM when doing the 
conversion.  


 


 


 


 


Return 
to [Classification Manager](CM-Overview.md) 




