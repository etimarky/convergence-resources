



Approving\_Attributes - Design For Retrieval (DFR) Help




**File 
Type Attributes**


 


 


DFR has been improved to support files natively by using a new 
data type File.  The File type will support Images, multimedia files, 
application files and text files.  This data type can be used similar to the 
data type items where there can be many files to the single item.  It will be 
handled like a relationship attribute where files will be stored as DFR items 
and associated to items via a relationship.  This association process will be 
automated during the file upload in WebDFR.  (See WebDFR help Document.)


 


The File attribute has 4 additional properties which will need to be 
set when creating a File type attribute.  These properties are the following:


1.     
File Type – This can be an Image, Multimedia file, 
Text file or an application file.  This is a dropdown.  (see example)


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/AM-File_Data_Type_files/image001.jpg)




**NOTE:**  By 
selecting the Image file type, the item will be displayed as an image.  By 
selecting any of the other file types, the item will be displayed as a 
clickable link.  


2.     
Classification Category – This is the category where the 
DFR Item will reside that represents the Item for each file uploaded.  Category 
is displayed like root\Non-Parts\Specification Documents.  The Category is set 
here. 


3.     
Repository – Data repository where the files will be 
stored.  The drop down list will be configured in the Remoting Server 
Configuration file.  (See DFR Admin Guide)


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/AM-File_Data_Type_files/image002.jpg)




4.    
Restrictions – This is a comma delimited list with no 
spaces and allows the user to configure which files are restricted from being 
uploaded.  The users will not be able to upload any file types should there be 
any restrictions configured here.  


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/AM-File_Data_Type_files/image003.jpg)




 


These properties can be edited within the Attribute Manager as 
long as the user has the appropriate roles of Attribute Authorizer or Attribute 
Developer.


 



 


Return 
to [Attribute Manager](hs2000.md)




