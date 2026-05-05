



Editing\_the\_Data - Design For Retrieval (DFR) Help




**Viewing 
Road Map Data**



A user can click on any variant-year item and view the 
associated data for that particular year as shown below.  Some of the fields 
are editable while other fields will be read in from other systems.  The 
attribute fields that are displayed in this view come from the data model in 
DFR.  If a user changes the data model in DFR, they will be able to changes 
these fields.


## ![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/IM-View_Road_Map_files/image001.gif)

![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/IM-View_Road_Map_files/image002.gif)

 ![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/IM-View_Road_Map_files/image003.jpg)



**Module variant item details tab in DFR Item Mapping tool.**



Currently the component data shown on the right side of the 
graphic above is read in from parts and BOM’s as read only data that cannot be 
edited here.  It is anticipated that some of the ERP type data e.g. cost, EAU, 
etc. will also be read in from another Whirlpool data source, making it read 
only.


 


The EAU and Unit Cost attributes are calculated values.  The 
user manually enters the regional EAU and Unit Cost data in the bottom grid.  
The EAU data total is displayed at the top of the item details page along with 
a weighted total for Unit Cost.


 


The formula for the calculated values for EAU and Unit Cost:


 


EAU – sum of each region at the bottom


Unit Cost – (EAUxUnit Cost) sum for all regions divided by 
total EAU\*


 


\*If data is missing for region then it is not included in 
the calculations.


## 


### 


### Header and Tab Information


 


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/IM-View_Road_Map_files/image004.jpg)





**Remarks field for a road map appears at the top along 
with the file path for what-if maps.**


 


The remarks field is currently a work in progress.  We will 
have to work out what information we want to be shown here.  Here are some 
potential fields:


 


- Name of road map
- Name of editor and creator
- Date of last change and creation date
- Path to loaded “what-if” file (show file name as well)
- Notes on change history

 


 


Currently there are three tab pages in the mapping tool:


 


Item Map Layout – Displays the road map for a loaded module 
or component type road map.


 


Properties – Describes important information on the road map 
including: associated information e.g. module set, remarks, high level metric 
summary, etc.


 


Item Details – Displays the details for an item on the road 
map.  This is where users can view specific data for an individual module 
variant or component.




*![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/IM-View_Road_Map_files/image005.jpg)*


**Properties tab will display additional summary data for a 
road map.**




![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/IM-View_Road_Map_files/image006.jpg)




**Variant and EAU summary information for each year is 
displayed at the top.**



![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/IM-View_Road_Map_files/image007.jpg)




**Example of Module, Variant and EAU calculations**




For every column in the Item 
Mapping Layout view, there are numbers under each year.  Here is the key for 
this data:


 


#M – number of modules for a 
colmn (year)


#V – number of variants for a 
column (year)


V/M – variant to module ratio


EAU – total EAU for a column 
(year) 


 


 


Return 
to [Item 
Mapping](IM-Item_Mapping.md)




