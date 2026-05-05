



Loading\_Relationship\_Information - Design For Retrieval (DFR) Help




**Loading 
Relationship Information**


 


The 
Item Collection Memberships are loaded using a file with the "**.rdl**" 
file extension on the tab-delimited data load file. The following 
specifications must be met:


 


- The Collection Attribute must be entered in the 
 first line of the file in the following format:

 


Collection Attribute Name=COLLECTION\_ATTRIBUTE


 


where COLLECTION\_ATTRIBUTE is the name of the 
collection attribute. The collection attribute name is case sensitive.


 


- Both the Item and the Member must have a **Qualifier** 
 column in the load file.  The Member 
 must also have a root qualifier.
- The .rdl file format must include a column with 
 a header of **Operation**. This column will tell Item Loader what to do 
 with the item information on each line. The possible operation values 
 include:

**add** - Add an item to a relationship


**delete** - Delete an item from a relationship


**update** - Update the relationship attribute values


 





<table border="0" cellpadding="0" cellspacing="0" class="MsoNormalTable" style="width:472.0pt;margin-left:4.65pt;border-collapse:collapse;mso-padding-alt: 
 0in 5.4pt 0in 5.4pt" width="629"><tr style="mso-yfti-irow:0;mso-yfti-firstrow:yes;height:12.75pt"><td colspan="4" nowrap="nowrap" style="width:294.0pt;border: 
  solid windowtext 1.0pt;border-right:solid black 1.0pt;mso-border-alt:solid windowtext .5pt; 
  mso-border-right-alt:solid black .5pt;padding:0in 5.4pt 0in 5.4pt;height: 
  12.75pt" valign="bottom" width="392"><p class="MsoNormal">Collection 
  Attribute Name=Link Part to Document<p></p></p></td><td nowrap="nowrap" style="width:66.0pt;border:solid windowtext 1.0pt; 
  border-left:none;mso-border-top-alt:solid windowtext .5pt;mso-border-bottom-alt: 
  solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt;padding: 
  0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="88"><p class="MsoNormal"> <p></p></p></td><td nowrap="nowrap" style="width:47.0pt;border:solid windowtext 1.0pt; 
  border-left:none;mso-border-top-alt:solid windowtext .5pt;mso-border-bottom-alt: 
  solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt;padding: 
  0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="63"><p class="MsoNormal"> <p></p></p></td><td nowrap="nowrap" style="width:65.0pt;border:solid windowtext 1.0pt; 
  border-left:none;mso-border-top-alt:solid windowtext .5pt;mso-border-bottom-alt: 
  solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt;padding: 
  0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="87"><p class="MsoNormal"> <p></p></p></td></tr><tr style="mso-yfti-irow:1;height:24.0pt"><td style="width:70.0pt;border:solid windowtext 1.0pt; 
  border-top:none;mso-border-left-alt:solid windowtext .5pt;mso-border-bottom-alt: 
  solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt;padding: 
  0in 5.4pt 0in 5.4pt;height:24.0pt" valign="bottom" width="93"><p class="MsoNormal">Item 
  Number<p></p></p></td><td style="width:86.0pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-bottom-alt:solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt;height:24.0pt" valign="bottom" width="115"><p align="center" class="MsoNormal" style="text-align:center">Item Qualifier<p></p></p></td><td style="width:65.0pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-bottom-alt:solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt;height:24.0pt" valign="bottom" width="87"><p class="MsoNormal">Member 
  Item Number<p></p></p></td><td style="width:73.0pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-bottom-alt:solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt;height:24.0pt" valign="bottom" width="97"><p align="center" class="MsoNormal" style="text-align:center">Member Item Qualifier<p></p></p></td><td style="width:66.0pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-bottom-alt:solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt;height:24.0pt" valign="bottom" width="88"><p class="MsoNormal">Member 
  Item Root Qualifier<p></p></p></td><td style="width:47.0pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-bottom-alt:solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt; 
  background:yellow;padding:0in 5.4pt 0in 5.4pt;height:24.0pt" valign="bottom" width="63"><p class="MsoNormal">Operation<p></p></p></td><td style="width:65.0pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-bottom-alt:solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt;height:24.0pt" valign="bottom" width="87"><p class="MsoNormal">Purpose of 
  Reference<p></p></p></td></tr><tr style="mso-yfti-irow:2;height:12.75pt"><td nowrap="nowrap" style="width:70.0pt;border:solid windowtext 1.0pt; 
  border-top:none;mso-border-left-alt:solid windowtext .5pt;mso-border-bottom-alt: 
  solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt;padding: 
  0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="93"><p class="MsoNormal">BB02163-01<p></p></p></td><td nowrap="nowrap" style="width:86.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-bottom-alt:solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="115"><p align="center" class="MsoNormal" style="text-align:center">2602<p></p></p></td><td nowrap="nowrap" style="width:65.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-bottom-alt:solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="87"><p class="MsoNormal">000-8020<p></p></p></td><td nowrap="nowrap" style="width:73.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-bottom-alt:solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="97"><p align="center" class="MsoNormal" style="text-align:center">94756<p></p></p></td><td nowrap="nowrap" style="width:66.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-bottom-alt:solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="88"><p class="MsoNormal">Document<p></p></p></td><td nowrap="nowrap" style="width:47.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-bottom-alt:solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt; 
  background:yellow;padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="63"><p class="MsoNormal">delete<p></p></p></td><td nowrap="nowrap" style="width:65.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-bottom-alt:solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="87"><p class="MsoNormal">primary 
  def<p></p></p></td></tr><tr style="mso-yfti-irow:3;height:12.75pt"><td nowrap="nowrap" style="width:70.0pt;border:solid windowtext 1.0pt; 
  border-top:none;mso-border-left-alt:solid windowtext .5pt;mso-border-bottom-alt: 
  solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt;padding: 
  0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="93"><p class="MsoNormal">BB02163-01<p></p></p></td><td nowrap="nowrap" style="width:86.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-bottom-alt:solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="115"><p align="center" class="MsoNormal" style="text-align:center">2602<p></p></p></td><td nowrap="nowrap" style="width:65.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-bottom-alt:solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="87"><p class="MsoNormal">100-1005<p></p></p></td><td nowrap="nowrap" style="width:73.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-bottom-alt:solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="97"><p align="center" class="MsoNormal" style="text-align:center">2602<p></p></p></td><td nowrap="nowrap" style="width:66.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-bottom-alt:solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="88"><p class="MsoNormal">Document<p></p></p></td><td nowrap="nowrap" style="width:47.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-bottom-alt:solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt; 
  background:yellow;padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="63"><p class="MsoNormal">delete<p></p></p></td><td nowrap="nowrap" style="width:65.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-bottom-alt:solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="87"><p class="MsoNormal">general 
  spec<p></p></p></td></tr><tr style="mso-yfti-irow:4;height:12.75pt"><td nowrap="nowrap" style="width:70.0pt;border:solid windowtext 1.0pt; 
  border-top:none;mso-border-left-alt:solid windowtext .5pt;mso-border-bottom-alt: 
  solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt;padding: 
  0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="93"><p class="MsoNormal">BB02163-01<p></p></p></td><td nowrap="nowrap" style="width:86.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-bottom-alt:solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="115"><p align="center" class="MsoNormal" style="text-align:center">2602<p></p></p></td><td nowrap="nowrap" style="width:65.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-bottom-alt:solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="87"><p class="MsoNormal">100-1006<p></p></p></td><td nowrap="nowrap" style="width:73.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-bottom-alt:solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="97"><p align="center" class="MsoNormal" style="text-align:center">3953<p></p></p></td><td nowrap="nowrap" style="width:66.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-bottom-alt:solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="88"><p class="MsoNormal">Document<p></p></p></td><td nowrap="nowrap" style="width:47.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-bottom-alt:solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt; 
  background:yellow;padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="63"><p class="MsoNormal">update<p></p></p></td><td nowrap="nowrap" style="width:65.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-bottom-alt:solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="87"><p class="MsoNormal">primary 
  def<p></p></p></td></tr><tr style="mso-yfti-irow:5;height:12.75pt"><td nowrap="nowrap" style="width:70.0pt;border:solid windowtext 1.0pt; 
  border-top:none;mso-border-left-alt:solid windowtext .5pt;mso-border-bottom-alt: 
  solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt;padding: 
  0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="93"><p class="MsoNormal">BB02163-01R<p></p></p></td><td nowrap="nowrap" style="width:86.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-bottom-alt:solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="115"><p align="center" class="MsoNormal" style="text-align:center">3953<p></p></p></td><td nowrap="nowrap" style="width:65.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-bottom-alt:solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="87"><p class="MsoNormal">100-1007<p></p></p></td><td nowrap="nowrap" style="width:73.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-bottom-alt:solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="97"><p align="center" class="MsoNormal" style="text-align:center">2D627<p></p></p></td><td nowrap="nowrap" style="width:66.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-bottom-alt:solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="88"><p class="MsoNormal">Document<p></p></p></td><td nowrap="nowrap" style="width:47.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-bottom-alt:solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt; 
  background:yellow;padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="63"><p class="MsoNormal">update<p></p></p></td><td nowrap="nowrap" style="width:65.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-bottom-alt:solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="87"><p class="MsoNormal">primary 
  def<p></p></p></td></tr><tr style="mso-yfti-irow:6;mso-yfti-lastrow:yes;height:12.75pt"><td nowrap="nowrap" style="width:70.0pt;border:solid windowtext 1.0pt; 
  border-top:none;mso-border-left-alt:solid windowtext .5pt;mso-border-bottom-alt: 
  solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt;padding: 
  0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="93"><p class="MsoNormal">BB02163-01R<p></p></p></td><td nowrap="nowrap" style="width:86.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-bottom-alt:solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="115"><p align="center" class="MsoNormal" style="text-align:center">CAGE-Code.3953<p></p></p></td><td nowrap="nowrap" style="width:65.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-bottom-alt:solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="87"><p class="MsoNormal">100-1009<p></p></p></td><td nowrap="nowrap" style="width:73.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-bottom-alt:solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="97"><p align="center" class="MsoNormal" style="text-align:center">ORG-ID.77272<p></p></p></td><td nowrap="nowrap" style="width:66.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-bottom-alt:solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="88"><p class="MsoNormal">Document<p></p></p></td><td nowrap="nowrap" style="width:47.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-bottom-alt:solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt; 
  background:yellow;padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="63"><p class="MsoNormal">add<p></p></p></td><td nowrap="nowrap" style="width:65.0pt;border-top:none; 
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-bottom-alt:solid windowtext .5pt;mso-border-right-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt;height:12.75pt" valign="bottom" width="87"><p class="MsoNormal">general 
  spec<p></p></p></td></tr></table>


**In the sample relationship load file above, there is one 
relationship attribute called Purpose of Reference which always appears after 
the operation column.**




**To load relationship information using the DFR Item Loader:**


 


- Select the **Import** button from the top of 
 the screen.
- Select the import .rdl file
- Select the root qualifier for the item in the 
 relationship.
- Press the **Ok** button.
- Now map the Item Number’s in the mapping 
 fields.  Then map any relationship 
 attributes if there are relationship attributes to map.  Then select Preview and Import.
- The Item Loader Preview window will display the 
 contents of the import load file. It will also provide a summary of adds, 
 deletes and updates.  After 
 reviewing the contents, press the **Import** button to load the 
 data.

 




 


 


 


 


 


Return to [Preparing 
Data for the Item Loader](hs3020.md) 


 






