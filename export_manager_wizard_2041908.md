



Export\_Manager\_Wizard - Design For Retrieval (DFR) Help




**Item 
Data Export**


 


After selecting the export type and specifying the options you 
want, the first screen you will be presented with is the *Attribute Filter 
Screen* (Figure 1). 


 


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/em_items_files/image003.jpg)




**Figure 1**


 


**Attribute Filter Selection**


 


There are three tabs on this page that allow the user to filter 
the data that will be exported.


 


The first is Attribute Group Selection. This tab shows all 
attribute groups that belong in the system. The user may check any box (or use 
the “check all” box in the column header to auto-select all attribute groups). 
A filter box at the top of the page allows the user to search attribute groups 
names on a “contains” basis (i.e., searching for “At” will return all 
attribute groups whose name has the “at” character combination). Selecting an 
attribute group will ensure that any attributes that belong to that group will 
be exported.


 


The second is Attribute Status Selection. This tab shows all 
statuses supported by the system. The user may check any box desired (or use 
the “check all” box in the column header to auto-select all attribute statuses; 
note that having no statuses selected or have all statuses selected means the 
same thing to the export – all statuses will be included). The status selection 
is an “and” operation for attribute filtering, so any attribute that doesn’t 
meet the status selection will not be included in the export.


 


The third tab is Individual Attribute Selection. This tab shows 
all master attributes in the system. Notice that some attributes may already be 
selected if Attribute Groups or Attribute Statuses are already checked. These 
attributes will be included in the export unless the user unchecks them. Any 
additionally checked attributes must still pass the group and status filters in 
order to be exported. Using the “check all” box in the column header will 
select all attributes, though individual attributes, again, must still meet any 
group and status filters in order to be exported. A filter box at the top of 
the page allows the user to search individual attribute names on a “contains” 
basis, just as the Attribute Group page.


 


Please note that these selections are all “and” operations; this 
means that if you select an attribute status and an attribute group, you will 
have all attributes that both belong to that attribute group and have that 
attribute status in your final exported file. Selecting nothing on all tabs 
will result in no attributes being filtered from the export.


 


Once the Attribute selections meet the user’s requirements, click 
the Next button to proceed to Category selection (Figure 2).


 


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/em_items_files/image001.jpg)




**Figure 2**


 


 


**Category Selection**


 


The 
Category selection screen works much like the Attribute selection page. There 
are three tabs that allow the user to filter their selection down for the items 
export.  Items will only be exported from the part of the classification 
structure selected.


 


The first tab 
is Category Selection. This will show two panels, one being the category 
structure in the system in a tree view, the other being a panel labeled 
“Attribute”. In the upper panel, you can search for categories by name in the 
“Category Name Search” box to perform a “contains” search. Note that any 
categories down the tree that match this criterion will be included, even if a 
higher-level category doesn’t. For example, if you search for “Screws”, the 
“Parts” category will show because one of its descendent categories matches, 
even though it doesn’t itself. Checking any box in the tree will select that 
entire subtree; to remove categories from being exported, the user can navigate 
down the tree and remove any undesired categories. Note that categories in the chosen 
subtree must meet any Category Status selections in the status  tab in 
order to be exported.


 


The second 
tab is Category Status Selection. This will show all statuses supported by the 
system. Check statuses individually or by using the “check all” box in the 
column header to select or deselect all at once. Note that having no statuses 
selected here is the same as having all statuses selected when exporting 
category definitions.   
  
 
The third tab is Category Attribute Status Selection. This will show all 
statuses support by the system. Check statuses individually or by using the 
“check all” box in the column header to select or deselect all at once. Note 
that having no statuses selected here is the same as having all statuses 
selected when exporting category attributes.


 


Please note 
that all these selections are “and” operations; this means that if you select a 
category status, a category attribute status, and a part of the classification 
tree, then you will have all category definitions in that subtree that have 
that category status, and all category attributes that belong on that category 
that have that category attribute status. Selecting nothing on all tabs results 
in no category and no category attribute definitions exported in the final 
file.


  
 
The lower panel will show attributes that belong to a category that is clicked 
in the tree in the upper panel. The view of these attributes can be changed in 
the dropdown just above the grid. Note that any master attribute selections 
will limit the category attributes that are viewed and exported – if you only 
want attributes from a certain group exported, then only category attributes 
that belong to that group will be exported as well.


 


***Auto Select 
Category Attributes****:*  With this checked, the 
system will auto select all category attributes automatically when you select a 
category.  If this option is not selected, then you will have to select 
what attributes you want to export manually.


 


Once the user has selected the 
category subtree to export and the desired category and category statuses, 
click the *Next* button to continue to batch selection (Figure 3).


 


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/em_items_files/image002.jpg)




**Figure 2**


 


 


**Batch Selection**


 


The batch selection 
screen allows the user to further filter the results by batches of items.  If 
no batches are selected, then items will not be filtered by any particular 
batch. A filter box at the top of the page allows the 
user to search individual batch names on a “contains” basis.


Once the 
user has selected (or not selected) any batches click *Export* to be begin 
the export process.


 


 


Return 
to [**Export Manager**](EM.md)  page




