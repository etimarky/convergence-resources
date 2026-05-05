



Best\_Practices\_\_Defining\_Attributes\_for\_Teamcenter - Design For Retrieval (DFR) Help



# Defining Attributes for Teamcenter


 


## Inherited Attributes


In Teamcenter, an Inherited Attribute is an attribute that is passed down to a class from its parent class. 


This only occurs when you are using abstract classes, as Groups do not provide attribute inheritance. 


 


## Class Attributes


Abstract classes in Teamcenter support the ability for the child classes below them to inherit their attributes. 


 


## Views


Allow you to modify what attributes are seen and required in Teamcenter.


CDS PIM has the option to use views or not. 


 


## Re-using Attributes


In order for an attribute to be re-used, it must match in every way. 


Attributes must match with the Data Type, Assigned LOVs,  Mandatory, and Key


 


## LOVs


When determining if you should re-use an attribute or break it out into multiples, one of the main considerations you should make is regarding LOVs.


If it is a string Attribute with LOVs you will have to combine all the LOVs in order to consolidate the attribute. 


This may be acceptable depending on the part, and your own structure. Or it make make more sense to break out the attributes into more specific, classification based versions in order to minimum the number of items in each LOV and make them more effective. There are pros and cons to each, and each system is different. Please reach out to your CDS representative if you would like help determining which is the best for your structure.


 


 



