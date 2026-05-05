



Using\_Properties\_to\_Control\_the\_Behavior\_of\_Item\_Collections - Design For Retrieval (DFR) Help



**Using Properties to Control the Behavior of Item Collections**


 


Attribute properties are used to define the way that Item Collections behave.  There are two system-defined properties: RelAttribGroup and ConstrainingCategory.


 


- The **RelAttribGroup** attribute property is used to tell the application what attributes are assigned to item collection attributes.  Attributes with a data type of Items with Properties can have a value for the property RelAttribGroup.  This value is always the name of an attribute group.  The attribute group defines the group of relationship attributes for this collection attribute.

 


- The **ConstrainingCategory** property is used to create a relationship between an attribute with a data type of Items with Properties and a category.  In the Item Browser, when the Add Items window opens, it automatically defaults to the category path defined by the value of the ConstrainingCategory property.

