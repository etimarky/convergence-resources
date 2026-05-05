# Creating a Classification Load File

Creating\_a\_Classification\_Load\_File - Design For Retrieval (DFR) Help

## Creating a Classification Load File

There is a specific load file format needed for Convergence PIM Import Manager when it comes to classification data.&#x20;

In this example, the spreadsheet will be set up for attributes, categories, and the mapping of the two.&#x20;

&#x20;

The column headers must be named exactly what the mapping fields show in Convergence PIM.  Name

Description

Data Type

Length

Unit of Measure If they are not listed in the Excel spreadsheet exactly as they appear in Convergence PIM, the auto-mapping will not recognize it and the user will have to manually select the column headers from a drop down list.&#x20;

&#x20; &#x20;

The pages of the spreadsheet must always indicate what it belongs to, as seen below: Attributes

Categories

Classification &#x20;

![](.gitbook/assets/image\(1166\).png)

&#x20;

&#x20;

### Attributes

The attributes listed above will all be imported as new attributes. This means they did not exist before and are being created brand new in the spreadsheet.&#x20;

If the user would like to use existing attributes, they simply need to pull the name, description, type and UoM (if applicable) and fill them in on this sheet.&#x20;

&#x20;

Name: How the attribute name will appear in Convergence PIM on the master attribute list, classification, exports, SmartFind, etc.&#x20;

Description: This isn't mandatory but it is helpful to users to understand what it is the attribute is being used for.

Data Type: Tells Convergence PIM if this attribute needs to be created a specific way, such as a boolean, string, numeric, or file attribute.&#x20;

Length: Tells Convergence PIM how many characters it should allow before showing up as errors when validating in Data Developer.&#x20;

Unit of Measure: This isn't mandatory, but is helpful to create a base unit of measure that will apply to all data under that attribute. For example: V, in, cm, ft, W

### Categories

The categories page is used to lay down the structure.&#x20;

This needs to be built-out in the particular order shown below, otherwise Convergence PIM will not read it.&#x20;

Only Parent Category, Name, Description, and Full Path are mandatory on this page to have filled out.&#x20;

&#x20;

![](.gitbook/assets/image\(1167\).png)

&#x20;

### Category Attribute Mapping

&#x20;

This screen brings everything together: structure and attributes.&#x20;

It's all the same information listed on the previous two sheets, put together.&#x20;

This tells Convergence PIM which categories will hold which attributes.&#x20;

&#x20;

As seen  below, the only difference is that the columns highlighted in blue are optional.&#x20;

These can be set up from a high level to import in with predetermined key and required attributes as well as a display order, or those things can be decided at a later date through SmartClass.&#x20;

&#x20;

![](.gitbook/assets/image\(1168\).png)
