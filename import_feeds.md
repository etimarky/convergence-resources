



Import\_Feeds - Design For Retrieval (DFR) Help



# Import Feeds


**Import Feeds**can be configured to import a file and update items in the background of the application.


- Used to automate importing data to update items
- Triggers are defined by time
- Example: a feed can be configured to watch an SFTP folder and automatically import a file added there


*Note: Import feeds are not connected to a particular deliverable. For more information on deliverable import feeds, **[click here](deliverable-import-feeds)**.*


 


## How to Set Up an Import Feed


1. Click the button for new import feed.  

![](assets/image(138).png)




**Feed Details**


2. Name your feed and write a description.


3. Set the Type of feed (will this feed be editing **Items** or the **Classification Structure**?).


4. Set the fail severity (recommended: **Error**).


![](assets/image(140).png)




 


**Trigger Details**


5. Select the desired trigger that will kick off the import feed.


For a standard import feed, the selection will typically be **SFTP File Watcher**.


This means that the feed will monitor your designated SFTP location and import any file found.


![](assets/image(142).png)




6. Select the endpoint to use (**[click here for instructions on configuration](endpoint-management)**).


7. Identify the Path (i.e. the folder path where the watcher will look for new files)


8. Choose your polling interval (default is set to check every 5 seconds for a file)


 


**Source and Format Details**


9. Choose Formatter (Excel)


10. Add source (SFTP file) and details (endpoint, path, and local file name)


\*Local file name can be anything you want


![](assets/image(143).png)




**Status Handler Details**


11. Click through this; no additional status handlers need to be configured.


 


**External Data Model Details**


12. Choose the external data model associated with the import.


You can either click on the magnifying glass to view existing data models or the + icon to add a new data model. (For instructions on setting up an external data model, **[click here](external-datamodel-management)**.)


![](assets/image(144).png)




13. Toggle the Active status "on" and click Save.


![](assets/image(145).png)




 


Your import feed is now configured and active.


 


**Related Pages:**


- **[SmartFeeds Overview](smartfeeds)**
- **[Feed Manager](default-template-4)**- How to view and manage import feeds
	- **[Deliverable Import Feeds](deliverable-import-feeds)**- How to set up a deliverable import feed
- **[EndPoint Management](endpoint-management)** - How to view, manage, and edit configured endpoints
- **[External Data Model Management](external-datamodel-management)** - How to view and manage external data models



