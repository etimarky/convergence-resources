



Options\_Manager - Design For Retrieval (DFR) Help




**Catalog 
Options**


 


There are certain features and behaviors that 
can be controlled at the catalog level.  These changes can be made in the 
Options Manager module.  Only those who log in as Catalog Administrator 
will be able to make changes in this module.  All other users will be able 
to view this module but not make changes.  Once a change is made in the 
Options Manager, changes do not require a restart of the Remoting Server.  



The 
local override column in Options Manager shows overrides per the config file on 
the specific client system. This is a read only field.  Changes are done 
through the local configuration file.  An example of when this might be 
necessary is to increase time out values for users over the Wide Area Networks 
that have network issues.



**Options that you may choose to change:**




<table border="0" cellpadding="0" cellspacing="0" class="MsoNormalTable" style="width:7.0in;border-collapse:collapse" width="672"><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in"><span style='font-size: 
  10.0pt;font-family:"Arial",sans-serif'>1.</span><span style="font-size:7.0pt">     
  </span><span style='font-size:10.0pt;font-family:"Arial",sans-serif'> </span></p></td><td style="width:170.8pt;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>AllowGlobalDescriptionChanges</span></p></td><td style="width:246.8pt;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>If 
  set to True, this allows the user to enable the control, and allow users to 
  uncheck it.  Users would be able to update items in Description 
  Generator that are NOT assigned to them.  This option is disabled by 
  default meaning the users can only change the Descriptions for items that are 
  assigned to them.</span></p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in"><span style='font-size: 
  10.0pt;font-family:"Arial",sans-serif'>2.</span></p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal" style="background:white"><span style='font-size:10.0pt; 
  font-family:"Arial",sans-serif'>AllowPropertyEditsOnApprovedCategories</span></p>
