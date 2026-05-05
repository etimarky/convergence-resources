



Using\_Description\_Generator - Design For Retrieval (DFR) Help



**Using Description Generator**


 


The category processing action **Description Generator**, defines how the attribute names and/or values will be organized in the target attribute when a description is generated.  The target attribute is the attribute where the attributes and values will be placed when the description generator is run.


 


**To create a description template:**


 


- Select a category in category tree on the right where the template will be created.

 


- Select the lower window.

 


- Select a target attribute by selecting the attribute in the name column.

 


- Select the **Insert** button and select **Target**.  This is the attribute where the result of the processing will be placed.

 


- To add the name of an attribute to the template, select the position of the attribute name in lower template window.

 


- Select the attribute in the name column.

 


- Select the insert button and select name.

 


This will insert the name into the template.  You can also add your own separators such as a comma or semicolon.  


 


- An attribute value can be added in a similar manner by selecting insert value.

 


The keys for the Description Generator Template are as follows:


 


TA: = Target Attribute


AN: = Attribute Name


AV: = Attribute Value


AP: = Attribute Name / Attribute Value


AVU: = A Value with a Unit of Measure


 


The sample template below would put the Noun, Modifier, Shaft Diameter and UOM in the DESCRIPTION attribute for each item in the selected category:


 


<TA:DESCRIPTION> <AN:NOUN>, <AV:MODIFIER>, <AVU:SHAFT DIAMETER> 


 


ITEM  DESCRIPTION


1234 Bullet, Mill, 12IN


3423 Bullet, Mill, 13IN


2342 Bullet, Mill, 5IN


 


Return to [How to Build a Classification](hs1200.md)





