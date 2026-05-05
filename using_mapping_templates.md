



Using\_Mapping\_Templates - Design For Retrieval (DFR) Help




**Loading 
Working Batches**


 


The 
Item Loader allows users to load working batches.  A working batch load file is a text file that 
contains a list of Item Numbers.  If an 
item has a qualifier, then a second column containing the qualifier must be 
present.  The text file must be saved 
with a **.bwb file extension**.


 




**Loading a New Working 
Batch:**


·         
When 
creating a new working batch; you start as if you are loading a new batch by 
following these steps:


o        
select 
new batch 


o        
select 
your working batch file (**.bwb file 
extension**)


o        
enter 
a working batch name


o        
Select 
the root qualifier  
  



·         
The 
.bwb extension triggers the Item Loader to handle load files differently; it 
puts the Item Loader into loading working batch mode.  As a result you will notice some differences 
with the Item Loader when creating and editing working batches.  
  



·         
You 
do not need to include the qualifier type in the .bwb file since qualifier type 
is handled when you select in the Item Loader; just like traditional load files. 
  
  



·         
You 
only need to map the Item Number and Qualifier fields when loading a new 
working batch of parts; there is no value to mapping other fields.  
  



·         
The 
preview screen has the option to clear existing contents in the top left; this 
field is only active when you are in the Regen mode.  The preview screen should show the Item Key 
mappings prior to loading.  The preview 
screen is called Working Batch Preview when you are loading working batches.  
  



·         
A 
user can also load items into an existing working batch using the **Regen option**.  They can also clear all of the items in an 
existing batch during the regen process.  
  
  



·         
The 
import process is not used when loading working batches.  
  



·         
**Error conditions** to be aware of:  
  



o        
You 
can only load working batches if all the items in the working batch have the 
same qualifier type for new batches.  For Regen batches for example; you 
can load a group parts to an existing working batch that may have documents as 
the qualifier type or other items with other qualifier types.  The Items you 
are loading (in your .bwb load file) must always have the same qualifier type 
for both new batches and regens.    
  



o        
You 
can only load items that already exist in the database  
  



o        
You 
can not select an existing batch name for a new working batch


 


 


Return to [Item 
Loader](hs3000.md) 




