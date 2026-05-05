



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
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in">1.     
   </p></td><td style="width:170.8pt;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal">AllowGlobalDescriptionChanges</p></td><td style="width:246.8pt;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal">If 
  set to True, this allows the user to enable the control, and allow users to 
  uncheck it.  Users would be able to update items in Description 
  Generator that are NOT assigned to them.  This option is disabled by 
  default meaning the users can only change the Descriptions for items that are 
  assigned to them.</p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in">2.</p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal" style="background:white">AllowPropertyEditsOnApprovedCategories</p>
<p class="MsoNormal"> </p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal">Setting 
  this option to <b>true</b> or <b>yes</b> will allow category developers the 
  ability to update category properties even after the category itself has been 
  approved.</p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in">3.     
   </p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal">AVM 
  Inactivity Timeout</p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal">The 
  AVM module closes if a user is inactive for this period of time.  
  Defaults to the value in [Client Inactivity Timeout].</p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in">4.     
   </p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal">Client 
  Inactivity Timeout</p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal">Some 
  modules drop a user into Browse-Mode (read only) if the user is inactive for 
  this period of time.  Defaults to 300 seconds.</p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in">5.     
   </p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal">Default 
  Batch Name</p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal">If 
  you do not enter a batch name in (Item Loader / New) you get the Batch: 
  "Default Batch".  <u>Default Batch Name</u> allows you to 
  override that to another name.</p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in">6.     
   </p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal">DefCategInhAttr</p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal">If set to TRUE, the box for inheriting attributes will be 
  checked by default in the Classification Manager.  All newly created 
  categories will have <i>Inherit Attributes</i> selected.  If set to 
  FALSE, the default will be unchecked.  If the value is set to INHERIT 
  then newly created categories will default to what the parent category has 
  set for <i>Inherit Attributes</i>.</p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in">6.     
   </p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal">DefCategInhSec</p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal">If set to True, the box for inheriting security will be checked 
  by default in the Classification Manager.  All newly created categories 
  will have <i>Inherit Securit</i>y selected. If set to FALSE, the default will 
  be unchecked. If the value is set to INHERIT then newly created categories 
  will default to what the parent category has set for <i>Inherit Security</i>.</p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in">7.</p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal">Default 
  Does Not Apply (DNA)</p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal">If set to True, Attributes added to a Category will have their 
  Allow “Does Not Apply” property checked.</p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in">8.     
   </p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal">Default 
  Decimal Places</p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal">Sets the default decimal places globally for all numeric 
  attribute values.  E.g. Default Decimal Places = 5  (This sets the 
  global default decimal places equal to 5.)  Note: This value can be 
  overridden by local changes made with the attribute properties.  If not 
  set, the default is 2.</p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in">9.     
   </p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal">DropinDir</p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal">This 
  is the path to the dropin directory on the Remoting Server.</p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in">10.     
   </p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal">DnaTag</p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal">This 
  is the string displayed in Data Developer and elsewhere when Non-Appl = 
  true.  The default value is: "&lt;DNA&gt;"</p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in">11.  
   </p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal">ExportCateg</p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal">If 
  set to true, it extends 2 reports: <u>Export-Text Item Attribute Values</u> 
  and <u>Export-XL Item Attribute Values</u> to have an extra column showing 
  the full category path of each item.</p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in">12.  
   </p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal">HideLdrBatches </p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal">If 
  present and set to “True”, loader batches are hidden in many places.  
  Once you have hidden load batch names, only the working batch names appear in 
  most of the batch filters that are used in Item Browser, Data Developer, Data 
  Validator and Allowed Values Manager.  Load batch names will always show 
  in the Item Loader and Batch Removal modules.</p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in">13.  
   </p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal">HowToHandleWhiteSpace</p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal">If set to “Ignore” (default), when a new Allowed Value is created 
  it will save allowed values that have leading/trailing whitespace as is. If 
  set to “Ask” then a dialog box will popup when creating a new allowed value 
  asking if you would like to trim the whitespaces before committing the new 
  value. If set to “Trim”, for new allowed values the leading/trailing 
  whitespace will be removed and the value will be saved without it.</p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in">14.  
   </p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal">ItemLoadAutoGenText</p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal">The value for this option will be used to trigger the auto 
  creation of the item number. For example if the value “$” is used with this 
  command, any item numbers that have “$” will auto-generate the next item 
  number.  This field can be a single value like “$” or multiple values 
  like “gen number”.  This feature works with a specific qualifier that 
  your DFR technical admin can set. E.g. part.auto.  See Item Loader help 
  files for additional detail for item number auto-generation.</p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in">15.  
   </p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal">MaxValuePicks</p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal">In 
  Data Developer, the dialog that configures search criteria often offers a 
  list of existing values to pick from, but only when the number of values is 
  less than MaxValuePicks.  The default is 500.</p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in">16.  
   </p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal">multiValSeparator</p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal">This 
  is the internally stored separator when an attribute value is saved to the 
  database.  This can be set in the Remoting Server config file as well in 
  the &lt;CDSSvrOptions&gt; section.  The default is ‘\n’ 
  (newline). </p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in">17.  
   </p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal">OnlyLatestRevInResults</p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal">If 
  present and set to “True” (thus default = false), only the latest revision of 
  the item will be shown in DFR’s Data Developer and SmartFind search 
  results.  If set to False or missing from the TblOptions table, all 
  revisions are shown in SmartFind and Show All Revisions link is enabled in 
  Data Developer.  Revision Date will determine the revision order and 
  which revision of a particular part is the latest. The assignment of Revision 
  Manager role overrides this setting.   </p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in">18.  
   </p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal">RemoveBatch_HideDefault</p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal">If 
  present and set to “True” (thus default = false), the default batch is not 
  offered by the RemoveBatch tool/dialog.</p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in">19.  
   </p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal">ReportsExcelPickListOK</p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal">If 
  set to true, will show pick lists in export file for Data Developer.  
  Eg. UOM and Allowed Values Lists.</p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in">20.  
   </p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal">SandboxMode</p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal">If 
  present and not set to “false”, “off”, or “0” (thus default = off), the user 
  is allowed to delete batches where some of the items are no longer new.  
  This setting is not recommended for production catalogs as is would allow 
  item numbers to be re-used.</p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in">21.  
   </p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal">SFTPConfig</p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal">This supports secure FTP.  Configuration should be the 
  following:  
  &lt;host&gt;;&lt;port&gt;;&lt;user&gt;;&lt;pwd&gt;;&lt;identityFile&gt;;&lt;accessURL&gt;</p>
