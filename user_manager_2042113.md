



User\_Manager - Design For Retrieval (DFR) Help




**Item Clusters**


 


### Application 
Overview


·         
The 
Item Cluster (IC) application is available as a DFR dropin; it will be listed 
under the applications icons as well in the tools menu in DFR.


·         
The 
IC application can create clusters from working batches defined in DFR.


·         
Category 
attributes can be weighted for each cluster as well as a sensitivity factor 
(neighbor distance) can be set to help contract or expand the cluster size


·         
Clusters 
can be exported along with their attribute settings; along users to share their 
cluster data


·         
An 
XML file is also produced with each export; this file can be used to share data 
from your particular session with another user.  
Since the Item Cluster only creates clusters locally; including the 
weighting factors; the way to share information for a batch is to share the xml 
file


·         
As 
second XML file with the cxp extension is used for integrating with the 
co-exprise sourcing application; this a way to share cluster data with a 
strategic sourcing application


·         
All 
DFR users currently can use this new module; to access this new module click on 
the IC icon on the Toolbox or use the tools menu


### Intial 
Log-in


When logging into the IC application 
a user is presented with two grids; the top grid represents the attributes for 
the selected batch and the bottom grid represents the items; including 
attribute values; for the selected batch.  
At this point in time when you first log in; no clusters have been 
determined.  The first thing a user needs 
to do is select the batch they want to work on from the batch filter.  Then the user needs to review the attribute 
weightings in the top grid.  The IC 
module defaults on a weight factor of 1 for all attributes; unless the minimum 
and maximum attribute values are equal; then it sets the weights to zero.  It will be up to the user to change the 
weight factors.


## The Attribute Data Grid


To change the weight factors a user 
can select the weight factor value and type in a new value.  If a user wants to change multiple weight 
factors for multiple attributes in a single step; select all the attributes and 
right click to obtain the weight factor editing menu.


There are 3 choices for weight 
values for each attribute including:


Weight 
Factor – this is the overall weight factor; if set to zero; the attribute will 
have no bearing on distance calculations; regardless of other weight values


Weight Null 
– for attributes that have a lot of empty fields; but are important; to avoid 
penalties to distance for the attributes with blank values; you can set this 
value to 0.  That way an item doesn’t get 
penalized for distance when it has a blank attribute value.


Weight Neg – 
if attribute values are negative; this weight factor is applied to help 
normalize the distance calculation.  See 
the information on absolute and relative below to understand further.


  
In addition to displaying the weight 
factors in the top grid; there are also other fields that display important 
information; including:


Critical – 
if this box is check the attribute will appear on the left side of the lower 
grid; so it can be more easily viewed


Occurrences 
– shows the number of occurrences where there is an actual value entered for an 
attribute.  If the number of occurrences 
is 0; you might want to set a zero weight factor since this attribute has no 
data.


Minimum and Maximum – this fields display the smallest and largest value 
for numeric data or for strings it shows the range of data expressed 
alphabetically


Base UOM – 
in order to compare numeric data for a numeric attribute; the data has to be 
normalized or converted to s single UOM called the base UOM.  The IC has to convert data so that it can be 
analyzed properly  
  
 
Note: most of these fields can me sorted including the weight factor fields; 
which may make it easier to use the application.


As displayed above; the right click 
menu provides 5 options for the user to select from when editing the weight 
factors including:


Zero – sets 
all 3 weights to zero


Null Ok – 
sets the weight null to zero


Default – 
changes all settings back to the original default settings 


Absolute  - selecting Negative Weight to 0 
provides an absolute distance calculation; see example below.


Relative – 
selecting a Negative Weight other than 0 handles provides a relative distance 
calculation where either the reference value or test value maybe negative; see 
example below.


### 


### Absolute Example


To call for 
absolute distance calculation for, set the Negative Weight = 0.


DistanceContribution 
= Weight \* |ReferenceValue – TestValue|


 




Examples




