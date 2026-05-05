



Loading\_DFR\_Export\_into\_Teamcenter - Design For Retrieval (DFR) Help



# Loading CDS PIM Export into Teamcenter


 


In order to load your data into Teamcenter, first it must be exported correctly from CDS PIM. Please see [(First Time Steup)](#) and [(PLMXML Export)](#) for instructions on creating the proper files.


 


These instructions assume that you are loading into a blank Teamcenter instance. For loading into existing Teamcenter classification structures, please contact Siemens with any additional questions.


This documentation assumes you have login information to an admin account in Teamcenter. 


 


**Locate CDS PIM Export XMLs**


Make sure you have access to the XML Files you have created from CDS PIM. For a full load into Teamcenter, there should be 4 files:


LOV


Attributes


Classification 


Items.


 


**Modify Classification file**


In order to correctly upload to a blank Teamcenter instance, you will need to manually modify the Classification.plmxml file. 


Open the file and look for the following line:


![](assets/image(905).png)




The <Parent> Tag value will need to be modified to say "ICM" (like the image above) instead of whatever it currently reads. This will allow the "Parts" level of your classification to sit at the top of the structure in Teamcenter.


 


**Teamcenter Load**


Open your Teamcenter instance and select the "Classification Admin" Module


You will want to expand the SAM Classification Root and select the "Classification Root" Object


 


![](assets/image(907).png)




 


With Classification Root selected, press the "Import Objects" Button


 


![](assets/image(908).png)




 


You will see the following pop-up:


 


![](assets/image(909).png)




 


Using the PLMXML Option, select the first file you want to import into Teamcenter. This should be the LOV.xml file


Make sure to use the "incremental\_import" Transfer mode. 


Hit Import and you should see a notification that your import completed successfully. You can click the "Yes" button to see the full import log. (A full log will be created in the same directory as the file you uploaded as well)


 


![](assets/image(910).png)




 


**Teamcenter Load: Repeat**


Repeat these steps for the remaining files in the following order:


LOV, Attributes, Classification, Items


Each time you complete a load,you should receive a notification that your import was completed.


 


![](assets/image(910)_1.png)




 


Once you have loaded all 4 part of the structure, refresh the Teamcenter Classification Window and you will see your newly loaded structure!


 


![](assets/image(921).png)





