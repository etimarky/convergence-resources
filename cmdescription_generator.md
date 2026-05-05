



CMDescription\_Generator - Design For Retrieval (DFR) Help




**Building a Description Template**


 


To build a description template the Description Generator is 
used.  The Description Generator is located on the Category Processing tab 
in Classification Manager.  The category processing action **Description 
Generator** is used to configure all the templates for that category. A 
description template consists of a target attribute and a combination of text, 
attribute data, and conditional statements.  The attribute names and/or 
values will be organized in the target attribute when a description is 
generated.


 


**![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/CM-Description_Generator_files/image001.jpg)**




**To create a new description template:**


 


1. Select a category 
 in category tree on the left where the template will be 
 created.
2. Make sure that the 
 Configure radio button is selected
3. Click the “Add” 
 icon ![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/CM-Description_Generator_files/image002.jpg)

 to add a new 
 template
4. Place your cursor 
 in the Template Name box and type a name for the template
5. Select the lower 
 window.
6. Select a target 
 attribute by selecting the attribute in the name column.
7. Select the **Insert** button and select **Target**.  This is the attribute where the 
 result of the processing will be placed.
8. To add the name of 
 an attribute to the template, select the position of the attribute name in 
 lower template window.
9. Select the 
 attribute in the name column.
10. Select the insert 
 button and select name.

11.    This will 
insert the name into the template.  You can also add your own separators 
such as a comma or semicolon.  


12. An attribute value 
 can be added in a similar manner by selecting insert value.
13. Save the template 
 before selecting the Run radio button by clicking the ![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/CM-Description_Generator_files/image003.jpg)

.

 


Description Generator allows for [Conditional logic](CM-Description_Generator_IfThenElse.md).  


 


The keys for the Description Generator Template are as follows:


 


TA: = Target Attribute


AN: = Attribute Name


AV: = Attribute Value


AP: = Attribute Name / Attribute Value


AVU: = A Value with a Unit of Measure


AVUWC: = A value with a specified Unit of Measure – a conversion 
to that unit will automatically be applied during description generation.


 


The Operators for the Description Generator Template are as 
follows:


 


==        (equals)


!=         (not equals)


&&        (and)


||           (or)


 


The Operations for the Description Generator Template are as 
follows:


 


·         
IF 


·         
ELSE


·         
AND/OR


 


The sample template below would put the Noun, Modifier, Shaft 
Diameter and UOM in the NOTES attribute for each item in the selected category.  
NOTE: the AVUMC takes an additional input parameter, this is the desired Unit 
of Measure (see below for example syntax):


 


<TA:NOTES> <AN:NOUN>, <AV:MODIFIER>, <AVUWC:SHAFT 
DIAMETER:ft>


 


NOTES


NOUN 1234 Bullet, Mill, 12IN, 1FT


NOUN 2456 Bullet, Mill, 18IN, 1.5FT


NOUN 2342 Bullet, Mill, 6IN, .5FT


 


**Additional 
keys** for the description generator include the following fields that 
are not listed in the attribute list.


<TD> indicates that the target is the Item Description 
system attribute. The sample template below would put the Noun, Modifier, 
Shaft Diameter and UOM in the Item Description attribute for each item in the 
selected category:


 


            i.e.:  <TD>  <AN:NOUN>, <AV:MODIFIER>, 
<AVU:SHAFT DIAMETER> 


            


Item Description


NOUN 1234 Bullet, Mill, 12IN


NOUN 2456 Bullet, Mill, 13IN


NOUN 2342 Bullet, Mill, 5IN


            


**Note**:  The user 
can enter free text to be inserted into the Item Description.  <TD> Test 
Description would result in ‘Test Description’ being inserted as the value of Item 
Description for all items in the batch.


 


 <NN> adds the Item Number to the generated string. 


            i.e.:  <TD>  <AN:NOUN>, <AV:MODIFIER>, 
<AVU:SHAFT DIAMETER> <NN>


 


<LL> adds the Legacy Part Number to the generated string. 


            i.e.:  <TD>  <AN:NOUN>, 
<AV:MODIFIER>, <AVU:SHAFT DIAMETER> <LL>


 


<QQ> adds the full qualifier path to the generated string.


            i.e.:  <TD>  <AN:NOUN>, <AV:MODIFIER>, 
<AVU:SHAFT DIAMETER> <QQ>


 


The following tokens have an optional parameter that can be added 
to the end of the token to specify the default number of decimal places to use 
in the case that the attribute is a numeric; AV, AP, AVU, and AVUWC.


 


The following example demonstrates setting the Shaft Diameter value 
limited to 3 decimal places.


Example:


            <TA:NOTES> <AN:NOUN>, <AV:MODIFIER>, 
<AVUWC:SHAFT DIAMETER:ft:3>


 


When specifying the decimal places you can specify how the 
overflow is handled by appending a T or an R to the number. 


 


            T = Truncate value, which drops all the additional 
decimal place values after the number specified


            R = Round, which rounds away from zero for all numbers 
5 and higher


 


Example:


            <TA:NOTES> <AN:NOUN>, <AV:MODIFIER>, 
<AVUWC:SHAFT DIAMETER:ft:3T>


 


If the template does not specify a handling of the overflow 
decimal places, the description generator rounds by default.


 


Now that the template is saved, the user is ready to run an 
update.  


 


**To run a description template:**



**![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/CM-Description_Generator_files/image004.jpg)**


 


 


1. Select the Run 
 radio button.
2. You can select any 
 template here from the Template Name dropdown box.
3. Select the batch 
 to update from the batch drop down.
4. Select the status 
 of the items to update.  There are 2 choices including In-work only or 
 In-work, pending, approved.
5. Restrict to my 
 items only will be checked as default option.  See DFR Help Description 
 Generator Assigned Items Only.  User will only be able to update items 
 assigned to them.
6. Click the Run 
 button and the Description Generator will identify how many records were 
 updated.

 


 


 


Return to [Using the Description Generator](CM-Using%20Description%20GeneratorMenu.md) 


 


 




