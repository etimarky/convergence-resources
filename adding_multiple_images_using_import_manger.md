# Adding Multiple Images Using Import Manger

Adding\_Multiple\_Images\_Using\_Import\_Manger - Design For Retrieval (DFR) Help

## Adding Multiple Images Using Import Manger

&#x20;

An Excel file must be set up first before the import process can begin.

&#x20;

It must look like the attached list. This includes:

* The column headings matching the format of
  * ItemNumber ( no spaces)
  * ImagePath  ( no spaces)
* The worksheet itself must be named "Image."
* The Image Path must be whatever it is named in the folder that will be referenced later in this document.

Usually this is located in a category folder or on the computer desktop.

* The image must be in PNG format.

It is most simple to, but not a requirement to name the image file the same name as the part number.  &#x20;

![](.gitbook/assets/image\(990\)_1.png)

&#x20;

Locate the Import Manager and select Item Data

&#x20;

![](.gitbook/assets/image\(974\)_1.png)

&#x20;

Browse for the file and select it.&#x20;

Select Next on the bottom right of the screen.&#x20;

&#x20;

![](.gitbook/assets/image\(975\)_1.png)

&#x20;

Select Excel as the Import Format.&#x20;

Excel Collection Data will also work for multiple image loading.&#x20;

&#x20;

![](.gitbook/assets/image\(977\)_1.png)

&#x20;

If the images are being loaded with new parts, the operation will need to be set as Create.&#x20;

If the images already exist and images are being loaded after the fact, the operation will need to be selected as Update.&#x20;

&#x20;

When loading images, the user must expand the arrow next to " Item Options."

&#x20;

![](.gitbook/assets/image\(978\)_1.png)

&#x20;

The Item Options will open up the following:

&#x20;

**Default Category:** This will always default to " Root\To Be Classified".&#x20;

This can be changed to any target category, but will always default if left alone.&#x20;

**New Batch:** This will always default to " Default\_Batch" meaning that there will always be a leaf node by that name under " To Be Classified" where parts will automatically be delivered to if they are not given another category path.&#x20;

The user can rename this batch to anything else, creating additional leaf nodes under " To Be Classified."&#x20;

**Existing Batch:** This option will allow the user to deliver parts to an existing batch or deliverable.

**Import Files from Directory:** This option allows the user to choose an image path from their desktop or documents on their computer.&#x20;

&#x20;

![](.gitbook/assets/image\(980\)_1.png)

&#x20;

Select Import Files from Directory and choose your category path.

&#x20;

![](.gitbook/assets/image\(981\)_1.png)

&#x20;

Once the category/image path has been selected, drop to the bottom of the mapping page.&#x20;

&#x20;

![](.gitbook/assets/image\(983\)_1.png)

&#x20;

* Locate the File Number on the drop down from the excel file chosen in previous steps.
* "Document.0" will be the default but since images are being uploaded, this must be changed to Image.0
* Locate the File Path on the drop down from the excel file chosen in previous steps.
* The operation will be set to Add, since images are being added for the first time.

Select Next on this page, and next on the following.&#x20;

&#x20;

Select Validate.&#x20;

&#x20;

![](.gitbook/assets/image\(984\)_1.png)

&#x20;

&#x20;

The ThickClient will then validate the data to ensure there are no errors or discrepancies.&#x20;

As long as there are no errors, select 'Next."&#x20;

&#x20;

![](.gitbook/assets/image\(986\)_1.png)

&#x20;

Select Import.

&#x20;

![](.gitbook/assets/image\(987\)_1.png)

&#x20;

The import process will take place and once complete, select Done.&#x20;

&#x20;

![](.gitbook/assets/image\(988\)_1.png)

&#x20;

Finally, locate the part in SmartFind and notice the updated image.&#x20;

&#x20;

![](.gitbook/assets/image\(989\)_1.png)
