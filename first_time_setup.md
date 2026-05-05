



First\_Time\_Setup - Design For Retrieval (DFR) Help



# First Time Setup


In order for your exports from DFR to Teamcenter to work, there are a few Items you must set up before your first export. 


 


## Attribution Script


The first thing you will need to do before proceeding is contact your CDS Representative and make sure all the correct Attribution scripts have been run in your environment in order to follow the steps below. Some Attribute values may not be available to you unless this has been done.


 


## Mapping to UoMs


In Teamcenter:


Locate UoM Definitions in Teamcenter


Unit Definition Class - Open in Classificaiton


Search for the Unit you are using, or do a blank search to see all


See Table Image.


 


![](assets/img1(2).png)




Note Object ID for chosen UoM(s)


 


In DFR:


First, configure UoM(s) are all correct in DFR.


Please contact your CDS representative, or refer to the information [here](#) to make sure your UoMs are properly set up.


 


Open the Export Manager Module


Select Classification Export


Select PLM Export Type


Hit Settings to open PLM Export Settings


 


![](assets/img2(1).png)




 


Enter Object ID in Teamcenter Unit Of Measure Column for all items needed


You have the ability to Save (export) or Load files as well.


These settings save automatically, and will now correctly map in future exports


 


## Settings for IDs


When it comes to setting your Teamcenter IDs for Attributes/LOVs, there are a few different options:


 


**Manual Load**


You can load a file with this information configured, and DFR will update the attributes to have the matching IDs. This may be necessary if loading into an existing Teamcenter Environment.


 


**Automatically Assign**


You can specify a staring ID Number (must be a positive integer) and DFR will create and assign the IDs to Attributes throughout the tree. This will follow the rules outlined in [(Best Practices - Abstract Classes)](#)


At a high level, this will add a unique ID to any attribute with a unique name. Any repeated occurrences will have the same ID.


This will occur when you select "Regenerate Teamcenter IDs" on Export (See [PLMXML Export](#) for examples)


 


**Manual Override**


After automatically assigning the IDs, you could go back to any attribute, and manually set the ID if only some need to be specified.


 


**LOV IDs**


LOV IDs operate the same as Attribute LOVs except they are **ALWAYS NEGATIVE**.


These can be assigned in any of the three ways mentioned above as well. LOV lists will be created and imported into Teamcenter even if they are not used, if they have an ID created and assigned to them. 



