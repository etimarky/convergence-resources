



Item\_Loader\_\_Does\_Not\_Apply - Design For Retrieval (DFR) Help




**CCR 
Load File**


 


 


The 
CCR load file is a tab delimited file used for import.  The CCR extension tells 
Item Loader that the import is going to be handled differently from the CDR 
file.  


 


The 
user saves the file as a tab delimited file with the .CCR file extension.  
There are two column names that must exist in the file making up part of the 
Item Key.  These 2 columns are Rev and Model Variant.  They must be named 
exactly as is or the file will not load.  


 


The 
Item Key will be Item number and Revision.  Rev and Model Variant will be 
concatenated into the Revision field as <Rev> - <Model Variant> 
upon import.  It does not matter what 2 fields Rev and Model Variant are mapped 
to in DFR.  The Item Loader will know to look at the source field names.  To 
keep things simple, create 2 attributes in DFR named Rev and Model Variant.  
Map the Rev to Rev and Model Variant to Model Variant.  (Note:  As long as the 
source columns are named exactly Rev and Model Variant, the import knows what 
to look for no matter what fields they will be mapped.)  


 


If 
you receive the error, “Please unmap the revision attribute before proceeding.  
The revision attribute must be left blank.” , check the column names in the 
.CCR file.


 


This 
will ensure uniqueness in the Item Key.  It will be unfeasible to load 2 items 
having the same Item Number, Rev and Model Variant keeping the record unique.  


 


 


Return 
to [Item Loader](hs3000.md)


 


 




