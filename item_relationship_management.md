# Item Relationship Management

Item\_Relationship\_Management - Design For Retrieval (DFR) Help

## Item Relationship Management

Convergence PIM software supports the linking of items to establish **Item Relationships**. These relationships can link items for any purpose, including but not limited to:

* Alternate parts
* Related parts
* Accessories

Managing these relationships is simple. You need the ability to access/edit the SmartClass module (Convergence PIM Online) and the Item Loader module (thick client).

&#x20;

### **Setting Up Data Model to Support Relationships**

The first step is configuring the data model to support the item linkages. This will be done using an item-type attribute assigned to the relevant category.

&#x20;

**1. Create the Relationship Attribute**

a. Navigate to SmartClass

b. Open the Attribute library (click the single tag icon ![](.gitbook/assets/image_118.png)

&#x20;in the left-hand navigation pane)

c. Create an attribute with a name that describes the relationship type (e.g. Related Parts)

d. Change the attribute's data type to "Items"

e. Click on "Properties" to expand the Properties options

f. Under the "Constraining Category" field, add the full category path for the category where the attribute will be assigned

![](.gitbook/assets/image\(2\).png)

&#x20;

**2. Add the Relationship Attribute to the Category**

a. Open the Classification Manager (click the folder structure icon in the left-hand navigation pane)

b. Navigate to and select the desired category

c. Add the relationship attribute to the desired category

![](.gitbook/assets/image\(3\).png)

&#x20;

**3. Confirm that adding the relationship attribute was successful**

a. Open the item details for an item within that category

b. The relationship attribute should appear as a Display Tab

![](.gitbook/assets/image\(4\).png)

&#x20;

### **Establish the Relationship Between Items**

To link items, you will need to create a .txt file and import that file using the Item Loader module in the Convergence PIM Thick Client.

&#x20;

**1. Create the import file**

a. Create a new spreadsheet

b. In cell A1, add the following text, replacing NAME OF ATTRIBUTE with the name of the attribute you created

Collection Attribute Name=NAME OF ATTRIBUTE So if your attribute is Related Parts, it would read

Collection Attribute Name=Related Parts c. Add column headers in row 2, in this order, starting in cell A2 and going across to cell H2:

Item Number

Item Revision

Item Qualifier

Member Item Number

Member Item Revision

Member Item Qualifier

Member Item Root Qualifier

Operation

d. Populate the rows beneath the headers with the desired item links

For example, imagine that you want to add item **90098765 (Qualifier = Part.0)** as a related part to **30012345 (Qualifier = Part.0)** **Item Number** - The item number for the item found in the category where you added the relationship attribute

In this example, the value would be **30012345** **Item Revision** - This column can be left blank

**Item Qualifier** - The value listed after the decimal in the item's Qualifier

If your item number is 30012345 and the qualifier is Part.0, the value in this column would be **0** **Member Item Number** - The item number for the item to link to the item in column A

In this example, the value would be **90098765** **Member Item Revision** - This column can be left blank

**Member Item Qualifier** - The value listed after the decimal in the member item's Qualifier

In this example, the value would be **0** **Member Item Root Qualifier** - The beginning root of the member item's Qualifier (default is "Part")

In this example, the value would be **Part** **Operation** - Indicate if the item is to be added to the relationship

The value in this column would be **Add** Example file:

![](.gitbook/assets/image\(15\).png)

&#x20;

e. Save the file as a **.txt** file

![](.gitbook/assets/image\(5\).png)

f. Close the file

g. Open your File Explorer and navigate to the location where you saved your file

h. Rename the file, changing the extension to **.rdl**

![](.gitbook/assets/image\(8\).png)

&#x20;

**2. Import the file to Thick Client**

a. Launch the Convergence PIM Thick Client and open the Item Loader module

![](.gitbook/assets/image\(9\).png)

b. Click "Import" at the top left of the window

c. Click on "Browse..." and select the file that you created

![](.gitbook/assets/image\(10\).png)

d. Confirm that the Root Qualifier matches what you wrote in column G of the file (default is Part)

e. Select "**ITEM NUMBER"** in both the Import File column and Product Attributes column, then click on the **<-->** button to map

![](.gitbook/assets/image\(12\).png)

f. Once mapped, you should see the fields reflected on the right side of the page

![](.gitbook/assets/image\(11\).png)

g. Click "Preview & Import"

h. Click "Import"

i. If the import was successfully processed, you will see "Items Loaded" appear at the bottom of the screen. If there are any errors, the import will not proceed and you will see an error message.

![](.gitbook/assets/image\(13\).png)

&#x20;

### **Validating the Import**

To confirm that the import was successful,

1. Navigate to one of the details page for one of the items in SmartFind
2. Click on the Display Tab associated with the relationship attribute you created
3. You should see the linked items appear on that tab

![](.gitbook/assets/image\(14\).png)

&#x20;

&#x20;

&#x20;

&#x20;
