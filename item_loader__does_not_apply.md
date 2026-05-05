



Item\_Loader\_\_Does\_Not\_Apply - Design For Retrieval (DFR) Help




**Auto 
Item Number Generation**


 


 


The 
load file must have the correct value in the item number field for auto item 
number generation to work.  Go to the options manager and look for the value 
used for option -  ItemLoadAutoGenText.  In the example below the value is 
“#”.  Also notice the qualifier set to work with this value is Auto.  It 
doesn’t have to be Auto, this is just an example.


 


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/IL-AutoItemNoGen_files/image001.jpg)




**Example of a load file formatted for 
auto-item number generation – see highlighted fields**


 


Make 
sure to select the correct root qualifier when loading a file that requires 
auto-generation of item numbers.


 


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/IL-AutoItemNoGen_files/image002.jpg)




**Item Loader Import dialog box**


 


A 
user must remember to have the correct qualifier and root qualifier, as well as 
value for the auto generation of item number to work properly.  If you are not 
sure, contact your DFR administrator.


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/IL-AutoItemNoGen_files/image003.jpg)

   


**Note the value for the item number - <Auto 
Number> in the preview screen**


 


 


Guidelines on auto item number 
generation:


 


1.)    
Configure this with help from your DFR 
Admin


2.)    
Select a value to use as item number 
that will trigger auto item number generation, this value needs to be setup in 
the options manager


3.)    
Remember to use the correct root 
qualifier and qualifier with each auto item number generation for both Item 
Loader and WebDFR.


4.)    
This feature can support different 
items e.g. documents, parts, organizations, that can all have their own 
sequence of auto generated item numbers


5.)    
Auto generated item numbers can have 
specific formats e.g. prefixes, suffixes, etc.  Contact your DFR admin to 
setup.


6.)    
It’s ok if auto generated item numbers 
don’t all get used in sequence, since users can delete parts or cancel creating 
a new part in WebDFR.


7.)    
Auto generated numbers are tied to 
qualifiers.  Different qualifiers can use the same auto generated number 
sequence or they can have their own.  Item numbers generated for specific 
qualifiers will share the same number sequence no matter where they are 
generated from; WebDFR or through Item Loader.


8.)    
WebDFR and DFR Item Loader all work off 
of the latest item number that is how they stay in sync.  It’s not possible for 
WebDFR and DFR Item Loader to try to use the same auto-generated item number, 
so you don’t need to worry about collisions.


 


Return 
to [Item Loader](hs3000.md)


 


 




