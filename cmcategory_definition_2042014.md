



CMCategory\_Definition - Design For Retrieval (DFR) Help




**Category Definition**


 


The right hand column of the Classification Manager displays 
detailed information about a particular node in the classification tree. The 
field below the Category displays the navigational path from the super-category 
through the sub-categories to the node selected from the center column.


 


The **Name** field indicates the category name or the item name 
if this is a terminal node.


 


The **Description** field contains a description of the 
category or teminal node.


 


The tabs below the description field contain detailed information 
about the item or category. This information applies to the current category 
and, depending on the [Inherit Attributes](javascript:popuplink('hs920.htm')) setting in 
subordinate categories and nodes, to each category below the current category.


 


**Attributes** list the characteristics or traits assigned to 
the category and any item subordinate to the category. These attributes are 
added to the category or item from the [Master Attribute List](javascript:popuplink('hs2751.htm')) and are 
defined in the Attribute Manager module. Values for the attributes are assigned 
to individual items when data items and their attribute values are loaded using 
the Item Loader module, or when values are manually entered in the Data 
Developer module. 


 


[**Properties**](hs2750.md) are 
additional information for a particular category. The System Administrator defines 
properties for the entire catalog, however, the Category Developer is 
responsible for assigning values to the properties. 


 


[**Responsible Users**](javascript:popuplink('hs930.htm')) lists the users 
who have access to the category and assigns certain functions to these users.


 


[**User Resources**](javascript:popuplink('hs950.htm')) are 
customizable for each catalog. This tab lists those individuals who understand 
the details of a product line and may be referred to for more information.


 


**Attachments** may be used to list reference files such as 
catalogues, documents, pictures or specification files associated with a 
category.


 


**Category Processing** allows a user to call [configuration objects](javascript:popuplink('hs1903.htm')) to perform 
specific tasks. An example of a Category Processing task is the [Description Generator](javascript:popuplink('hs2600.htm')).


 


Below the tabs are several fields that provide information about 
the creation and status of the category. The administrator for your 
installation may modify the choices in this field:


 


- [**Authorization Type**](javascript:popuplink('hs903.htm'))indicates which 
 authorizers can approve or reject a category
- [**Status**](javascript:popuplink('CM-Category_Statuses.htm')) designates the 
 condition of a category
- The **Created** fieldlists the author and the date and time when this category was created
- **Last Updated** lists the user who 
 last changed the category including date and time
- **Terminal Node** indicates whether 
 the current node is a last node in this branch of the classification. This 
 field value is "Yes" for all newly created nodes and 
 automatically toggles to "No" when a child category is created 
 below it.
- [**Inheritance**](javascript:popuplink('hs920.htm'))specifies whether 
 a node is to automatically adopt the characteristics of its parent node.
- **Remember where I 
 am when I close the application -** When this box is checked, your 
 location within the classification structure is noted prior to closing the 
 Design for Retrieval application and you are returned to that location 
 when you log in again.
- **Awaiting Approval** logs the number 
 of nodes in the classification with a status of **Pending**

 


 


 


Return 
to [Classification Manager](CM-Overview.md) 


 




