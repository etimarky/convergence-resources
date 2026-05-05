



Adding\_Multiple\_Images\_Using\_Import\_Manger - Design For Retrieval (DFR) Help



# Adding Multiple Images Using Import Manger


 


An Excel file must be set up first before the import process can begin.  

 


It must look like the attached list. This includes:


- The column headings matching the format of
	- ItemNumber ( no spaces)
	- ImagePath  ( no spaces)
- The worksheet itself must be named "Image."
- The Image Path must be whatever it is named in the folder that will be referenced later in this document.  

 Usually this is located in a category folder or on the computer desktop.
- The image must be in PNG format.


It is most simple to, but not a requirement to name the image file the same name as the part number. 
 


![](assets/image(990)_1.png)




 


Locate the Import Manager and select Item Data


 


![](assets/image(974)_1.png)




 


Browse for the file and select it. 


Select Next on the bottom right of the screen. 


 


![](assets/image(975)_1.png)




 


Select Excel as the Import Format. 


Excel Collection Data will also work for multiple image loading. 


 


![](assets/image(977)_1.png)




 


If the images are being loaded with new parts, the operation will need to be set as Create. 


If the images already exist and images are being loaded after the fact, the operation will need to be selected as Update. 


 


When loading images, the user must expand the arrow next to " Item Options."


 


![](assets/image(978)_1.png)




 


The Item Options will open up the following:  

 


**Default Category:** This will always default to " Root\To Be Classified". 


This can be changed to any target category, but will always default if left alone. 


**New Batch:** This will always default to " Default\_Batch" meaning that there will always be a leaf node by that name under " To Be Classified" where parts will automatically be delivered to if they are not given another category path. 


The user can rename this batch to anything else, creating additional leaf nodes under " To Be Classified." 


**Existing Batch:** This option will allow the user to deliver parts to an existing batch or deliverable.


**Import Files from Directory:** This option allows the user to choose an image path from their desktop or documents on their computer. 


 


![](assets/image(980)_1.png)




 


Select Import Files from Directory and choose your category path.


 


![](assets/image(981)_1.png)




 


Once the category/image path has been selected, drop to the bottom of the mapping page. 


 


![](assets/image(983)_1.png)




 


- Locate the File Number on the drop down from the excel file chosen in previous steps.
- "Document.0" will be the default but since images are being uploaded, this must be changed to Image.0
- Locate the File Path on the drop down from the excel file chosen in previous steps.
- The operation will be set to Add, since images are being added for the first time.


Select Next on this page, and next on the following. 


 


Select Validate. 


 


![](assets/image(984)_1.png)




 


 


The ThickClient will then validate the data to ensure there are no errors or discrepancies. 


As long as there are no errors, select 'Next." 


 


![](assets/image(986)_1.png)




 


Select Import.


 


![](assets/image(987)_1.png)




 


The import process will take place and once complete, select Done. 


 


![](assets/image(988)_1.png)




 


Finally, locate the part in SmartFind and notice the updated image. 


 


![](assets/image(989)_1.png)





