



Reports\_Loadoffroot - Design For Retrieval (DFR) Help




**Reports**


 


 


DFR has a preset list of *Reports* on the mail menu 
accessible to various users depending on access and which module is open.  
Below is a summary of each report and the required security access.  Reports 
can be customized as a drop-in for any requirements that the user may 
have.  


 


**Admin Audit** 


The Administrative Audit report displays all actions 
performed by the Admin login.  Primary information details the Date/Time, 
Action, User Login and any Additional Information.  


 


The Action can include actions such as *Added User to 
Catalog* or *Updated User*.  The User Login displays the login of 
the user that performed the action.  The majority displays the Admin 
login.  However, if any user has Catalog Administrator privileges, their 
logins would display as well.  The *Additional Information* displays 
more details.  


 


**Batch Status By User** 


The Batch Status by User report displays the status of all 
batches within DFR.  This could be a very sizeable report.  It groups 
each batch by assigned users and unassigned items.  Then it tracks counts 
of each status including New, InWork, Pending and Approved.  The InWork 
column includes all items with a User Defined Status.


 


The right half of the report tracks validation statistics 
which are the field completion totals.  Validations log the number of 
items in a batch that have been validated.  Total displays the percent of 
the total items in the batch that have been completed.  Required displays 
the total percent of fields that have been validated, completed and are 
required.  


 


**DFR Audit** 


The DFR Audit report allows the user to enter in 
criteria.  This criterion includes a date range, a selection of users, and 
a selection of audit types.  The Audit Report gives a detailed list of 
what logins performed what actions and which users logged in and out of the 
system.  It tracks down to the granular detail listing every part that was 
loaded in an Item Load, attributes updated and what values are removed for any 
attributes. 


 


By default, the date range is 30 days from the time the 
Audit window is opened, no users are selected, and all audit types are 
selected. Clicking the “…” button under the Users panel will open a secondary 
window that allows selection of users available to the catalog. Multi-selection 
of users is available by using CRTL + click. Checking and unchecking the check 
box labeled “Select All” will select and unselect all audit actions in the 
Audit Types panel.  


 


**Duplicate Collection Entries**


The Duplicate Collection Entries report displays any item 
that is duplicated assigned to the same parent.  The query looks at all 
the relationships and does a check to see if there are multiple entries for the 
same parent and child relationships that have the same values down to 
relationship attributes.  


 


**Error Log**


The Error Log report displays all errors that were logged in 
the error log table in the database.  This is an organized report summary 
of errors that occurred with the catalog and DFR.  


 



**Export-Excel With Pick Lists**


This report does not display in DFR but exports to 
Excel.  Data Developer must be open in order for this option to be 
active.  The user must select a group of items whether it is a batch, a 
report or a category.  All attributes are exported to an Excel spreadsheet 
with the pick lists.  This means that if there are dropdown options 
(Allowed Value Lists) for any attributes, they will be imported into Excel as a 
pick list.


 


**Export-Text Item Attribute Values**


This report does not display in DFR but exports to a txt 
file format.  Data Developer must be open in order for this option to be 
active.  The user must select a group of items whether it is a batch, a 
report or a category.  All attributes are exported to a text file which is 
| delimited.


 


**Export-XL Item Attribute Values**


This report does not display in DFR but exports to 
Excel.  Data Developer must be open in order for this option to be 
active.  The user must select a group of items whether it is a batch, a 
report or a category.  All attributes are exported to an Excel 
spreadsheet.  This is a straight export on the attribute values.  
This report does not export the Allowed Values Lists into pick lists. 


 


**Items Load Report**


The Items Load report functions much the same as the DFR 
Audit report, but only shows items that were loaded into DFR. The items listed 
in the report can be filtered by date loaded, as well as by which users loaded 
items. 


 


**Item Management**


The Item Status report displays general information on a 
group of items.  This report is dependent on Data Developer being 
open.  Select either a batch of items or a category of items and click 
Retrieve.  Once items are retrieved, this report will be active on the 
Reports toolbar.


 


The general information displayed includes all item key 
information such as Item Number, Rev, Qualifier and Legacy Part Number as well 
as the description.  The report shows the status of each item at the time 
the report is run.  Status items shown are the User each item is currently 
assigned to, status of the item, Date Update and the latest batch the item was 
added.  


 


**Module Type Summary**


The Module Type Summary is active if Item Mapping module is 
open.  This report displays details on **ALL** module types in Item 
Mapping.  Since the report runs for all modules within Item Mapping, this 
report will take a few hours to run depending on the count of modules 
types.  


 


**Overall Batch Status**


The Overall Batch Status report displays the status of all 
batches within DFR.  This is a very simple report.  It lists each 
batch name and tracks counts of each status including New, InWork, Pending and 
Approved.  The InWork column includes all items with a User Defined 
Status.  


 


The right half of the report tracks validation statistics 
which are the field completion totals.  Validations log the number of 
items in a batch that have been validated.  Total displays the percent of 
the total items in the batch that have been completed.  Required displays 
the total percent of fields that have been validated, completed and are 
required.  


 


**System Information**


The System Information report gives very detailed 
information that is pertinent to the system it is being run.  This 
information includes Machine name, application files and their version, 
drop-in’s being used and their version.  The report also includes all the 
same information that applies to the Remoting Server the catalog is running. OS 
information, directories used for the application and drop-in, versions of all 
the dlls and drop-in files.  


 


**User Logins**


The User Logins report can only be viewed by the Admin 
login.  This report just displays all current users logged in to the 
Remoting Server by catalog.  


 


**Validation Report**


The Validation Report must be run after a validation is performed 
on a batch of records.  Data Developer module needs to be open and the 
Validation box should be checked to execute the Data Validator.  The 
Report then displays all results from the validation.  This includes every 
attribute that displays in pink flagging the user that there is an issue.  




**What Description Templates Need To Be Rerun**


This report provides a list by category of which templates 
need to be rerun due to data model changes or an edited description 
template.  The following changes will cause a template which uses the 
changed attribute to appear within the report:  attribute names, attribute 
data type, deletion of an attribute, default unit of measure, and attribute 
default decimal places.


 




