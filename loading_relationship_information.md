



Loading\_Relationship\_Information - Design For Retrieval (DFR) Help




**Item 
Key Rename Loader**


 


If there are a group of items that need to have their item key 
updated for any reason, such as the need to set a proper revision, there is a 
load file type that allows for this.  In order to change a group of items' item 
keys, a file with the "**.irl**" file extension on a tab-delimited 
data load file can be used.


 


The following specifications must be met:


 


- There must be an Item Number field 
 specified.  It can have any name as it will be mapped during load time.
- The item revision column and item 
 qualifier columns are optional.  If they are not specified then it will be 
 assumed the revision of the part/item is empty and the qualifier is the 
 default, 0.  **Note:** The qualifier column contains the full qualifier 
 minus the root qualifier as that is specified in the load user interface.  
 Ex: Part.CageCode.123 should be in spreadsheet as CageCode.123
- The following three columns are mandatory and must have the 
 following names (case doesn't matter):  
  
**New Item Number:** This is the field that will hold what the new item 
 number will be.  If the item number is not changing then specify the 
 original item number in this field.  
  
**New Revision**: This is the field that will hold what the new 
 revision of the part will be.  If the revision is not changing then specify 
 the original revision value.  
  
**New Item Qualifier**: This is the field that will hold what the new 
 qualifier of the part will be.  The qualifier MUST be specified in full, 
 including the root qualifier.  If the qualifier is not changing then 
 specify the original qualifier value in this field.

 





<table border="0" cellpadding="0" cellspacing="0" class="MsoNormalTable" style="width:453.0pt;margin-left:4.65pt;border-collapse:collapse" width="604"><tr style="height:24.0pt"><td style="width:70.0pt;border:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:24.0pt" valign="bottom" width="93"><p class="MsoNormal"><span style='font-size:9.0pt;font-family:"Arial","sans-serif"'>Item 
  Number</span></p></td><td style="width:86.0pt;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt;height:24.0pt" valign="bottom" width="115"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:9.0pt;font-family:"Arial","sans-serif"'>Item Revision</span></p></td><td style="width:86.0pt;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt;height:24.0pt" valign="bottom" width="115"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:9.0pt;font-family:"Arial","sans-serif"'>Item Qualifier</span></p></td><td style="width:65.0pt;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt;height:24.0pt" valign="bottom" width="87"><p class="MsoNormal"><span style='font-size:9.0pt;font-family:"Arial","sans-serif"'>New 
  Item Number</span></p></td><td style="width:73.0pt;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt;height:24.0pt" valign="bottom" width="97"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:9.0pt;font-family:"Arial","sans-serif"'>New Revision</span></p></td><td style="width:73.0pt;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt;height:24.0pt" valign="bottom" width="97"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:9.0pt;font-family:"Arial","sans-serif"'>New Item Qualifier</span></p></td></tr><tr style="height:12.75pt"><td nowrap="nowrap" style="width:70.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="93"><p class="MsoNormal"><span style='font-size:9.0pt;font-family:"Arial","sans-serif"'>BB02163-01</span></p></td><td style="width:86.0pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="115"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:9.0pt;font-family:"Arial","sans-serif"'>Rev1</span></p></td><td nowrap="nowrap" style="width:86.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="115"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:9.0pt;font-family:"Arial","sans-serif"'>Cage-Code.2602</span></p></td><td nowrap="nowrap" style="width:65.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="87"><p class="MsoNormal"><span style='font-size:9.0pt;font-family:"Arial","sans-serif"'>BB02163-01</span></p></td><td style="width:73.0pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="97"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:9.0pt;font-family:"Arial","sans-serif"'>Rev1</span></p></td><td nowrap="nowrap" style="width:73.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="97"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:9.0pt;font-family:"Arial","sans-serif"'>Part.2602</span></p></td></tr><tr style="height:12.75pt"><td nowrap="nowrap" style="width:70.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="93"><p class="MsoNormal"><span style='font-size:9.0pt;font-family:"Arial","sans-serif"'>BC02163-02</span></p></td><td style="width:86.0pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="115"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:9.0pt;font-family:"Arial","sans-serif"'>Rev1</span></p></td><td nowrap="nowrap" style="width:86.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="115"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:9.0pt;font-family:"Arial","sans-serif"'>2602</span></p></td><td nowrap="nowrap" style="width:65.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="87"><p class="MsoNormal"><span style='font-size:9.0pt;font-family:"Arial","sans-serif"'>BB02163-02</span></p></td><td style="width:73.0pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="97"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:9.0pt;font-family:"Arial","sans-serif"'>Rev1</span></p></td><td nowrap="nowrap" style="width:73.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="97"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:9.0pt;font-family:"Arial","sans-serif"'>Part.2602</span></p></td></tr><tr style="height:12.75pt"><td nowrap="nowrap" style="width:70.0pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="93"><p class="MsoNormal"><span style='font-size:9.0pt;font-family:"Arial","sans-serif"'>BB02163-03</span></p></td><td style="width:86.0pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="115"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:9.0pt;font-family:"Arial","sans-serif"'> </span></p></td><td nowrap="nowrap" style="width:86.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="115"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:9.0pt;font-family:"Arial","sans-serif"'>2602</span></p></td><td nowrap="nowrap" style="width:65.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="87"><p class="MsoNormal"><span style='font-size:9.0pt;font-family:"Arial","sans-serif"'>BB02163-03</span></p></td><td style="width:73.0pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="97"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:9.0pt;font-family:"Arial","sans-serif"'>Rev1</span></p></td><td nowrap="nowrap" style="width:73.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="97"><p align="center" class="MsoNormal" style="text-align:center"><span style='font-size:9.0pt;font-family:"Arial","sans-serif"'>Part.2602</span></p></td></tr></table>


**To rename items using the DFR Item Loader:**


- Select the **Import** button from the 
 top of the screen.  It must be the **Import** button.  An error will 
 occur if the **New** or **Regen** options are chosen.
- Select the import **.irl** file
- Select the root qualifier for the item 
 in the relationship.
- Press the **Ok** button.
- Now map the Item Number, Revision, and 
 Item Qualifier in the mapping fields then select **Preview and Import**.

 


Return 
to [Item Loader](/html/hs3000.md)




