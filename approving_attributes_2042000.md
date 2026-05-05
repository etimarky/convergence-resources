



Approving\_Attributes - Design For Retrieval (DFR) Help




**Add 
File**


 


 


DFR has been improved to support files natively by using a new 
data type File.  This data type can be used similar to the data type items 
where there can be many files to the single item.  


 


Files will be added in the **WebDFR** application.  


 


1)  Add the file data type to the 
category desired just like any other attribute.  This is done in Classification 
Manager.  


2)  Open Data Developer and 
assign items to yourself.  **Note**:  You will NOT see the file data type in 
Data Developer that you created in Attribute Manager and assigned to this 
category.  It will not display as an attribute in Data Developer.  


3)  Go to WebDFR and the items 
will appear on the My Items tab. 


4) Edit Item which will bring the 
user to the Edit Screen in WebDFR.  The file data type that was created was 
‘IMAGES’.  **Note:**  File type supports Images, multimedia files, 
application files and text files. 


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/AM-Add_File_files/image001.jpg)




 


5)  Click on [Add Files] and the Select files dialog box will 
appear.  From here the user can add 1 to many files.  


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/AM-Add_File_files/image002.jpg)




 


6)  Select the ![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/AM-Add_File_files/image003.jpg)

 button.  This will browse your 
drive to select the file.  Select the file you want and click ok.  


7)  The File Information dialog 
box will display enabling the user to enter required attribute information.  
These attributes will depend on which ones apply to the Classification Category 
entered in when setting up the File data type attribute.


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/AM-Add_File_files/image004.jpg)




 


All attributes will display in 
the pop up with the exception of the vector data type attributes.  Click OK.  


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/AM-Add_File_files/image005.jpg)




 


8)  File will display in the list 
putting it in the queue.  Click on ![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/AM-Add_File_files/image003.jpg)

 to add any more files for upload.  


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/AM-Add_File_files/image006.jpg)




9)  Click on ![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/AM-Add_File_files/image007.jpg)

 button.  File will upload and 
progress of the upload will display on the screen.  


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/AM-Add_File_files/image008.jpg)




10)  The file upload is complete 
and the file is updated to the list on the left.  


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/AM-Add_File_files/image009.jpg)




 


Once a file is uploaded, the metadata is saved to the database for 
the DFR item that is created.  The file is saved to the data repository 
specified in the file data type settings.  If there is no Repository selected 
in the properties in the drop down, the file will automatically write to the 
default setting in the Remoting Server File.  It is required to have a default 
Repository.  If there is no default Repository set, the Remoting Server 
configuration file will throw an error.  


 


Each file upload displays 3 icons 
to the right of the file and the filename is hyperlinked.  


![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/AM-Add_File_files/image010.jpg)

  


 


If the user 
clicks on the filename, it will bring them to the edit function.  The edit 
function allows the user to edit the attribute information that was entered on 
the file upload.  These are the attributes based on the Classification Category.  
The ![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/AM-Add_File_files/image011.jpg)

 edit icon 
takes the user to the edit function as well.  The ![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/AM-Add_File_files/image012.jpg)

 open icon will open the file for 
viewing.  If the file data type cannot be opened, it will be downloaded to the 
user’s machine.  The ![](/userfiles/13115/16830/ckfinder/images/import-d2f34nel28gg/AM-Add_File_files/image013.jpg)

 delete icon will delete not only the file 
from the data repository but also the DFR item from the DFR catalog/database.  
This is a hard delete and not an obsolete status change.   
  



 


Return 
to [Attribute Manager](hs2000.md)




