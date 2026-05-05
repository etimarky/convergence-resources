



DDSortingandFilteringItems - Design For Retrieval (DFR) Help




**Sorting 
and Filtering Items**



The 
Data Developer module allows the user to apply filters to columns and save 
specific filters and column configurations as views.


 


Items 
do not need to be assigned to the current user to create a view or filter.


 


Once 
you have retrieved your select set of records, to set a filter:


 


·         
Select 
an attribute you want to filter and put the mouse to the attribute label.  
Right click to bring up the menu.  Select Filter.  


·         
At 
the Region dialog box, select the Operation from the drop down, the Filter 
Value and a UOM if it applies


·         
Select 
OK to apply the Filter


 


 


To 
create a filter, right click on a column, and choose “Filter”.


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DD-Sorting-and-Filtering-Items_files/image001.jpg)




Example: 
Selecting a filter for an attribute.


 


After 
selecting Filter, the user is presented a dialog to define the filter:


 


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DD-Sorting-and-Filtering-Items_files/image002.jpg)




After 
clicking OK, only items which match the defined filter will be displayed. So, 
in this case, only items with a Shank Length of less than 2.1 inches will be 
displayed:


 


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DD-Sorting-and-Filtering-Items_files/image003.jpg)




**Example**: Displaying only 
Shanks 2.1” or less. 


*Note*: After a filter has 
been applied, the attribute is underlined.


 


You 
can add filters on as many attributes as you wish.


 


Filter 
operators include:


- Equal – filter will find an exact match
- LIKE – filter will find similar items, 
 you have to use a wild card %
- Range – typically two values with a dash 
 in the middle, works for strings and numerics e.g. 1-2
- Is Null – will filter on null fields
- Exists – will only filter on fields with 
 values
- Greater – will filter on values greater 
 than
- Less – will filter on values less than

 


 


Filters 
can be removed by right clicking the column, and choosing Clear Filter.


 


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DD-Sorting-and-Filtering-Items_files/image004.jpg)




**Example**: Removing a filter 
from an attribute column.


 


*Hint*: To remove all 
filters at once, click the “Clear All Filters” button:


 


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DD-Sorting-and-Filtering-Items_files/image005.jpg)




Example: 
Clearing all filters.


 


To 
auto-retrieve data after applying a filter, check the “Auto Retrieve After 
Filtering” option:


 


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/DD-Sorting-and-Filtering-Items_files/image006.jpg)




**Example**: When checked, data 
will automatically be retrieved and displayed in the main grid after the user 
sets a filter.


 


If this is checked, any column you filter, sort or hide will 
trigger a retrieval of the data.  If you uncheck this option, you can set 
multiple filters, hide columns and sort and no retrieval will occur until you 
manually select retrieve.  Please note that the grid clears after the first 
column filter you set and will not restore with items until you select 
retrieve.


 


 


**Pending Changes:**


 


You cannot use any of the new column filters if you have changes 
pending in the grid, a warning dialog will appear telling the user to save 
changes prior to setting any new filters.


 


 


 


Return 
to [Data Developer](/html/hs4000.md)




