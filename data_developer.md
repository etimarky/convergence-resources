# Data Developer

Data\_Developer - Design For Retrieval (DFR) Help

**Assigning Items to Users**

&#x20;

&#x20;

Items can be assigned to the current user or to other users listed in the DFR catalog from the data developer.&#x20;

&#x20;

The user who makes the assignment must have the **Item Assign** role to perform this function. This role is set in the User Manager module.

&#x20;

To assign an item (or items) in Data Developer, select the item(s), right click, and choose Assign Item.

&#x20;

Example: assigning 3 items to a user.

&#x20;

Once the Assign Item has been clicked, the use will have the option to choose the Assignee:

Example: Choose the user you would like, and click the OK button.

&#x20;

**Unassigning Items**

&#x20;

To unassign an item (or items) in Data Developer, select the item(s), right click, and choose Unassign Item.

&#x20;

Example: Unassigning 3 items.

&#x20;

Once the items have been unassigned, you’ll notice the Assigned User column is blank for those items

&#x20;

Example: After unassigning the “Assigned User” field is blank.

&#x20;

&#x20;

&#x20;

**Adding Items to a Batch**

&#x20;

To add items to a working batch in Data Developer, select the item(s), right click, and choose “Add Items to Working Batch…”

&#x20;

Example: Adding three items to a working batch.

&#x20;

After selecting the “Add Items to Working Batch…”, the user will be prompted for the batch name. The user can either type in a new name for the batch, or select an existing batch name from the dropdown list.  To remove all existing items from the batch prior to adding the new items, select the Clear Existing Items box.

&#x20;

Example: typing an new batch name.

&#x20;

Example: Selecting an existing batch.

&#x20;

**Filters**

All of the data displayed in Data Developer is based off of the filters in the upper left corner.

There are filters for Batch, User, and Status.

Example: filters set to return all data.

&#x20;

Adjust the filters to return the results desired.  For example, to only see the items in the “new batch name” batch, adjust your filters to select only that batch:

&#x20;

&#x20;

You’ll notice only the items in that batch are displayed in the category tree.

Example: filtering on a batch name.

&#x20;

Similarly, the user can filter on items with a specific status, or owner.

&#x20;

To toggle between the selected Filter, and the “All” mode, double click the text next to the dropdown.  For example, if “new batch name” is currently selected, you can toggle to “—ALL BATCHES—“ by double clicking “Batch”:

&#x20;

Example: To toggle “new batch name” to “—ALL BATCHES”, double click the label next to the dropdown.

&#x20;

Similarly, you can double click the “User” or “Status” label, to toggle between the selected value, and the “ALL” value.

&#x20;

When the user exits DFR, the values they had selected are saved, and restored the next time the user opens Data Developer.

&#x20;

**Removing Items from a Batch**

To delete an item from a working batch, select the item, right click, and select “Delete Item From Working Batches”.



Example: Deleting an item from a working batch.

&#x20;

After choosing “Delete Item from Working Batches…”, a dialog box appears to choose which batch to remove the item from.

&#x20;

Example: removing an item from a batch.

&#x20;

Choose the batch you wish the item to be removed from, and choose “Ok”.

Hint: To delete multiple items from a batch, follow the instructions in the Manage Working Batches section below.

&#x20;

**Managing Working Batches**

To manage working batches, right click on an item, and choose “Manage Working Batches…”:

Example: Selecting “Manage Working Batches…”

&#x20;

After selecting, a dialog box will appear, where the user can either delete or protect working Batches, as well as remove items.

&#x20;

Example: Deleting a working batch.

&#x20;

Example: Protecting a working batch.

&#x20;

Example: Removing an item from a working batch.

&#x20;

Hint: This dialog allows the user to delete multiple items from a batch.

&#x20;

**Editing Data**

To modify data, select the cell, Press F2 (or double click), and enter your new data. Modified data will appear in green.

Example: modified data appears in green.

&#x20;

Hint: A user can only modify items which are assigned to them.

&#x20;

After modifying data, you can commit your changes by selecting the “Save to DB” button.

&#x20;

&#x20;

**Editing Custom Attributes**

&#x20;

&#x20;