<table border="1" cellpadding="0" cellspacing="0" class="MsoTableGrid" style="border-collapse:collapse;border:none;mso-border-alt:solid windowtext .5pt; 
 mso-yfti-tbllook:480;mso-padding-alt:0in 5.4pt 0in 5.4pt;mso-border-insideh: 
 .5pt solid windowtext;mso-border-insidev:.5pt solid windowtext"><tr style="mso-yfti-irow:0;mso-yfti-firstrow:yes"><td style="width:95.95pt;border:solid windowtext 1.0pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="128"><p class="MsoNormal">Reference 
  Value<p></p></p></td><td style="width:90.2pt;border:solid windowtext 1.0pt; 
  border-left:none;mso-border-left-alt:solid windowtext .5pt;mso-border-alt: 
  solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="120"><p class="MsoNormal">Test 
  Value<p></p></p></td><td style="width:92.15pt;border:solid windowtext 1.0pt; 
  border-left:none;mso-border-left-alt:solid windowtext .5pt;mso-border-alt: 
  solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="123"><p class="MsoNormal">Weight<p></p></p></td><td style="width:82.25pt;border:solid windowtext 1.0pt; 
  border-left:none;mso-border-left-alt:solid windowtext .5pt;mso-border-alt: 
  solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="110"><p class="MsoNormal">Negative 
  Weight<p></p></p></td><td style="width:82.25pt;border:solid windowtext 1.0pt; 
  border-left:none;mso-border-left-alt:solid windowtext .5pt;mso-border-alt: 
  solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="110"><p class="MsoNormal">Distance 
  Contribution<p></p></p></td></tr><tr style="mso-yfti-irow:1"><td style="width:95.95pt;border:solid windowtext 1.0pt; 
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="128"><p class="MsoNormal">10<p></p></p></td><td style="width:90.2pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="120"><p class="MsoNormal">7<p></p></p></td><td style="width:92.15pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="123"><p class="MsoNormal">0.5<p></p></p></td><td style="width:82.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="110"><p class="MsoNormal">0 (must 
  be 0)<p></p></p></td><td style="width:82.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="110"><p class="MsoNormal">1.5<p></p></p></td></tr><tr style="mso-yfti-irow:2;mso-yfti-lastrow:yes"><td style="width:95.95pt;border:solid windowtext 1.0pt; 
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="128"><p class="MsoNormal">10<p></p></p></td><td style="width:90.2pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="120"><p class="MsoNormal">13<p></p></p></td><td style="width:92.15pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="123"><p class="MsoNormal">0.5<p></p></p></td><td style="width:82.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="110"><p class="MsoNormal">0 (must 
  be 0)<p></p></p></td><td style="width:82.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="110"><p class="MsoNormal">1.5<p></p></p></td></tr></table>

### Relative 
Example


NegativeWeight 
must be non-zero.  NegativeWeights less 
than 0 are untested.


When 
ReferenceValue > TestValue


            DistanceContribution = Weight \* ( |ReferenceValue| / |TestValue| - 1)


When ReferenceValue 
< TestValue


            DistanceContribution = Weight \* 
(|TestValue| / |ReferenceValue| - 1)


We handle this 2 different ways to assure symmetry, such that the 
distance between the ReferenceItem and the TestItem is the same as the distance 
between the TestItem and the ReferenceItem.  
When either the ReferenceValue or the TestValue is negative (but not 
both), the Negative Weight also adds to the DistanceContribution.


 




Examples:




