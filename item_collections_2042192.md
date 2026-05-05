



Item\_Collections - Design For Retrieval (DFR) Help



**Item Collections**


 


An attribute may have more than one legitimate value for an individual item in the database. Several examples of common collections could include: images that are associated with the item; manufacturers or manufacturer's part numbers that correspond to the internal part number for an item; people who worked on the design team for an item; or, a bill of materials for an assembly.


 


A collection of items is created by defining a specific type of attribute with the data type of "Items." The Items attribute can have several values, each of which will point to an item located in the database. Each of these collection items may have a set of relationship attributes which describe it. The diagram below illustrates the concept of Item Collections.


 


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/images/Help - Collections Chalk Talk 2.jpg)




 


The values associated with the Items collection attribute, refered to as "members" of the collection, can have properties associated with them. In the example below, the Component Items collection attribute has a property of "RelAttribGroup", or Relationship Attribute Group. The RelAttribGroup property has attributes associated with it that describe the component memberships' relationship to the Fastener item.


 


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/images/Help - RelAttribGroup Chalk Talk 2.jpg)




 


Each member of the collection, as well as the item that has a collection relationship with the members, must have an item in the classification. The diagram below illustrates the location of each in the classification.


 


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/images/Help - Collections Chalk Talk class tree.jpg)




 


Item Collections are managed in the Classification Manager, the Attribute Manager and the Item Browser Tools. For more information about how to create and use Item Collections, review the following topics:


 


[Create an Items Collection Attribute](javascript:popuplink('hs8100.htm'))


 


[Assign an Items Collection Attribute to a Category](javascript:popuplink('hs8300.htm'))


 


[Define a Group of Attributes about the Relationship](javascript:popuplink('hs8200.htm'))}


 


[Assign Members to an Item Collection](javascript:popuplink('hs8400.htm'))


 


[Add Values to Item Collection Relationship Attributes](javascript:popuplink('hs8500.htm'))


 


 


Return to [Item Browser](hs6000.md).


  





