



Best\_Practices\_\_Setting\_up\_Abstract\_Classes - Design For Retrieval (DFR) Help



# Setting up Abstract Classes


 


## When to use Abstract Classes![](assets/image(1001).png)


 


This can group together multiple classes that have a common item. This allows you to search across multiple classes in these areas


These have to be EXACT MATCHES however. If anything differs in the attributes, this will cause issues.


 


## When to use Groups ![](assets/image(1000).png)


Groups in Teamcenter are used to group similar items into easily identifiable sectors of data


They may or may not share attributes, but you would likely not need to search for them together.


Example:


Fasteners. This can cover a large area of items that may not be comparable, but grouping them by function allows them to be more easily navigated in Teamcenter


 


## Storage Classes in Teamcenter![](assets/image(1002).png)


A Storage Class in Teamcenter is the lowest level of the Classification Tree. It contains the Items, and manages the Attributes that show, are required, etc.


The Attributes that are defined on this Storage class, and any Abstract Classes above it make up the full range of available attributes for any Item classified here. 


 


## Managing Abstract Classes in CDS PIM


In order to set up an Abstract class in CDS PIM, you need to set the property of isAbstract to True on a given Parent Category. This attribute will only work on a parent category, and setting it on a leaf node will cause issues when you try to do any exports.


Abstract classes require that any attribute they have is also on any child class. Therefore in CDS PIM you must make sure that all of the child classes not only have an attribute with the same name, but it must have the same TC\_ID as well. 


For more on matching attributes, please see the Defining Attributes for Teamcenter Page [(Click Here)](#)


A common issue you may encounter is if these are not matching in your items export, there will be attributes with blank entries.


 


## Combined Attributes


In order to have attributes combine, they must be identical in a number of ways. 


They must have:


1) the same name


2) the same type


3) match in the information of Key, DNA, and Mandatory


4) If the attribute is linked to an LOV in any of the Categories it appears in, it must be linked to that LOV in all areas.


 


 


## Differing LOVs


If the LOVs don't match, you can either remove the LOVs , change the Attribute names, or consolidate the LOVs


1) Remove the LOVS - You can remove the LOVs from all of the attributes. This will allow them to be combined, but there is the obvious drawback of losing the LOVs


2) Separate the Attributes- you can instead break the attributes out to be named differently, so they can be easily identified.


Example . Material could become something more specific, such as "Fastener Material" or "Metallic Material"


3) Consolidate the LOVS - you could combine all the LOV lists into one and assign it to all of the involved Attributes.


This will create a longer list, but also, you will only have 1 list to manage on a go forward basis. Depending on your specific data, this may or may not be the right solution for you.


 


## Common Problems You May Encounter


- Mismatched IDs


Check to make sure the ID haven't been manually assigned. This will create issues if they are assigned separate numbers. 


- LOVs, Required, Key DNA flags to check


As mentioned above, if there are differences on an attribute of the Key, Mandatory and DNA flags, the attributes will be broken out. 


 