<table border="1" cellpadding="0" cellspacing="0" class="MsoTableGrid" style="border-collapse:collapse;border:none;mso-border-alt:solid windowtext .5pt; 
 mso-yfti-tbllook:480;mso-padding-alt:0in 5.4pt 0in 5.4pt;mso-border-insideh: 
 .5pt solid windowtext;mso-border-insidev:.5pt solid windowtext"><tr style="mso-yfti-irow:0;mso-yfti-firstrow:yes"><td style="width:95.95pt;border:solid windowtext 1.0pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="128"><p class="MsoNormal">Reference 
  Value<p></p></p></td><td style="width:90.2pt;border:solid windowtext 1.0pt; 
  border-left:none;mso-border-left-alt:solid windowtext .5pt;mso-border-alt: 
  solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="120"><p class="MsoNormal">Test 
  Value<p></p></p></td><td style="width:92.15pt;border:solid windowtext 1.0pt; 
  border-left:none;mso-border-left-alt:solid windowtext .5pt;mso-border-alt: 
  solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="123"><p class="MsoNormal">Weight<p></p></p></td><td style="width:82.25pt;border:solid windowtext 1.0pt; 
  border-left:none;mso-border-left-alt:solid windowtext .5pt;mso-border-alt: 
  solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="110"><p class="MsoNormal">Negative 
  Weight<p></p></p></td><td style="width:82.25pt;border:solid windowtext 1.0pt; 
  border-left:none;mso-border-left-alt:solid windowtext .5pt;mso-border-alt: 
  solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="110"><p class="MsoNormal">Distance 
  Contribution<p></p></p></td></tr><tr style="mso-yfti-irow:1"><td style="width:95.95pt;border:solid windowtext 1.0pt; 
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="128"><p class="MsoNormal">1000<p></p></p></td><td style="width:90.2pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="120"><p class="MsoNormal">1500<p></p></p></td><td style="width:92.15pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="123"><p class="MsoNormal">0.5<p></p></p></td><td style="width:82.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="110"><p class="MsoNormal">1<p></p></p></td><td style="width:82.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="110"><p class="MsoNormal">0.25<p></p></p></td></tr><tr style="mso-yfti-irow:2"><td style="width:95.95pt;border:solid windowtext 1.0pt; 
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="128"><p class="MsoNormal">1500<p></p></p></td><td style="width:90.2pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="120"><p class="MsoNormal">1000<p></p></p></td><td style="width:92.15pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="123"><p class="MsoNormal">0.5<p></p></p></td><td style="width:82.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="110"><p class="MsoNormal">1<p></p></p></td><td style="width:82.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="110"><p class="MsoNormal">0.25<p></p></p></td></tr><tr style="mso-yfti-irow:3"><td style="width:95.95pt;border:solid windowtext 1.0pt; 
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="128"><p class="MsoNormal">1000<p></p></p></td><td style="width:90.2pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="120"><p class="MsoNormal">-1500<p></p></p></td><td style="width:92.15pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="123"><p class="MsoNormal">0.5<p></p></p></td><td style="width:82.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="110"><p class="MsoNormal">1<p></p></p></td><td style="width:82.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="110"><p class="MsoNormal">1.25<p></p></p></td></tr><tr style="mso-yfti-irow:4;mso-yfti-lastrow:yes"><td style="width:95.95pt;border:solid windowtext 1.0pt; 
  border-top:none;mso-border-top-alt:solid windowtext .5pt;mso-border-alt:solid windowtext .5pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="128"><p class="MsoNormal">1500<p></p></p></td><td style="width:90.2pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="120"><p class="MsoNormal">-1000<p></p></p></td><td style="width:92.15pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="123"><p class="MsoNormal">0.5<p></p></p></td><td style="width:82.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="110"><p class="MsoNormal">1<p></p></p></td><td style="width:82.25pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  mso-border-top-alt:solid windowtext .5pt;mso-border-left-alt:solid windowtext .5pt; 
  mso-border-alt:solid windowtext .5pt;padding:0in 5.4pt 0in 5.4pt" valign="top" width="110"><p class="MsoNormal">1.25<p></p></p></td></tr></table>

 




Once a user has set all of the 
weight factors for the first time; they will need to save their settings by 
selecting the **save button**.  Next time they enter an IC session for that 
same batch; the settings should appear as you saved them.


### 


### Setting 
Neighbor Distance


Setting the neighbor distance is 
typically an iterative process.  The 
neighbor distance serves as a sensitivity factor; the smaller you make this 
number typically the smaller the clusters you end up with.  Conversely the larger the neighbor distance 
the larger the clusters.  Once the 
neighbor distance has been set; a user can now select Calculate to view their 
first clusters.  See a typical output 
below.  If you notice the 
items in bold represent the largest cluster in your batch where the first item 
in the list is the **center of the largest 
cluster**.   The size of the 
cluster is determined by the number of neighbors which is contained in one of 
the columns of data.


### Selecting 
Calculate


