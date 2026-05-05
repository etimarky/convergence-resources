



Deliverable\_Import\_Feeds - Design For Retrieval (DFR) Help



# Deliverable Import Feeds


**A deliverable import feed**is tied to a SmartTrack deliverable. The import is triggered when an item in a deliverable reaches a certain task. 


 


To support this, a specific task type is used in the deliverable configuration: **AutoEnrich**.


 


**Use Case****:**This feature was created to support automatic enrichment of item data using an API from an external database. In the example below, you will see the feed configured using a SiliconExpert API. The end result is that an item in this deliverable will have an attribute bounced off the SiliconExpert database and relevant attribute values will be automatically pulled into Convergence PIM in the item's record.


 


**Setting Up a Deliverable Import Feed**


The simplest way to do this is directly in a deliverable. You will need to have already configured an **[endpoint](endpoint-management)** and an **[external data model](external-datamodel-management)**.


 


1. Navigate to [**SmartTrack**](https://convergencedata.helpdocsonline.com/smarttrack) and the deliverable you want to associate with the import feed. Open the configuration for the deliverable by clicking on the wrench icon (or navigate through Manage Deliverables at the top right of the page).


![](assets/image(146).png)




 


2. Identify which task you want to use for Auto Enrichment. It can be any step in the deliverable but it is recommended to not be first or last.


 


3. Set the Task Type to AutoEnrich.


![](assets/image(147).png)




 


4. A dropdown titled Deliverable Feed will appear next to the Task Type field when AutoEnrich is selected.


 


5. If a deliverable import feed has already been configured, you can select from the dropdown menu. Otherwise, click Add Feed.


 


![](assets/image(148).png)




 


6. Follow the steps in the feed configurator.


 


**Feed Details**


7. Name and describe your feed. Choose the fail severity (recommended: Error).


Note: The Type will default to items as the feed is - by design - meant to enrich item data.


![](assets/image(149).png)




**Trigger Details**


8. The Trigger will default to **DFR Item Trigger**. You do not need to add a Status Filter or Batch Filter.


9. If desired, edit the Polling Interval (default is 5 seconds).


![](assets/image(150).png)




**Source and Format Details**


10. Choose SiliconExpert for the Formatter and Source.


11. Select your desired endpoint (e.g. SiliconExpert API Endpoint).


12. Select your Desired Attribute. This is the attribute that will be referenced when searching the SiliconExpert database.


![](assets/image(151).png)




**Status Handler Details**


13. Click through this step; no changes are necessary.


 


**External Data Model Details**


14. Select the external data model to use. In this use case, we have selected the SiliconExpert data model which has been mapped to Convergence PIM attributes.


15. If desired, you can attempt to auto-map fields, which will work on non-mapped attributes. If there is an exact match to the attribute name between SiliconExpert and Convergence PIM, the system can auto-map.


![](assets/image(152).png)




16. Toggle the feed as Active and click Save.


![](assets/image(153).png)




**Confirm Deliverable**


17. When returned to the deliverable configuration page, review the steps to ensure the process is flowing as desired.


In the example below, the items will be automatically enriched by the SiliconExpert database when an item reaches the Auto-enrichment step (A) and its status is "Enrichment In Progress" (B). Once the enrichment is complete, the item will automatically move to the next step (Final Review) and the status will be changed to "Enrichment Complete" (C).


![](assets/image(154).png)




 


**Related Pages:**


- **[SmartFeeds Overview](smartfeeds)**
- **[Feed Manager](default-template-4)**- How to view and manage import feeds
	- **[Deliverable Import Feeds](deliverable-import-feeds)**- How to set up a deliverable import feed
	- **[Import Feeds](default-template-1730124762)** - How to set up an import feed
- **[EndPoint Management](endpoint-management)** - How to view, manage, and edit configured endpoints
- **[External Data Model Management](external-datamodel-management)** - How to view and manage external data models