An attribute can have special properties to achieve certain functions.  This section describes some examples of DFR’s custom attributes and how to create, edit and use them in Data Developer.

&#x20;

&#x20;

**Vectors**

&#x20;

A vector attribute can be edited in Data Developer.  When you click on a vector attribute in Data Developer to edit, the user is presented attribute fields for each attribute in the vector as columns.  If you right click on a column a user can change the Unit of Measure for individual numeric attributes.  The rows of data combined represent a vector that a user can enter values against.

&#x20;

You can only filter Vectors, you cannot sort them, and all sorting options will be grayed out.  If you select Filter you will be presented with a custom dialog that will allow the user to filter on different vector values.  As the user enters values for the filter, a contextual explanation of the filter will appear in the bottom of the dialog box.  This explanation will help guide the user to select only valid filter values.

&#x20;

Users can use both copy and paste and drag copy (using the Alt key) on vector values, it works just like the normal attribute values.  The find and replace function only has find enabled, users will not be able to use the replace, that feature has been disabled.

&#x20;

**Ranges**

&#x20;

Range attributes are read only in Data Developer.  They will only display the minimum and maximum value in a range along with the units of measure.  If a user changes either a minimum and/or maximum attribute value the range attribute will automatically update to reflect this change.

&#x20;

You can filter ranges but you cannot sort ranges, sorting options will be grayed out.  When you pull up the filter dialog, you will notice the only operation choice is Test.  A user can only enter a test value for filtering, if that value fits in an existing range, it will bring back those ranges in the filter result.  For example, if the user enters 50 Deg C (for temperature range attribute) it will display all of the ranges that 50 Deg C would fit inside e.g. 0 to 100 Deg C.

&#x20;

Copy and paste and drag copy have been disabled for ranges.  A user can still access these operations on the fields used to create the range.  (E.g. max temperature or min temperature)  Find and replace has also been disabled on range values, as with copy and paste, these can still be done on the fields used to create the range.  (E.g. max temperature or min temperature)&#x20;

&#x20;

&#x20;

**MultiVal  (Multi-Value Attributes)**

&#x20;

MultiVal attributes can have multiple attribute values for a single field in Data Developer.  A user first has to create an allowed values list using the allowed values manager that contains all the possible multi-values.  When you click on a MultiVal attribute in Data Developer, a menu will appear allowing a user to select any or all of the possible values for the MultiVal attribute.  Once the values are selected they will appear in the single attribute field in Data Developer separated by vertical lines e.g. 4:value1|value2|value3|value4.  You will also notice the total number of values appears first in the field, followed by the individual values.

&#x20;

Since MultiVal works off of the allowed values list, any new values can be added to the MultiVal list by right clicking in Data Developer and selecting add allowed value.  Only users with allowed values rights can do this on the fly.

&#x20;

You can filter on MultiVal attributes but you cannot sort them, all sorting options have been grayed out.  The filter uses the Like operator.  A user has the option of sorting on an existing value using the drop down list or they can filter on just an individual value in a set of values e.g. steel.  The user must remember to use the wild card value % around filter values to obtain the filter result they desire.  For example, enter %steel% and the user will see items with multi-values like carbon steel, cold rolled steel, etc.  If they just enter steel, they will not get see these values in the filter result.

&#x20;

A user can copy and paste MultiVal attribute values from one field to another field (s) as long as it’s in the same column of data.  User can also drag copy MultiVal attributes, using the alt key on your keyboard, to populate multiple fields below or above a selected MultiVal value.

&#x20;

Users can use find and replace on MultiVal attributes just like normal attribute values.

&#x20;

Users can validate MultiVal attributes just like allowed values validation.  The validation should find any MultiVal attribute values that are not on the allowed values list.

&#x20;

&#x20;

&#x20;

**Setting the Status for an Item**

&#x20;

To set the status of an item in Data Developer, choose the item (or items), and select “Set Status”

&#x20;

Example: setting an items status to “Pending”.

&#x20;

&#x20;

**Exporting Data**

You can export data in Data Developer in either Excel (xls) or Text (csv) Format.

&#x20;

Once you have the data you wish to export displayed in the main grid, choose your report format from the Reports menu:

&#x20;

Example: Exporting data as text (csv).

&#x20;

Example: Exporting data as excel (xls).

