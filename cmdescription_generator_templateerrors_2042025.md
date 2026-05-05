



CMDescription\_Generator\_TemplateErrors - Design For Retrieval (DFR) Help




**Description Generator – Find and Fix Template Errors**



To find and fix templates which contain errors, select the Description 
Template Validator action on the Category Processing tab within Classification 
Manger.   The validate button will parse all templates for errors.  All 
templates found in error will be listed and allow the user to fix the errors.  
The validation process runs validations for the currently selected category and 
all subcategories.  The table below shows what is validated in templates during 
the validation process.


 




<table border="1" cellpadding="0" cellspacing="0" class="MsoTableGrid" style="border-collapse:collapse;border:none"><tr style="height:12.15pt"><td style="width:152.75pt;border:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.15pt" valign="top" width="204"><p align="center" class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt; 
  text-align:center;line-height:normal"><b>Error</b></p></td><td style="width:297.4pt;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt;height:12.15pt" valign="top" width="397"><p align="center" class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt; 
  text-align:center;line-height:normal"><b>Description</b></p></td></tr><tr style="height:35.85pt"><td style="width:152.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:35.85pt" valign="top" width="204"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Invalid Attribute Name</p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal"> </p></td><td style="width:297.4pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:35.85pt" valign="top" width="397"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Name changes to attributes will invalidate templates which use the 
  attribute.</p></td></tr><tr style="height:48.0pt"><td style="width:152.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:48.0pt" valign="top" width="204"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Invalid Category Attribute</p></td><td style="width:297.4pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:48.0pt" valign="top" width="397"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Removing attribute from a category invalidates templates on the 
  category which use the attribute.</p></td></tr><tr style="height:48.7pt"><td style="width:152.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:48.7pt" valign="top" width="204"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Invalid UOM</p></td><td style="width:297.4pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:48.7pt" valign="top" width="397"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">UOM type changes invalidates templates which specify a UOM from the 
  old UOM type for the attribute.</p></td></tr><tr style="height:59.55pt"><td style="width:152.75pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:59.55pt" valign="top" width="204"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Invalid Data Type of Attribute</p></td><td style="width:297.4pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:59.55pt" valign="top" width="397"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Attribute data type changes invalidates templates if the template 
  uses a UOM or decimal place precision and the new data type is not numeric.</p></td></tr></table>

 


 


**Fixing template errors:**


After a validation is run, any templates with errors will be 
listed in the grid below the Validate button.


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/CM-Description_Generator_TemplateErrors_files/image001.jpg)




To inspect and fix a template in error, select the template 
within the grid.  Below the grid, the template will be displayed with the 
error(s) highlighted in Red.  As each error 
is navigated to, the current error is shown in ***Bold*** and the description of the error is displayed below 
the template.


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/CM-Description_Generator_TemplateErrors_files/image002.jpg)




 


Use the navigation actions to move from error to error and 
to fix errors.  As each error is navigated properties of the token in error is 
displayed in the Properties section.  Using the action controls an attribute 
can be fixed or removed.  To fix an error click the fix button, this will 
enable the properties editor allowing changes to the currently selected token.    
To remove a token in error, click the remove button when the desired token is 
selected.


 


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/CM-Description_Generator_TemplateErrors_files/image003.png)




 


When the properties section is in edit mode, the attribute 
can be changed.  Based on the attribute type, other parameters can also be 
changed on the token.  Once editing is completed click Save to save the updated 
token.


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/CM-Description_Generator_TemplateErrors_files/image004.jpg)




 


 


Return to [Using the Description Generator](CM-Using%20Description%20GeneratorMenu.md) 


 


 