<p class="MsoNormal">NOTE:  &lt;identityFile&gt; is the path including the 
  filename on the client machine.  </p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in">22.  
   </p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal">SuperSetStatus</p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal">If set to “True”, category admin will be able to use the new 
  control shift and right click option to override category attribute status 
  changes (cascading changes) in Classification Manager for category 
  attributes.  If this field is empty, then you will not have this 
  capability.</p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in">23.  
   </p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal">Welcome 
  Page Target</p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal">The default URL is the Convergence home page. This can be 
  changed to other available URL’s</p></td></tr><tr><td style="width:49.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="65"><p class="MsoListParagraph" style="text-indent:-.25in">24.  
   </p></td><td style="width:170.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="228"><p class="MsoNormal">AttrTextBoxThreshold</p></td><td style="width:246.8pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="329"><p class="MsoNormal">String Attributes with a length greater than this value will be displayed as 
  multi-line text areas.</p></td></tr></table>

 **Options that should only be modified on advice from CDS:**




<table border="0" cellpadding="0" cellspacing="0" class="MsoNormalTable" style="width:6.25in;margin-left:5.4pt;border-collapse:collapse" width="600"><tr><td style="width:31.5pt;border:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="42"><p class="MsoNormal">1</p></td><td style="width:2.0in;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="192"><p class="MsoNormal">ClassTimeoutScaleFactor</p></td><td style="width:274.5pt;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="366"><p class="MsoNormal">Defaults 
  to 20000.  DFR uses this value to compute timeouts for SQL that are 
  influenced by the size of tblCategoryAttribute_c.  Thus if you have 
  50,000 category_item records, CDS may advise that you set this value to 
  50000.  This is <u>deliberately not computed</u> from the size of 
  tblCategoryAttribute_c.</p>
<p class="MsoNormal"> </p></td></tr><tr><td style="width:31.5pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="42"><p class="MsoNormal">2</p></td><td style="width:2.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="192"><p class="MsoNormal">GlobalTimeoutScaleFactor</p></td><td style="width:274.5pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="366"><p class="MsoNormal">Defaults 
  to 100.  DFR uses this value to scale timeouts for SQL.</p></td></tr><tr><td style="width:31.5pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="42"><p class="MsoNormal">3</p></td><td style="width:2.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="192"><p class="MsoNormal">ItemTimeoutScaleFactor</p></td><td style="width:274.5pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="366"><p class="MsoNormal">Defaults 
  to 750000.  DFR uses this value to compute timeouts for SQL that are 
  influenced by the number of items in the database.  Thus if you have 
  2,000,000 items in your database, CDS may advise that you set this value to 
  2000000.  This is <u>deliberately not computed</u> from the size of 
  tblItems.</p></td></tr><tr><td style="width:31.5pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="42"><p class="MsoNormal">4</p></td><td style="width:2.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="192"><p class="MsoNormal">UomCheckout</p></td><td style="width:274.5pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="366"><p class="MsoNormal">When 
  a user checks-out the UOM data to edit it, DFR puts that person’s name here.</p></td></tr><tr><td style="width:31.5pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="42"><p class="MsoNormal">5</p></td><td style="width:2.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="192"><p class="MsoNormal">Where 
  Used Display Limit</p></td><td style="width:274.5pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="366"><p class="MsoNormal">Defaults 
  to 100000.  In Item Browser, a collection-where-used search might return 
  an excessive number of results that would overrun the memory of a client 
  system.  This value protects that.  An under-configured system 
  might do better with a lower value.  A heavily configured system might 
  be able to handle a higher value.</p></td></tr></table>

 


**Options 
that are modified in the CDS DFR Config file:**




<table border="0" cellpadding="0" cellspacing="0" class="MsoNormalTable" style="width:6.25in;margin-left:5.4pt;border-collapse:collapse" width="600"><tr><td style="width:31.5pt;border:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="42"><p class="MsoNormal">1</p></td><td style="width:2.0in;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="192"><p class="MsoNormal">MaxTimeSpanToReconnect</p></td><td style="width:274.5pt;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="366"><p class="MsoNormal">This 
  setting allow a delay to be set (0-10000 msec (100 seconds)) once a network 
  drop has occurred.  This configuration can be set locally or globally in 
  the config file.  (see details below)</p></td></tr></table>

 


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




