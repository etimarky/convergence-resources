



Loading\_Items\_Directly\_to\_a\_Destination\_Category - Design For Retrieval (DFR) Help




**Loading Items 
Directly to a Destination Category**


 


Using 
the [**New Batch Mode**](javascript:popuplink('hs3041.htm')), Item Master Data and 
attribute values may be loaded directly to a destination category using a 
"**.cdr**" file extension on the tab-delimited data load file. The 
following specifications must be met:


·         
The first line of the load file must have the category path 
exactly as shown in the Classification Manager in the form of:


 


Category Path=Root\node\node...\terminal node


 


·         
The second line should contain the attribute names as column 
headings as shown below:


 


These attributes must include:


 


**Item Number** - a unique identifier for an item in the 
catalog; usually a part number.  Item number is mandatory and must be 
mapped in every new load file.


 


**Qualifier** – can be used to identify projects or programs, 
or could be a CAGE code in Aerospace applications.  Including a value in 
this field is optional but recommended; the system will load a 0 in the field 
if there is no data.


 


**Qualifier** **Type** - Selected when the batch is 
imported, Qualifier Type provides an additional label to further differentiate 
an item. Qualifier Types include PART, DOCUMENT, ORGANIZATION, PERSON, PROGRAM, 
GUID, GIDEP and IMAGE. For example, a part and a document with the same item 
number and cage code can be differentiated by qualifier types PART and 
DOCUMENT.


 


All items in a batch MUST be of the same 
Qualifier Type within a load batch. 


 


 


To 
add attributes to items already loaded into the classification, use the [**Import 
Mode**](javascript:popuplink('hs3042.htm')). For Import operations, the .cdr import file does not have to 
contain columns and values for all attributes. Additional attribute values may 
be imported in a subsequent load operation. Import operations require the 
following:


 


·         
The import file must minimally contain a column for Item Number, 
which has to be mapped during loading.


 




·         
No new items may be added to the file. New items should be added 
to a batch using the **Regenerate Mode**.


 




·         
Import items must reside in the same category, but do not need to 
be in the same batch.


 


 


To 
add new items to an existing batch, use the [**Regenerate Mode**](javascript:popuplink('hs3043.htm')). Regenerate operations 
require the following:


 


- New items added to the batch are added as news 
 rows at the bottom of the original New Batch .cdr file.

 




- All of the items from the original New Batch 
 load operation must be present in the Regenerate .cdr file.

 




- Root attributes from the original file may be modified, 
 however, technical attributes cannot be modified.

 


 


 


 


 


Return to [Preparing 
Data for the Item Loader](hs3020.md) 