<p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'> </span></p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>Setting 
  this option to <b>true</b> or <b>yes</b> will allow category developers the 
  ability to update category properties even after the category itself has been 
  approved.</span></p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in"><span style='font-size: 
  10.0pt;font-family:"Arial",sans-serif'>3.</span><span style="font-size:7.0pt">     
  </span><span style='font-size:10.0pt;font-family:"Arial",sans-serif'> </span></p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>AVM 
  Inactivity Timeout</span></p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>The 
  AVM module closes if a user is inactive for this period of time.  
  Defaults to the value in [Client Inactivity Timeout].</span></p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in"><span style='font-size: 
  10.0pt;font-family:"Arial",sans-serif'>4.</span><span style="font-size:7.0pt">     
  </span><span style='font-size:10.0pt;font-family:"Arial",sans-serif'> </span></p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>Client 
  Inactivity Timeout</span></p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>Some 
  modules drop a user into Browse-Mode (read only) if the user is inactive for 
  this period of time.  Defaults to 300 seconds.</span></p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in"><span style='font-size: 
  10.0pt;font-family:"Arial",sans-serif'>5.</span><span style="font-size:7.0pt">     
  </span><span style='font-size:10.0pt;font-family:"Arial",sans-serif'> </span></p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>Default 
  Batch Name</span></p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>If 
  you do not enter a batch name in (Item Loader / New) you get the Batch: 
  "Default Batch".  <u>Default Batch Name</u> allows you to 
  override that to another name.</span></p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in"><span style='font-size: 
  10.0pt;font-family:"Arial",sans-serif'>6.</span><span style="font-size:7.0pt">     
  </span><span style='font-size:10.0pt;font-family:"Arial",sans-serif'> </span></p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>DefCategInhAttr</span></p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>If set to TRUE, the box for inheriting attributes will be 
  checked by default in the Classification Manager.  All newly created 
  categories will have <i>Inherit Attributes</i> selected.  If set to 
  FALSE, the default will be unchecked.  If the value is set to INHERIT 
  then newly created categories will default to what the parent category has 
  set for <i>Inherit Attributes</i>.</span></p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in"><span style='font-size: 
  10.0pt;font-family:"Arial",sans-serif'>6.</span><span style="font-size:7.0pt">     
  </span><span style='font-size:10.0pt;font-family:"Arial",sans-serif'> </span></p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>DefCategInhSec</span></p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>If set to True, the box for inheriting security will be checked 
  by default in the Classification Manager.  All newly created categories 
  will have <i>Inherit Securit</i>y selected. If set to FALSE, the default will 
  be unchecked. If the value is set to INHERIT then newly created categories 
  will default to what the parent category has set for <i>Inherit Security</i>.</span></p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in"><span style='font-size: 
  10.0pt;font-family:"Arial",sans-serif'>7.</span></p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>Default 
  Does Not Apply (DNA)</span></p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>If set to True, Attributes added to a Category will have their 
  Allow “Does Not Apply” property checked.</span></p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in"><span style='font-size: 
  10.0pt;font-family:"Arial",sans-serif'>8.</span><span style="font-size:7.0pt">     
  </span><span style='font-size:10.0pt;font-family:"Arial",sans-serif'> </span></p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>Default 
  Decimal Places</span></p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>Sets the default decimal places globally for all numeric 
  attribute values.  E.g. Default Decimal Places = 5  (This sets the 
  global default decimal places equal to 5.)  Note: This value can be 
  overridden by local changes made with the attribute properties.  If not 
  set, the default is 2.</span></p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in"><span style='font-size: 
  10.0pt;font-family:"Arial",sans-serif'>9.</span><span style="font-size:7.0pt">     
  </span><span style='font-size:10.0pt;font-family:"Arial",sans-serif'> </span></p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>DropinDir</span></p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>This 
  is the path to the dropin directory on the Remoting Server.</span></p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in"><span style='font-size: 
  10.0pt;font-family:"Arial",sans-serif'>10.</span><span style="font-size:7.0pt">     
  </span><span style='font-size:10.0pt;font-family:"Arial",sans-serif'> </span></p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>DnaTag</span></p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>This 
  is the string displayed in Data Developer and elsewhere when Non-Appl = 
  true.  The default value is: "&lt;DNA&gt;"</span></p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in"><span style='font-size: 
  10.0pt;font-family:"Arial",sans-serif'>11.</span><span style="font-size:7.0pt">  
  </span><span style='font-size:10.0pt;font-family:"Arial",sans-serif'> </span></p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>ExportCateg</span></p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>If 
  set to true, it extends 2 reports: <u>Export-Text Item Attribute Values</u> 
  and <u>Export-XL Item Attribute Values</u> to have an extra column showing 
  the full category path of each item.</span></p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in"><span style='font-size: 
  10.0pt;font-family:"Arial",sans-serif'>12.</span><span style="font-size:7.0pt">  
  </span><span style='font-size:10.0pt;font-family:"Arial",sans-serif'> </span></p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>HideLdrBatches </span></p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>If 
  present and set to “True”, loader batches are hidden in many places.  
  Once you have hidden load batch names, only the working batch names appear in 
  most of the batch filters that are used in Item Browser, Data Developer, Data 
  Validator and Allowed Values Manager.  Load batch names will always show 
  in the Item Loader and Batch Removal modules.</span></p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in"><span style='font-size: 
  10.0pt;font-family:"Arial",sans-serif'>13.</span><span style="font-size:7.0pt">  
  </span><span style='font-size:10.0pt;font-family:"Arial",sans-serif'> </span></p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>HowToHandleWhiteSpace</span></p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>If set to “Ignore” (default), when a new Allowed Value is created 
  it will save allowed values that have leading/trailing whitespace as is. If 
  set to “Ask” then a dialog box will popup when creating a new allowed value 
  asking if you would like to trim the whitespaces before committing the new 
  value. If set to “Trim”, for new allowed values the leading/trailing 
  whitespace will be removed and the value will be saved without it.</span></p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in"><span style='font-size: 
  10.0pt;font-family:"Arial",sans-serif'>14.</span><span style="font-size:7.0pt">  
  </span><span style='font-size:10.0pt;font-family:"Arial",sans-serif'> </span></p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>ItemLoadAutoGenText</span></p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>The value for this option will be used to trigger the auto 
  creation of the item number. For example if the value “$” is used with this 
  command, any item numbers that have “$” will auto-generate the next item 
  number.  This field can be a single value like “$” or multiple values 
  like “gen number”.  This feature works with a specific qualifier that 
  your DFR technical admin can set. E.g. part.auto.  See Item Loader help 
  files for additional detail for item number auto-generation.</span></p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in"><span style='font-size: 
  10.0pt;font-family:"Arial",sans-serif'>15.</span><span style="font-size:7.0pt">  
  </span><span style='font-size:10.0pt;font-family:"Arial",sans-serif'> </span></p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>MaxValuePicks</span></p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>In 
  Data Developer, the dialog that configures search criteria often offers a 
  list of existing values to pick from, but only when the number of values is 
  less than MaxValuePicks.  The default is 500.</span></p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in"><span style='font-size: 
  10.0pt;font-family:"Arial",sans-serif'>16.</span><span style="font-size:7.0pt">  
  </span><span style='font-size:10.0pt;font-family:"Arial",sans-serif'> </span></p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal"><span style="color:black">multiValSeparator</span></p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>This 
  is the internally stored separator when an attribute value is saved to the 
  database.  This can be set in the Remoting Server config file as well in 
  the </span><span style='font-size:11.0pt;font-family:"Calibri",sans-serif; 
  color:#1F497D'>&lt;CDSSvrOptions&gt; section.  The default is ‘\n’ 
  (newline). </span></p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in"><span style='font-size: 
  10.0pt;font-family:"Arial",sans-serif'>17.</span><span style="font-size:7.0pt">  
  </span><span style='font-size:10.0pt;font-family:"Arial",sans-serif'> </span></p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>OnlyLatestRevInResults</span></p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>If 
  present and set to “True” (thus default = false), only the latest revision of 
  the item will be shown in DFR’s Data Developer and SmartFind search 
  results.  If set to False or missing from the TblOptions table, all 
  revisions are shown in SmartFind and Show All Revisions link is enabled in 
  Data Developer.  Revision Date will determine the revision order and 
  which revision of a particular part is the latest. The assignment of Revision 
  Manager role overrides this setting.   </span></p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in"><span style='font-size: 
  10.0pt;font-family:"Arial",sans-serif'>18.</span><span style="font-size:7.0pt">  
  </span><span style='font-size:10.0pt;font-family:"Arial",sans-serif'> </span></p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>RemoveBatch_HideDefault</span></p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>If 
  present and set to “True” (thus default = false), the default batch is not 
  offered by the RemoveBatch tool/dialog.</span></p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in"><span style='font-size: 
  10.0pt;font-family:"Arial",sans-serif'>19.</span><span style="font-size:7.0pt">  
  </span><span style='font-size:10.0pt;font-family:"Arial",sans-serif'> </span></p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>ReportsExcelPickListOK</span></p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>If 
  set to true, will show pick lists in export file for Data Developer.  
  Eg. UOM and Allowed Values Lists.</span></p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in"><span style='font-size: 
  10.0pt;font-family:"Arial",sans-serif'>20.</span><span style="font-size:7.0pt">  
  </span><span style='font-size:10.0pt;font-family:"Arial",sans-serif'> </span></p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>SandboxMode</span></p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>If 
  present and not set to “false”, “off”, or “0” (thus default = off), the user 
  is allowed to delete batches where some of the items are no longer new.  
  This setting is not recommended for production catalogs as is would allow 
  item numbers to be re-used.</span></p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in"><span style='font-size: 
  10.0pt;font-family:"Arial",sans-serif'>21.</span><span style="font-size:7.0pt">  
  </span><span style='font-size:10.0pt;font-family:"Arial",sans-serif'> </span></p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>SFTPConfig</span></p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>This supports secure FTP.  Configuration should be the 
  following:  
  &lt;host&gt;;&lt;port&gt;;&lt;user&gt;;&lt;pwd&gt;;&lt;identityFile&gt;;&lt;accessURL&gt;</span></p>