When you select calculate it 
identifies the items with the most neighbors; highlighting the largest cluster 
in bold.  To see all the neighbors in the 
largest cluster (in bold); sort on the distance column; it will group the 
largest cluster to the top.  Calculate 
will also shade the items with a 0 Weight Factor and place them to the right 
hand side of the grid.  The time stamp 
displays the last time calculate was selected.


### Selecting 
Auto-Calculate


When you select auto-calculate; 
every time you make a change to the neighbor distance it will update the main 
item grid based on the new neighbor distance.  
If you have a batch size under 1000 or 500 items; you might want to have 
this function checked.  For larger 
batches; it may take longer for the grid to redisplay to reflect your changes; 
it’s a user preference on what to do with this feature.  When ever you make changes to the attribute 
weighting; the data is automatically updated in the lower grid to reflect this 
change; independent of the auto-calculate setting.  Auto-calculate only works 
with the neighbor setting.


## 


## The Item Data Grid


If you notice there is a distance 
column; this column shows the distance between neighbors.  This value is calculated based on the 
attribute values for an item and the weight factors.  If the distance is zero; that means the item 
is an exact duplicate to the center item.  
As you can see in the cluster above; there are five items with a distance 
of zero which means there are five duplicates based on the weight factors you 
have set.


To view what values contribute to an 
items distance; you can right click on a value and view the distance 
calculations.  Please be careful **not to select** the item first; then you 
will end up selecting a new center for a cluster.  This process is a little tricky and will take 
a little time to get used to how to manage this lower grid.  
  



### String Attributes 
Distance


The distance calculations work 
differently for string data versus numeric data.  For example; is a string attribute has a 
weight factor of 1 and if an item has a different string value than the center 
item for the cluster; the penalty for the distance is 1 (1 X weight 
factor).  If numeric values with units of 
measure; the distance calculation is done differently.  Weight factors for numeric attributes are 
described in the following section.


### Numeric Attributes 
Distance


The 
distance calculations on numeric attributes are of a linear calculation that 
scales with the difference between values.  
A simple example; if your reference value for a numeric is 1 and the 
neighbor item value is 2; then the distance penalty is 1 (2-1=1).  If your reference value for a numeric is .250 
and the neighbor item value is .260; then the distance penalty is .01 
(.26-.25=.01) (assuming absolute with a weight factor of 1).  For small decimal values that have small 
differences between the reference item and the neighbor items; it’s recommended 
to increase the weighting factor to better account for the differences.


### Keeping 
distance calculations simple all costs


Use absolute 
for all numeric values.  The price of 
simple is that the distance between a 1 1 uF vs 2 uF 
capacitors will be 1000 times more than the distance between a 1 pF vs 2pF 
capacitors.


### Keeping 
distance calculations simple but realistic


Use the 
default (right click menu) for numeric values.  
This picks absolute vs relative computation for a numeric value based on 
it’s value range.


### Leaving 
simple behind


Imagine you 
have electric motors ranging from 50 rpm to 1800 rpm, but left handed rotation 
is modeled as a negative value.  Is 1800 
rpm vs -1800 rpm more different (thus modeled as a greater distance) than 1800 
vs 50 rpm.  Probably 1800 rpm vs -1800 rpm is a trivial difference.  For such cases, the negative weight factor 
for the motor speed would be a very small value say 0.01, but not 0.


Temperatures 
are another case, since most measurement units for temperature have a zero 
value arbitrary zero value.  The default 
logic will probably lead to a relative temperature weighting when absolute 
weighting might make more sense.  CDS is 
considering modifying the default logic for temperatures or changing the base 
UOM to Kelvin.


 




In order to prevent the same item 
from appearing the multiple clusters; the user has the option to create a 
cluster.  If you right click on the center 
item of a cluster; you will be presented with the option to create a cluster as 
shown below.  Once a cluster is created; 
you will noticed if you scroll to the bottom of the cluster using the vertical 
scroll bar; that at the end of the cluster the distances go up by a much large 
value.  The cluster distance is set in 
the upper grid; the default is 1000.  
It’s recommended to keep this value large to avoid having the same item 
appear in multiple clusters; if that is your intention.  


