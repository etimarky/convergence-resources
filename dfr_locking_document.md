



DFR\_Locking\_Document - Design For Retrieval (DFR) Help




This document gives certain use cases for DFR that will 
cause a lock in a certain item or part of the application. An example of a lock 
is something that occurs when you have an item open for editing and someone 
else tried to open that same item for editing. In this scenario the user who 
already had the item open will still be able to edit the item but the second 
user opening that item will be prompted with a message that will let them know 
they do not have sole rights to that item causing their edit to be in a read 
only mode. All of these error messages below are expected and you should not be 
alarmed when you see one.





<table border="1" cellpadding="0" cellspacing="0" class="MsoNormalTable" style="border-collapse:collapse;border:none"><tr><td style="width:144.15pt;border:solid black 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="192"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal"><b><span style="font-size:14.0pt">User1</span></b></p></td><td style="width:334.65pt;border:solid black 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="446"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal"><b><span style="font-size:14.0pt">User2</span></b></p></td></tr><tr><td style="width:144.15pt;border:solid black 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="192"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Open Classification Manager and browse to the “Root\Raw 
  Materials\Tube and Pipe\Tube” Category </p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Double click on the “Condition” attribute to View or Edit it.</p></td><td style="width:334.65pt;border-top:none;border-left: 
  none;border-bottom:solid black 1.0pt;border-right:solid black 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="446"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Open Classification Manager and browse to the “Root\Raw 
  Materials\Tube and Pipe\Tube” Category </p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Double click on the “Condition” attribute to View or Edit it.</p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">You should see this error message:</p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal"><img height="120" src="../Images/image001.jpg" width="361"/></p></td></tr><tr><td style="width:144.15pt;border:solid black 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="192"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Open Classification Manager and browse to the “Root\Raw 
  Materials\Tube and Pipe\Tube” Category </p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Double click on the “Condition” attribute to View or Edit it.</p></td><td style="width:334.65pt;border-top:none;border-left: 
  none;border-bottom:solid black 1.0pt;border-right:solid black 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="446"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Open Data Developer set Batch to “All Batches”, User to “All Users”, 
  Status to “All Statuses” </p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Navigate to “Root\Raw Materials\Tube and Pipe\Tube” Category </p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Click Retrieve</p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">You should receive an error message similar to this:</p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal"><img height="124" src="../Images/image002.jpg" width="359"/></p></td></tr><tr><td style="width:144.15pt;border:solid black 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="192"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Open Data Developer set Batch to “All Batches”, User to “All Users”, 
  Status to “All Statuses” </p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Navigate to “Root\Raw Materials\Tube and Pipe\Tube” Category </p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Click Retrieve</p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal"> </p></td><td style="width:334.65pt;border-top:none;border-left: 
  none;border-bottom:solid black 1.0pt;border-right:solid black 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="446"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Open Classification Manager and browse to the “Root\Raw 
  Materials\Tube and Pipe\Tube” Category </p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Double click on the “Condition” attribute to View or Edit it.</p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">You should see this error message:</p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal"><img height="120" src="../Images/image003.jpg" width="361"/></p></td></tr><tr><td style="width:144.15pt;border:solid black 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="192"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Open Classification Manager and browse to the “Root\Raw 
  Materials\Tube and Pipe\Tube” Category </p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Double click on the “Condition” attribute to View or Edit it.</p></td><td style="width:334.65pt;border-top:none;border-left: 
  none;border-bottom:solid black 1.0pt;border-right:solid black 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="446"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Open Attribute Manager and search for “Condition” under the Words in 
  Name field.</p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Right Click on Condition in lower pane and change the Status to any User Defined status.</p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">A message similar to this should appear:</p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal"><img height="120" src="../Images/image004.jpg" width="362"/></p></td></tr><tr><td style="width:144.15pt;border:solid black 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="192"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Open Attribute Manager and search for “Condition” under the Words in 
  Name field.</p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Right Click on Condition in lower pane and change the Status to any User Defined status.</p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Click Edit</p></td><td style="width:334.65pt;border-top:none;border-left: 
  none;border-bottom:solid black 1.0pt;border-right:solid black 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="446"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Open Classification Manager and browse to the “Root\Raw 
  Materials\Tube and Pipe\Tube” Category </p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Double click on the “Condition” attribute to View or Edit it.</p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">A message similar to this should appear:</p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal"><img height="124" src="../Images/image005.jpg" width="371"/></p></td></tr><tr><td style="width:144.15pt;border:solid black 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="192"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Open Data Developer and make sure Browse Mode is un-checked. Set 
  Batch to “All Batches”, User to “All Users”, Status to “All Statuses” </p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Navigate to “Root\Raw Materials\Tube and Pipe\Tube” Category </p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Click Retrieve</p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal"> </p></td><td style="width:334.65pt;border-top:none;border-left: 
  none;border-bottom:solid black 1.0pt;border-right:solid black 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="446"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Open Classification Manager and browse to the “Root\Raw Materials\Tube 
  and Pipe\Tube” Category </p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Double click on the “Condition” attribute to View or Edit it.</p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">A message similar to this should appear:</p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal"><img height="124" src="../Images/image005.jpg" width="371"/></p></td></tr><tr><td style="width:144.15pt;border:solid black 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="192"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Open Item Loader and run an import using an import file. </p></td><td style="width:334.65pt;border-top:none;border-left: 
  none;border-bottom:solid black 1.0pt;border-right:solid black 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="446"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Open Data Developer and make sure Browse Mode is Un-Checked.</p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Navigate to the same category that the import is going to. </p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Try to edit the same data that was in the load file from the import. </p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">A message similar to this should appear:</p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal"><img height="124" src="../Images/image006.jpg" width="359"/></p></td></tr><tr><td style="width:144.15pt;border:solid black 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="192"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Open Item browser</p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Navigate to “Root\Raw Materials\Tube and Pipe\Tube”</p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Use “657013” in the Search String and click Search.</p></td><td style="width:334.65pt;border-top:none;border-left: 
  none;border-bottom:solid black 1.0pt;border-right:solid black 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="446"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Open Data Developer set Batch to “All Batches”, User to “All Users”, 
  Status to “All Statuses” </p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Navigate to “Root\Raw Materials\Tube and Pipe\Tube” Category </p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Click Retrieve</p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Double click item “657013” to edit it.</p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">You should receive an error message similar to this:</p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal"><img height="124" src="../Images/image007.jpg" width="359"/></p></td></tr><tr><td style="width:144.15pt;border:solid black 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="192"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Open allowed Values Manager</p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Navigate to “Root\Raw Materials\Slow Moving Inventory”</p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Select “Windchill Cabinet” for the Attributes value.</p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Select “Diode Application3” for the Global Allowed Values</p></td><td style="width:334.65pt;border-top:none;border-left: 
  none;border-bottom:solid black 1.0pt;border-right:solid black 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="446"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Open allowed Values Manager</p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Navigate to “Root\Raw Materials\Slow Moving Inventory”</p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Select “Windchill Cabinet” for the Attributes value.</p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Select “Diode Application3” for the Global Allowed Values</p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Click Use List if not already selected</p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Add a new Global Value of “Test”</p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Click “Save List”</p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">You should see a message similar to the one below asking what you 
  want to do with your changes:</p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal"><img height="216" src="../Images/image008.gif" width="432"/></p></td></tr><tr><td style="width:144.15pt;border:solid black 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="192"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Using the UOM Editor</p></td><td style="width:334.65pt;border-top:none;border-left: 
  none;border-bottom:solid black 1.0pt;border-right:solid black 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="446"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">No users can be logged into DFR or webDFR to commit changes to the 
  database.  You should receive an error message similar to this:</p>
<p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal"><img height="187" src="../Images/image009.jpg" width="242"/></p></td></tr></table>

 