<p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>NOTE:  &lt;identityFile&gt; is the path including the 
  filename on the client machine.  </span></p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in"><span style='font-size: 
  10.0pt;font-family:"Arial",sans-serif'>22.</span><span style="font-size:7.0pt">  
  </span><span style='font-size:10.0pt;font-family:"Arial",sans-serif'> </span></p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>SuperSetStatus</span></p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>If set to “True”, category admin will be able to use the new 
  control shift and right click option to override category attribute status 
  changes (cascading changes) in Classification Manager for category 
  attributes.  If this field is empty, then you will not have this 
  capability.</span></p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in"><span style='font-size: 
  10.0pt;font-family:"Arial",sans-serif'>23.</span><span style="font-size:7.0pt">  
  </span><span style='font-size:10.0pt;font-family:"Arial",sans-serif'> </span></p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>Welcome 
  Page Target</span></p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>The default URL is the Convergence home page. This can be 
  changed to other available URL’s</span></p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in"><span style='font-size: 
  10.0pt;font-family:"Arial",sans-serif'>24.</span><span style="font-size:7.0pt">  
  </span><span style='font-size:10.0pt;font-family:"Arial",sans-serif'> </span></p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>AttrTextBoxThreshold</span></p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>String Attributes with a length greater than this value will be displayed as 
  multi-line text areas.</span></p></td></tr></table>

 **Options that should only be modified on advice from CDS:**