&#x20;

Select the rows you wish to export, and choose the Export type from the Reports Menu.

Example: exporting 2 rows of data as a text file.

&#x20;

After choosing the export type, the user is prompted to save the file to a particular location.

&#x20;

Example: saving two rows of data as a text (csv) file as c:\reports\text\two\_rows.txt

&#x20;

&#x20;

**Viewing Attachment URL’s**

&#x20;

In the event that an item has a URL attribute, a “Link to: URL” will appear in the drop down.

&#x20;

&#x20;Example: Link to: URL.

&#x20;

When chosen, Internet Explorer will launch the URL of the selected item.

&#x20;

**Resizing the Detail Grid**

The user can resize the detail grid, by clicking the minimize or maximize buttons:

&#x20;

Example: to minimize the lower grid.

&#x20;

Example: to maximize the lower grid.

&#x20;

Note: The user may also resize the panels manually by clicking the area between the grid, and dragging the controls.

&#x20;

**Retrieving Relationship Data in the Detail Grid**

&#x20;

To populate the lower grid with Relationship data, double click the cell that contains the Relationship data you wish to retrieve.

&#x20;

Example: To display the 8 items indicated in the “Link Part to Document” attribute, double click.

&#x20;

Once the user double clicks this cell, the detail grid will be populated.

Example: Detail grid populated with the 8 items from the previous example.

&#x20;

Note: You can use the arrow keys to populate the grid with the details for other rows. For example, with the \<count=8> row selected, pressing the down arrow will retrieve the detail info for the next row.

&#x20;

**Adding or Deleting Items to the Detail Grid**

To add items to the detail grid, right click in the lower grid, and choose “Add Item”

&#x20;

Example: adding an item to the detail grid.

&#x20;

After selecting Add Item, a dialog box is displayed for the user to select the item they wish to add.  Locate the appropriate item(s), and choose Ok.

&#x20;

&#x20;

&#x20;

Example: Adding 3 items to the detail grid.

&#x20;

Note: To add items to the detail grid, the user must be the assigned use for the main item selected in the main grid.

&#x20;

Example: Deleting an item from the detail grid.

&#x20;

To delete items from the detail grid, select the item, right click, and choose “Delete Item”

&#x20;

Much like the upper grid, the detail grid also allows for assigning to new batches, setting status, and assigning items.

Example: the various commands for the detail grid.

&#x20;

&#x20;

**Commit or Cancel data in the Detail Grid**

If you have added, deleted or modified data in the detail grid, you have the option to commit those changes, or cancel them.  To commit changes, click the “Commit” button.

&#x20;

Example: committing changes to the detail grid.

&#x20;

To cancel the changes you made, click “Cancel”.

&#x20;

Example: Cancelling changes made to the detail grid.

&#x20;

&#x20;

**Re-Classifying Items**

To re-classify items in Data Developer, you can drag the item from the main window into the desired category in the category tree.  In order to reclassify items, the item needs to be writeable; that is, it must be assigned to the current user.

&#x20;

For example, to reclassify the highlighted item, click it, and drag it over to the desired category.

&#x20;

Example: Re-classifying an item into the “Document Information” category.

&#x20;

Note: If the item you are re-classifying has attributes that differ from the target category attributes, you will receiving a warning message similar to:

Example: Warning message indicating that the attributes for the item differs from the attributes for the target category.

&#x20;

**Sorting and Filtering Items**

Users are able to create filters for columns, and save those filters as configuration views.

&#x20;

To create a filter, right click on a column, and choose “Filter”.

Example: selecting a filter for an attribute.

&#x20;

After selecting Filter, the user is presented a dialog to define the filter:

&#x20;

After clicking OK, only items which match the defined filter will be displayed. So, in this case, only items with a Shank Length of less than 2.1 inches will be displayed:

&#x20;

Example: displaying only Shanks 2.1” or less. Note: After a filter has been applied, the attribute is underlined.

&#x20;

You can add filters as many attributes as you wish.

&#x20;

Filter operators include:

* Equal – filter will find an exact match
* LIKE – filter will find similar items, you have to use a wild card %
* Range – typically two values with a dash in the middle, works for strings and numerics e.g. 1-2
* Is Null – will filter on null fields
* Exists – will only filter on fields with values
* Greater – will filter on values greater than
* Less – will filter on values less than