Once a cluster has been created; it 
can be removed or deleted from the data all together.  By selecting remove cluster; you will notice 
the distance values go back to a normal setting outside the cluster.  Note you need to select save to save your 
cluster; otherwise if you go to another batch without saving; your cluster will 
disappear.


Remove cluster item – removes 1 item 
from a cluster; next time you export the deleted item will not appear in the 
cluster.


Delete cluster – deletes the entire 
cluster; it doesn’t delete the data just the cluster name.  Next time you export; the deleted cluster 
will not appear in the export file; unless its 
highlighted in bold.


### Recent 
Selections


### Recent selections allows users to 
quickly navigate to past item selections.  
Every time you select an item in the grid; it gets recorded in this 
menu.  This data is only stored during 
your IC session; if you close the IC and log back in this field clears 
out.  This make’s it easier to remember 
where you may have left off as your analyzing the data in your session.


### Exporting 
Clusters


Exporting clusters can be 
accomplished by selecting the export button; the items in bold will be exported 
once you select this.  Once you export 
the cluster 4 files are created.  One of 
the files is called the batch\_name\_items.txt; this file represents the data in 
the lower grid for just the cluster in bold text.  


The other 2 files that are exported 
include the batch\_name\_attrs.text and the batch\_name\_cxp.xml file.  The attrs export file shows the weight 
settings for each attribute for the cluster that was exported.  The XML file is used for other applications 
only.  To find the export files for the 
Item Cluster application; look in your DFR program files directory; typical 
path: C:\Program Files\Convergence Data Services\CDS Toolset v3.5\Clusters.


When you export data a second time 
the previous export file gets replaced by a new export file that will now 
contain both clusters that you have exported.  
In order to differentiate between clusters; sort the data by the cluster 
name like the example above.  The items 
highlighted in yellow are in a different cluster than those that are not 
highlighted.  Unless you delete a cluster 
it will continue to show up in your export files.


Exports works for both clusters and 
items highlighted in bold that might not be set as a cluster.  Future exports only export named clusters in 
addition to the data you have selected for export.  If you don’t want a named cluster to appear 
in your export file; you can remove that cluster and next time it will not be 
exported; unless you purposely select it.  
The following example shows the type of information that appears in an 
export file; including batch name, neighbor distance and all of the attribute 
values for your past clusters.


Exporting attributes (batch name\_attrs.txt) 
works a little differently.  This file 
only contains the attribute weightings for the most recent export file.  This file gets replaced with each export that 
is done.  


**Sharing XML Files**


There are 2 XML files that are also 
created with each export including: Batch\_Name\_cxp.xml and Batch\_Name.xml.  The cxp xml file is for feeding data to 
strategic sourcing applications; please ignore this file.  The other xml file; called batch\_name.xml; 
represents the data generated for your particular batch which includes all of the attribute and distance settings.  Since the Item Cluster module creates 
information locally; the only way for other users to share data is to share 
this XML file.


**Tips for Using the IC application:**


1.)     
To 
get a new cluster to appear at the top of the grid other than the largest 
cluster; select the center item of interest and select the distance column 
heading to sort the data to the top of the grid.  
  



2.)     
When 
checking individual distance calculations for items in a cluster; avoid 
selecting the item of interest; just right click on it to view the distance 
details.  
  



3.)     
Make 
sure your export files are closed when you do subsequent exports; otherwise you 
will get a warning and you will not be able to export.  
  



4.)     
If 
you want to save the export files for an extended period; same them under a 
different name and location since they will be replaced in subsequent exports.  
  



5.)     
Make 
sure your data has been thoroughly cleansed and validated and approved prior to 
creating any clusters.  If the data has 
errors your clusters will be invalid.  
  



6.)     
Try 
sorting your attributes by occurrence count and for all the attributes with a 
low occurrence count, set Wight Factor to zero.  
  



7.)     
Use 
the set cluster function to avoid obtaining the same item in multiple 
clusters.  Its recommend to set the 
cluster attribute weighting to a high number like 1000 to help differentiate 
items that are in a cluster.  
  



8.)     To remove a cluster; sort the item 
numbers; match an item number with the cluster name; sort to the top and right 
click to remove cluster.  
  