<table border="0" cellpadding="0" cellspacing="0" class="MsoNormalTable" style="width:6.25in;margin-left:5.4pt;border-collapse:collapse" width="600"><tr><td style="width:31.5pt;border:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="42"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>1</span></p></td><td style="width:2.0in;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="192"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>ClassTimeoutScaleFactor</span></p></td><td style="width:274.5pt;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="366"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>Defaults 
  to 20000.  DFR uses this value to compute timeouts for SQL that are 
  influenced by the size of tblCategoryAttribute_c.  Thus if you have 
  50,000 category_item records, CDS may advise that you set this value to 
  50000.  This is <u>deliberately not computed</u> from the size of 
  tblCategoryAttribute_c.</span></p>
<p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'> </span></p></td></tr><tr><td style="width:31.5pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="42"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>2</span></p></td><td style="width:2.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="192"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>GlobalTimeoutScaleFactor</span></p></td><td style="width:274.5pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="366"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>Defaults 
  to 100.  DFR uses this value to scale timeouts for SQL.</span></p></td></tr><tr><td style="width:31.5pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="42"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>3</span></p></td><td style="width:2.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="192"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>ItemTimeoutScaleFactor</span></p></td><td style="width:274.5pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="366"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>Defaults 
  to 750000.  DFR uses this value to compute timeouts for SQL that are 
  influenced by the number of items in the database.  Thus if you have 
  2,000,000 items in your database, CDS may advise that you set this value to 
  2000000.  This is <u>deliberately not computed</u> from the size of 
  tblItems.</span></p></td></tr><tr><td style="width:31.5pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="42"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>4</span></p></td><td style="width:2.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="192"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>UomCheckout</span></p></td><td style="width:274.5pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="366"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>When 
  a user checks-out the UOM data to edit it, DFR puts that person’s name here.</span></p></td></tr><tr><td style="width:31.5pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="42"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>5</span></p></td><td style="width:2.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="192"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>Where 
  Used Display Limit</span></p></td><td style="width:274.5pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="366"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>Defaults 
  to 100000.  In Item Browser, a collection-where-used search might return 
  an excessive number of results that would overrun the memory of a client 
  system.  This value protects that.  An under-configured system 
  might do better with a lower value.  A heavily configured system might 
  be able to handle a higher value.</span></p></td></tr></table>

 


**Options 
that are modified in the CDS DFR Config file:**




<table border="0" cellpadding="0" cellspacing="0" class="MsoNormalTable" style="width:6.25in;margin-left:5.4pt;border-collapse:collapse" width="600"><tr><td style="width:31.5pt;border:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="42"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>1</span></p></td><td style="width:2.0in;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="192"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>MaxTimeSpanToReconnect</span></p></td><td style="width:274.5pt;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="366"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif'>This 
  setting allow a delay to be set (0-10000 msec (100 seconds)) once a network 
  drop has occurred.  This configuration can be set locally or globally in 
  the config file.  (see details below)</span></p></td></tr></table>

 


In 
the config file, you will have an uncommented line which starts with  
“<channel type=”Belikov.GenuineChannels.Genuine Tcp…”.  You will need 
to add MaxTimeSpanToReconnect=”x” where x is the number of milliseconds from 0 
to 10000.  


 


Your 
new line should look similar to this:



**Client 
Example**


<channel 
type="Belikov.GenuineChannels.GenuineTcp.GenuineTcpChannel, 
GenuineChannels" MaxTimeSpanToReconnect="10000" 
MaxTimeSpanToReconnect="5000" InvocationTimeout="3600000" 
ClosePersistentConnectionAfterInactivity="3600000" name="DFR 
Channel" />


 


**Server 
Example**


<channel 
type="Belikov.GenuineChannels.GenuineTcp.GenuineTcpChannel, 
GenuineChannels" MaxTimeSpanToReconnect="10000" 
InvocationTimeout="3600000" 
ClosePersistentConnectionAfterInactivity="3600000" NoSizeChecking="true" 
port="65100" name="DFR Server Channel">


 


To 
set this locally, you will need to add the entry in the “Program 
Files\Convergence Data Services\CDS Toolset Universal\CDSTOOLSET.exe.config” 
file.  To set this globally, you will need to add the entry in the 
“Program Files\Convergence Data Services\DFR Remoting 
Server\Shared\RmtSvr.exe.config” file.  




