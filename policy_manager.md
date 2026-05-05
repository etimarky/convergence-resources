



Policy\_Manager - Design For Retrieval (DFR) Help




**Policy 
Manager**


 


The 
Policy Manager allows power users to add enforcement criteria, also known as 
policies, to the data model.  The Policy Manager module will only be viewable 
for users with the catalog role, “Policy Manager” enabled.  Within the Policy Manager 
module, policies can be defined, enabled, disabled and validated against the 
current defined data model.


 


**Policies:**


Within 
Policy Manager there are canned policies a user can customize.  The table below 
lists the current policies.


 




<table border="1" cellpadding="0" cellspacing="0" class="MsoTableGrid" style="border-collapse:collapse;border:none"><tr><td style="width:166.25pt;border:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="222"><p align="center" class="MsoNormal" style="text-align:center"><b><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>Policy</span></b></p></td><td style="width:158.55pt;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="211"><p align="center" class="MsoNormal" style="text-align:center"><b><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>Description</span></b></p></td><td style="width:142.7pt;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="190"><p align="center" class="MsoNormal" style="text-align:center"><b><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>Settings</span></b></p></td></tr><tr><td style="width:166.25pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="222"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>Attribute 
  Name Invalid Characters</span></p></td><td style="width:158.55pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="211"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>Policy 
  denies creation of Attribute names which contain any of the specified 
  characters.</span></p></td><td style="width:142.7pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="190"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>A 
  list of invalid characters (Note: characters are not separated)  Example: 
  #$%*&amp;^</span></p></td></tr><tr><td style="width:166.25pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="222"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>Attribute 
  Name Length</span></p></td><td style="width:158.55pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="211"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>Policy 
  allows minimum and maximum restrictions to be placed on Attribute names.</span></p></td><td style="width:142.7pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="190"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>A 
  minimum length and a maximum length.</span></p>
<p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>Default 
  settings are:</span></p>
<p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>Minimum 
  – 2</span></p>
<p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>Maximum 
  - 500</span></p></td></tr><tr><td style="width:166.25pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="222"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>Attribute 
  Description Length</span></p></td><td style="width:158.55pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="211"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>Policy 
  allows minimum and maximum restrictions to be placed on Attribute descriptions</span></p></td><td style="width:142.7pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="190"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>A 
  minimum and maximum length. Default settings are:<br/> 
  Minimum – 2<br/> 
  Maximum – 500 (Note: the maximum length value cannot be more than 500 because 
  that is the maximum allowable by the system.)</span></p></td></tr><tr><td style="width:166.25pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="222"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>Allowed 
  Value Length</span></p></td><td style="width:158.55pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="211"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>Policy 
  allows minimum and maximum restrictions to be placed on allowed values</span></p></td><td style="width:142.7pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="190"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>A 
  minimum and maximum length. Default settings are:<br/> 
  Minimum – 1<br/> 
  Maximum – 200 (Note: the maximum length value cannot be more than 200, 
  because that is the maximum allowable by the system.)</span></p></td></tr><tr><td style="width:166.25pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="222"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>Allowed 
  Value Invalid Characters</span></p></td><td style="width:158.55pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="211"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>Policy 
  denies creation of an allowed value which contains any of the specified 
  characters</span></p></td><td style="width:142.7pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="190"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>A 
  list of invalid characters (Note: characters are not separated) Example: 
  #$%*^&amp;</span></p></td></tr><tr><td style="width:166.25pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="222"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>Category 
  Name Invalid Characters</span></p></td><td style="width:158.55pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="211"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>Policy 
  denies creation of Category names which contain any of the specified 
  characters.</span></p></td><td style="width:142.7pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="190"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>A 
  list of invalid characters (Note: characters are not separated)  Example: 
  #$%*&amp;^</span></p></td></tr><tr><td style="width:166.25pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="222"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>Category 
  Name Length</span></p></td><td style="width:158.55pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="211"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>Policy 
  allows minimum and maximum restrictions to be placed on Category names.</span></p></td><td style="width:142.7pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="190"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>A 
  minimum length and a maximum length.</span></p>
<p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>Default 
  settings are:</span></p>
<p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>Minimum 
  – 2</span></p>
<p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>Maximum 
  - 150</span></p></td></tr></table>

 


Note: 
Custom policies can be created and dropped into an existing environment. Please 
contact your support representative at Convergence Data for custom policies.  


 


**Changing 
policy settings:**


To 
change policy settings click the Settings 
link for the policy which is to be customized.  This action will display the 
settings associated with the policy.  Note: settings changes are automatically 
saved.


 


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/Policy_Manager_files/image001.jpg)




 


 


**Policy 
enforcement:**


To 
actively enforce any policy, the policy must be enabled.  To enable a policy, 
click the **Disabled** text.  This will change the policy to Enabled.  To 
disable a policy, click the **Enabled** text.


 


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/Policy_Manager_files/image002.png)

  ![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/Policy_Manager_files/image003.png)




 


Once 
a policy is Enabled a check will be applied in the associated module to ensure 
actions do not violate the policy.  For example, if the Category Name Length 
policy had a maximum length of 10 and a user tries to create a category name 
greater than 10 characters, the user will not be allowed to save with a 
validation error show.


 


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/Policy_Manager_files/image004.jpg)




 


**Policy 
validation and violations:**


Policy 
validation will validate if the currently defined data model meets the criteria 
defined in all the enabled policies.  A user must have both the “Policy 
Manager” and “Policy Validator” roles in order to perform a validation.  To 
validate the enabled policies, click the Validate button.


 


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/Policy_Manager_files/image005.png)




 


Once 
the policies are validated the count of violations will be shown to the right 
of the Settings link.  Violations are viewable by clicking the Violations link.


 


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/Policy_Manager_files/image006.jpg)




 


When 
viewing the violations each violation is shown in a list.  For category related 
violations, to see the complete category path click the View Tree link.


 


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/Policy_Manager_files/image007.jpg)






