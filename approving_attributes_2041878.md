



Approving\_Attributes - Design For Retrieval (DFR) Help




**Export 
Manager**


 


 


Export Manager is the primary and preferred method for exporting 
both structure and items data in the DFR system to a file of a particular 
format, an external system, or to some external API.  Export Manager has an 
extensible infrastructure that allows Convergence Data Services to add any 
export format or system integration needed.  The Out of the Box formats 
that are supported are Excel, XML, and PLM XML.


 


When opening the Export Manager, 
the first screen will provide the user with a summary of past exports completed 
along with the option to export classification structure or item data (See 
Figure 1).  To continue, choose whether you want to export Classification Structure, 
Attribute Groups, or Item Data.


 


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/EM_files/image002.jpg)




**Figure 1**


 


 


**Export Options**


 


Regardless 
of whether a user chooses to export Classification Data or Item Data they will 
be presented with an options screen that looks similar to the Figure 2. The 
options displayed to the user vary depending on the export type being 
done.  The user must provide all required information before they are able 
to proceed.


 


![](/userfiles/13115/16830/ckfinder/images/import-cbg4qpn20hv5/EM_files/image001.jpg)




**Figure 
2**


 



**Options Common to All 
Export Types**


 


The following options 
are available regardless of the export type chosen:


- **Export Name**:  This is 
 the name that will be given to the export.  This name will be visible 
 when viewing export history.
- **Export Type**:  Type of 
 export to perform.  This defaults to Excel but other out of the box 
 export types are PLM Xml and CDS Xml file formats.
- **Incremental Export**:  The export 
 process will include only items and classification structure that are new 
 or have changed since the last export.  NOTE: Exported items and 
 classification structure history are per Export Type.
- **Advanced Options**
- Root Category 
 Path: When exporting Categories, they will be appear in the output file 
 relative to this category path. For example, if you specify “Root\Parts”, 
 then export “Root\Parts\Screws” and “Root\Parts\Screws\Metric” the Parent 
 Category for “Screws” will be blank, and the Parent Category for “Metric” 
 will be “Screws”. If you leave this field blank and export 
 “Root\Parts\Screws” and “Root\Parts\Screws\Metric”, the Parent Category 
 for “Screws” will be “Root\Parts” and the Parent Category for “Metric” 
 will be “Root\Parts\Screws”.
- Attribute Prefix: 
 This value will be pre-pended to the Name of each Attribute exported. 
 This feature is useful if the data will be imported into another system 
 and there is a possibility of Attribute Name collisions.

            



**Excel Options**



The following options 
are additional options that are available when we exporting to an Excel file:


- **Export File Name**:  This is 
 the name that will be given to the export file.
- **Export Folder**: The folder the 
 export file will be created in.

 


**CDS XML Options**



The following options 
are additional options that are available when we exporting to a CDS XML file:


- **Base Export File 
 Name:** This 
 puts a prefix before the XML filename making it unique for this export so 
 that files are not overwritten if the user chooses to export to the same 
 folder they have done so in the past.
- **Export Folder:** The folder the 
 export file(s) will be created in.  Browse to the location where the 
 user would like to save the XML files or type in the location.
- **Export Items by 
 Category:** *[Applies 
 to Item Exports Only]* The default behavior of the CDS XML File Exporter is 
 to write the data to a single file. If this option is selected, then the 
 items will be grouped by category and written out to their own files.
- **Export AVL’s 
 Separately:** *[Applies 
 to Classification Exports Only]*Allowed Values Lists are exported by 
 default within each category and attribute they are associated with.  
 By checking this box, the Allowed Values Lists will be exported at the top 
 of the file in addition to the category and attributes they are associated 
 with.
- **Embed Base 
 Attribute Information in Category Attributes:** *[Applies to 
 Classification Exports Only]* Selecting this option will make sure that 
 when category attributes are exported the base attribute information is 
 also included along with the category specific information.  Not 
 selecting this option will cause the base attribute information to be 
 exported in its own section of the XML file.  Selecting this option 
 increases the size of the file.


**PLM XML Options**



The following options 
are additional options that are available when we exporting to a PLM XML file:


- **Export Folder**: The folder the 
 export file will be created in.
- **Output Item Files 
 by Category**: *[Applies 
 to Item Exports Only]* The default behavior of the PLM XML File Exporter is to 
 write the data to a single file named Items\_<CurrentDateTime>.xml. 
 If this option is selected, then the items will be grouped by category and 
 written out to their own files.
- **Default ICO UOM 
 System**: 
 *[Applies to Item Exports Only]*
When writing out item data to PLM XML each ICO must be 
 either Metric or English.  If the user is exporting item data from a 
 category that contains multiple numeric attributes and those attributes 
 are different UOM systems (metric vs imperial) then this setting will be 
 used to determine what UOM system will be used for the ICO.  All item 
 data that does not match the ICO UOM system will be converted during 
 export to match the UOM system of the ICO.

 


**Export Selections**


 


After 
filling in all the required options the user can click the Next button.  
Whether or not the user has chosen to export classification data or item data 
determines what the user sees next.


 


[**Classification Data Export**](EM_Class.md)


 


[**Item Data Export**](em_items.md)


 


 


 


Return 
to [**Welcome**](hs100.md)page 


 




