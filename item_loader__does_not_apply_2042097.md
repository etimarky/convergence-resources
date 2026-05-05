



Item\_Loader\_\_Does\_Not\_Apply - Design For Retrieval (DFR) Help




**Does 
Not Apply <DNA>**


 


 


All 
attributes are global throughout DFR and SmartFind.  Setting them to Required 
may be a data requirement for some instances.  However, in some modules, this 
“Required” may not apply.  The application allows you to set an instance of it 
to Allow:”Does Not Apply”.  With this setting, the field is not required.  The 
application sets the value to <DNA> as its value.  This acts as a place 
holder in the field.


 


Users 
can set Does Not Apply for each category attribute, as a category property, in 
the Classification Manager.  Once this is set for a particular category 
attribute, users have the ability to identify which items in this category do 
not require values for an attribute in the Data Developer, even if the 
attribute maybe required for that category.  See the Classification Manager 
help file for more information on enabling Does Not Apply.


 


In 
Item Loader, select Import or New to import a new batch file.  See sample batch 
file below.


 


![](images/IL-Does_Not_Apply001.jpg)




**Note <DNA> values in Document Type 
column in sample TestDNA.cdr file**


 


Name 
the batch and select a Root Qualifier from the dropdown.  Select OK to process.


 


![](images/IL-Does_Not_Apply002.jpg)




**Item Loader Import dialog box**


 


When 
performing a batch load, all rows are displayed.


 


![](images/IL-Does_Not_Apply003.jpg)

   


**Note that 32 rows are in the file for batch 
load.**


 


If 
a user attempts to load DNA values for an attribute that does not allow DNA, or 
does not have DNA enabled as a category attribute property, then those items 
will be flagged as an error when loading using the Item Loader.  You will be 
able to preview the Import Error Report displaying the rows that cannot be 
imported and why.  Seven rows were identified as having DNA values specified 
for attributes that do not allow DNA as a value.  


 


![](images/IL-Does_Not_Apply004.jpg)




**Import errors on <DNA> values being 
brought in to attributes that do not allow <DNA> value**


 


Item 
Loader will then take these rows out of the file for import. There are now 25 
rows to load. 


 


![](images/IL-Does_Not_Apply005.jpg)




**Note there are 25 rows that qualify to be 
loaded** 


 


Select 
Import to complete the batch load.  Once you see the words “Items Loaded” at the 
bottom of the screen, this displays a successful load on the 25 rows.  


 


![](images/IL-Does_Not_Apply006.jpg)




**Note the Items Loaded message.**


 


The user can now view items loaded 
in Data Developer by selecting the batch name of the file you just imported.  
See the Data Developer help file for more information on how to preview the 
items loaded.


 


 


Return 
to [Item Loader](hs3000.md)


 


 