&#x20;

&#x20;

Filters can be removed by right clicking the column, and choosing Clear Filter

Example: Removing a filter from an attribute column.

&#x20;

Hint: To remove all filters at once, click the “Clear All Filters” button:

&#x20;

Example: Clearing all filters.

&#x20;

To auto-retrieve data after applying a filter, check the “Auto Retrieve After Filtering” option:

&#x20;

Example: When checked, data will automatically be retrieved and displayed in the main grid after the user sets a filter.

&#x20;

**Creating a View**

Once the user has configured a category to their liking (including custom filters, hiding/aligning columns, they can save it as a view.  To create a view, select the “Views…” button:

&#x20;

Example: Clicking the Views button.

&#x20;

After clicking Views, the user is presented with a dialog.  Next to the save as field, enter the name of the view; you have the choice of saving the view as public or private.  Only you can access the private views, public views are shared with all users.

&#x20;

Example: Saving a Private View with a name of “MyView”.

&#x20;

Note: After clicking “Save as”, the view will appear in the list of views.

&#x20;

**Selecting a View**

To select a view, navigate to the category of interest, or select the Root node, and click the “Views…”  Button.



Example: Clicking the views button.

&#x20;

After clicking the views button, a dialog is presented for the user to select a previously saved view.

&#x20;

Example: To load a view, select it in the View Manager, and click “Load View”.

&#x20;

**Deleting a View**

To delete a view, click the “Views…”  Button.



Example: Clicking the views button.

&#x20;

After clicking the views button, a dialog is presented for the user to select a previously saved view.

&#x20;

Example: To delete a view, select it from the list of available views, and click the “Delete” button.

&#x20;

Note: Only a catalog admin can delete public views.

&#x20;

**Searching By Item Number or Description**

&#x20;

To search for an item by the item’s name or description, select the “Item Number/Description” tab, and enter a search string.  The “Search String” can match using a wildcard (“%”). So, to find all items that begin with DDXB, you could enter DDXB% as your search string, and press search.

&#x20;

Example: Searching for all items that begin with _DDXB._

&#x20;

Note: to do a search for all items, there is no need to search for “%”, just double click the category, and all data will be returned.

**Limiting Search to Previously Found Items**

&#x20;

Limiting a search to previously found items is useful when you want to search a number of items returned from a previous search.  In the previous example, we found all Items that began with DDXB.  If we wanted to find all items with “-13” in them from the previous search results, we could search for:

&#x20;

Example: Searching a subset of items for all items with “-13” in the name.

&#x20;

Note: Searching is limited to items within the selected category, as well as to the Batch, User, and Status selected.

&#x20;

**Searching Where Used**

To search through relationships to find where a particular item is used, you can use the Where Used Tab.&#x20;

&#x20;

Example, to find all items, which are contained in the relationship “Link Part to Document”, select the Roots\Non-Parts category, select the where used tab, choose the “Link Part to Document”, and then search.

&#x20;

&#x20;

&#x20;

&#x20;

&#x20;

Example: Returning all Items which are contained in Collections, “Link Part To Document”.

&#x20;

Double clicking on an item will display the items which contain this item in their attribute “Link Part To Document”. Example, double clicking on Item 100-1005, populates the detail grid with data like:

&#x20;

Example: Same item, which contains the Item 100-1005 as an item in its “Link Part To Document” attribute.

&#x20;

That is to say, that if we were to search for the item 100036, and look at the Attribute “Link to Part Document”, we’d see Item 100-1005 as one of its items:

Example: Showing detailed information for Item 100036’s “Link To Part Document” attribute.

&#x20;

&#x20;

**Searching Relationships**

Searching for Relationship attributes with a specific value is done using the Relationship tab.

&#x20;

For example, to find all items, which contain the relationship “Link Part to Document”, which have a relationship attribute with the value “test”, select the Relationship from the dropdown, enter your search criteria, and click search.

Example: finding all items which contain the relationship “Link Part to Document”, which have a relationship attribute with the value “test”.

&#x20;

At this point, if you double click on the cell, you’ll drill down into the details, where you’ll see the value “test”, which you searched for.

&#x20;



Example: Relationship Attribute which contains the text “test” which was searched for previously.

&#x20;

**Viewing Attribute Attachments**

&#x20;

The Data Developer allows users to view and open attribute attachments.  Attachments cannot be edited, deleted or updated, only viewed.

&#x20;

**Viewing Attribute Attachments:**

&#x20;

·         Retrieve the item or items you want to view from Data Developer.

·         Select the column title of the attribute you would like to preview.

·         At the top of the right click menu will display Attribute Information.  Select this.

**Right click option menu**

·         In the Attribute Information dialog box, you will see the list of Attribute Attachments.

**List of Attribute Attachments**

·        Double click on any attachment in the list to preview.

**Customizing the Data Display**

&#x20;

The Data Developer Module allows the user to hide columns and sort data to expand the work area and increase the efficiency of data manipulation. Use the **View** drop-down menu on the tool bar to manipulate the contents of the screen

&#x20;

**To hide the Toolbox column:**

&#x20;

·         Move the cursor to the X in the upper right corner of the **Toolbox** column on the left side of the screen

&#x20;

·         Press the **X** button

Note that the Toolbox column on the left side of the screen has been removed

&#x20;

&#x20;

**To hide the Category Tree column:**

&#x20;

·         Press the **View** button on the tool bar at the upper left corner of the screen

&#x20;

·         Select the **Hide category tree** button

Note that the category tree column has also been removed

&#x20;

The screen is now formatted to show the maximum screen area in spreadsheet format. However, there are several columns displayed with no data to work on and others with data that are not in view.  Columns not needed for editing can be hidden from view.

&#x20;

**To maximize the data display:**

&#x20;

·         Press the **View** button

&#x20;

·         Select the **Show/Hide Columns** option

&#x20;

·         Using the **Show/Hide Attributes** window, attribute columns may be selected to be displayed or hidden

&#x20;

·         To hide an attribute column, select the attribute or attribute (s) and then select Hide Y/N. Attributes that are hidden will show up in italic font. To unhide attributes, select the attribute or attributes (s) and then select Hide Y/N

&#x20;

&#x20;

The order of the displayed columns can also be changed, moving target attributes into a preferred order for editing.

&#x20;

**To change the order in which data columns are displayed:**

&#x20;

·         Click on the attribute name, holding down on the key on mouse, slide the attribute column to the right or left. This will move the attribute column to your desired position.

&#x20;

The data is now ready to be edited

&#x20;

**To reset the columns to the original order:**

&#x20;

·         Press the **Reset Columns** button at the top of the screen

&#x20;

&#x20;

&#x20;

**To Format Row Height and Column Width: (gang selection)**

&#x20;

·         Select all of the row (s) you want to adjust the row height for.  Drag the last row down to the desired row height; you will notice the other rows will adjust the same way.

·         Select all of the column (s) you want to adjust to column width for.  Drag the last column to the desired column width; you will notice the other columns will adjust the same way.

·         Both row and column formatting can be saved with a View.  Formatting can be removed only once reset columns is set, clear all filters button does not clear any formatting.

&#x20;

&#x20;

**Deleting and Removing Items**

&#x20;

Users can delete items that are assigned to them in Data Developer as long as the DFR catalog is in sandbox mode.



**Example of deleting items in Data Developer**

&#x20;

**Does Not Apply**

&#x20;

&#x20;

Users can set Does Not Apply for each category attribute, as a category property, in the Classification Manager.  Once this is set for a particular category attribute, users have the ability to identify which items in this category do not require values for an attribute in the Data Developer, even if the attribute maybe required for that category.  See the Classification Manager help file for more information on enabling Does Not Apply.

**Using Does Not Apply in Data Developer:**

To use Does Not Apply, once it has been enabled in Classification Manager, you must have items assigned in Data Developer for that category.  From Data Developer, a user can right click on an attribute field and select **Set Does Not Apply - Set**.  Only attributes that have Does Not Apply enabled in Classification Manager will offer this option.  The user will need to save this change just like an attribute value change, in order for this setting to work.  When Does Not Apply has been set, the user should see in the attribute value field.  Attributes that are shaded in brown have DNA enabled.  Only attributes that are required can have DNA enabled.

Looking at the data in Data Developer, you will see the in the fields as place holders as shown below.  Right clicking on the field gives you the option to clear the Does Not Apply value in which the field would be empty yet displayed in green.  Right clicking again gives you the option to add the Does Not Apply value.&#x20;

A user can not copy and paste the value or drag copy the value.  If a user wants to set for multiple fields, highlight the fields first, then you can right click to set for the highlighted fields.  You also can not filter on DNA using the filtering capabilities of Data Developer.

If a user exports DNA data to excel, the symbol will show up in the export file.

To remove Does Not Apply for an attribute field you right click and select **Does Not Apply – Clear**.

To preview the data result in Data Developer, set batch to the name of the file you just imported.  Retrieve the records that were imported, select the rows and assign all rows to you.  Right click on the attribute to get the Does Not Apply – Clear or Does Not Apply – Add option.  (See below)

&#x20;

_**Right click to get the Does Not Apply – Clear or Does Not Apply – Add option**_

When running validations, required attribute fields that are blank with Does Not Apply set, will not create a validation error.

When loading data from the Item Loader (via Import Mode), if your load file has values in a field that has Does Not Apply Set, it will automatically reset that field or clear the Does Not Apply. &#x20;

&#x20;

&#x20;

**Running a Validation in Data Developer**

&#x20;

Once the validations have been defined and data cleansing has been performed in the Data Developer, a validation is run against the data using the Validation mode.  To perform validations on items they need to be assigned to a batch and assigned to the user running the validations.&#x20;

&#x20;

**To perform validations on a batch of data:**

·         Select Validation Mode.

·         Press the down arrow to the right of the **Batch** field and select thebatch to be validated.

&#x20;

·         Press the down arrow to the right of the **User** field and select the owner of the batch.

&#x20;

·         Press the down arrow to the right of the **Status** field and select the status of the items to be validated.

&#x20;

·         Press the down arrow to the right of the **Error Type** field and select the type of validation to be run. This field will list the standard validation routines as well as any site specific or custom validations included in the installation.

&#x20;

·         If an Allowed Values List has been used to restrict the attribute to a specific set of values, check the **Restrict to Allowed Values** check box.

&#x20;

·         Move the cursor through the classification tree opening categories to expose the target category. Select the target category.

&#x20;

·         Press the **Retrieve** button to retrieve and display the data.

&#x20;

The Data will be displayed in spreadsheet format. The spreadsheet display can be customized to better view the data.

&#x20;

If the data has been validated in the past, that date will be displayed in the **Last Validated:** field.

&#x20;

·         Press the **Validate** button to begin the validation. A **Validation Progress** window will appear and report the progress of the validation.&#x20;

&#x20;

·         A **Validation Complete** window will confirm that the operation has concluded. Press **OK**.

&#x20;

**To retrieve the validation results:**

&#x20;

Attribute fields containing errors will be shaded in pink.

&#x20;

·         Use the arrows at the right and bottom of the spreadsheet to scroll through the data. Attribute fields containing errors will be shaded in pink. Run the cursor over the pink shaded fields to view the error.

&#x20;

·         Press **View Report** to generate a detailed report of the validation. Each item in the batch will be listed along with its current status.

&#x20;

**To fix validation errors:**

&#x20;

Validation errors can be corrected in the Data Developer spreadsheet in the same manner as in the Data Validator Module. Once the errors have been corrected, save the changes by pressing the **Save to DB** button at the top of the screen.

&#x20;

&#x20;

**Setting Allowed Values**

&#x20;

The Data Developer allows users to add values to the allowed values list.  If a user has the allowed value role, they will have the additional option of assigning allowed values to an attribute in the Data Developer.  The data needs to be assigned to you in order to execute this function.

&#x20;

&#x20;

**Setting an Allowed Value:**

&#x20;

* Retrieve the item or items you want to work on in Data Developer.
* Select and copy the value you want to add to the allowed values list.
* The right click menu will display the option to add an allowed value.
* A dialog box will open presenting the user a list; now paste the value you want to add at the top of this list.
* If there are two allowed value lists for this attribute, the user will have the option to assign the new value as either a local allowed value or a global.

&#x20;
