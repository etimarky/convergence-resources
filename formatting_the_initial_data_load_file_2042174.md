



Formatting\_the\_Initial\_Data\_Load\_File - Design For Retrieval (DFR) Help



**Formatting the Initial Data Load File**


 


All items for a batch should contain one column for each **root attribute**.  Root attributes are those customer assigned and system attributes that will be common to all items in the catalog. These attributes are:


 


**Item Number** - a unique identifier for an item in the catalog; usually a part number.  Item number is mandatory.


 


**Legacy Part Number** - during a conversion process, it is desirable to keep a legacy part number if new part numbers are being created; Legacy Part Number is optional.


 


**Item Description** - a description of the item; Optional but recommended.


 


**Revision** - a revision of an item.  Revision is optional; the system will leave the field blank if the field has no data.


 


**Qualifier** - used to identify projects or programs, or could be a CAGE code in Aerospace applications.  The qualifier attribute is required. Including a value in this field is optional but recommended; the system will load a 0 in the field if there is no data.


 


**Qualifier** **Type** - Selected when the batch is imported, Qualifier Type provides an additional label to further differentiate an item. Qualifier Types include PART, DOCUMENT, ORGANIZATION, PERSON, PROGRAM, GUID, GIDEP and IMAGE. For example, a part and a document with the same item number and cage code can be differentiated by qualifier types PART and DOCUMENT.


 


All items in a batch MUST be of the same Qualifier Type. 


 


It is not unusual to have duplicate item numbers loaded into a batch or a classification. If a duplicate number exists in the batch, the Item Loader will reject the import with an error.  To correct the batch, edit the text file and remove the duplicate items, or use the Qualifier attribute to make the duplicates different. 


 


Separating items by Qualifier Type and loading different types of items in a separate batch will allow duplicate item numbers for drawings, documents and other items to be loaded along with parts of the same item number. 


 


Combining the Item Number, Revision, Qualifier, and Qualifier Type attributes to create a unique identifier provides the maximum opportunity to distinguish differences between items in the classification.


 


Return to [Preparing Data for the Item Loader](hs3020.md) or [New Batch Mode](hs3041.md).







