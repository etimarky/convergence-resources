



Views\_and\_Filters - Design For Retrieval (DFR) Help




**Views and 
Filters**


 


 


The 
Data Developer module allows the user to apply filters to columns and save 
specific filters and column configurations as views.


 


**Items do not need to be assigned to the current user to create a 
view or filter.**


 


**To Set a Filter:**


 


·         
Select an attribute you want to filter and then select Filter…  
  



·         
Select an operation from the list of operations.  
  



·         
Select a filter value or type in a filter value for your 
filter.  For Numeric attributes select an 
UOM if you choose not to use the default.  
The filter values represent all of the unique values for a column of 
data.  
  



·         
Now select ok to apply the filter or cancel to cancel.  
  



·         
If you selected ok, the spreadsheet should filter correctly.  To verify your filter settings, you can run 
your cursor over the attribute name and the mouse over will display the filter 
settings.  
  



·         
You can filter as many columns at once as you need.  Attributes that have an underline indicate a 
filter has been applied.  
  



·         
Filters can be removed one at a time by right clicking on the 
filtered attribute and selecting clear filter, or alternatively a user can 
select Clear All Filters and this will remove all filter applied yet still 
maintain your column configuration.  If 
you want to completely refresh your view, select Rest Columns and this will 
remove all filters as well as any column configurations to your grid, taking 
you back to the default view.  
  



 


 **To 
Create a View:**


 


·         
Once a user has configured their view for a category in data 
developer including: custom filters, aligning and hiding columns, formatting 
row and column widths, these settings can all be saved as a view.  
  



·         
To create a view select the Views… button.  
  



·         
Next to the save as field, enter the name of the view; you have 
the choice of saving the view as a public or private.  Only you can access the private views, public 
views are shared with all users.  
  



 **To Select a View:**


 


·         
A view can be selected from one of two places; all views can be 
selected if you are on the root category.  
If you are on a sub category to the root or a terminal node, only select 
the views associated with that category.  
You can view the category paths to determine what views you can load.  
  



·         
An error message will appear if you select a view that’s not 
accessible from the category you are on.



**To Delete a View:**


 


- A user can 
 delete all of their private views using the delete function from the views 
 screen.
- Only catalog 
 admin can delete public views.


 **To Sort a Column:**


 


·         
To sort a column in ascending and descending order, right click on 
the attribute heading and select sort ascending or sort descending.  
  



·         
A user can sort more than one column at once, the second column 
sorts after the first column.  When you 
mouse over a spreadsheet with more than one sort, it will display the sort hierarchy.  
  



·         
To clear a sort, right click on the attribute heading and select 
unsorted.


 



**Filter Operator’s:**


 


There 
are several operators to choose from when creating a filter.  Here is a description of some of the current filters:  
  



- Equal – filter 
 will find an exact match
- LIKE – filter 
 will find similar items, you have to use a wild card %
- Range – 
 typically two values with a dash in the middle, works for strings and numerics e.g. 1-2
- Is Null – will 
 filter on null fields
- Exists – will 
 only filter on fields with values
- Greater – will 
 filter on values greater than
- Less – will 
 filter on values less than

 


**Auto-Retrieve Mode:**


 


You 
will notice in the top right hand side of the grid there is an **Auto Retrieve After 
Filtering** option you can check.  If 
this is checked, any column you filter, sort or hide will trigger a retrieval 
of the data.  If you uncheck this option, 
you can set multiple filters, hide columns and sort and no retrieval will occur 
until you manually select retrieve.  
Please note that the grid clears after the first column filter you set 
and will not restore with items until you select retrieve.


 




**Pending Changes:**


 


You 
can not use any of the new column filters if you have change pending in the 
grid, a warning dialog will appear telling the user to save changes prior to 
setting any new filters.


 




Return to [Data Developer](mk:@MSITStore:C:\PROGRA~1\CONVER~1\CDSTOO~1\DESIGN~1.CHM::/html/hs4000.md)




