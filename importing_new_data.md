



Importing\_New\_Data - Design For Retrieval (DFR) Help



# Importing Segment Data


As it stands, segment and fastener data are the only data that can be imported into Convergence PIM SmartTeardown. 


Structure and Model importing is not a function that Convergence PIM supports. 


 


The first thing that needs to be done before a user can consider importing segment or fastener data is verify that General Management and Family Management are set up correctly. 


Some fields will be utilized as drop-down fields based on information in either of those administrative areas. 


 


**Models must be added manually**, and **structure must be built out manually** before importing can begin.  ( <--these will contain hyperlinks)


 


Once structure is built out, the user can export the family structure template in Family Management. 


 


![](assets/image(75).png)




 


The family export will appear exactly as displayed below:   

 


The user at this point can fill out any and/or all information on the first 2 tabs: Segment Data and Fastener Data. 


Areas such as **Region** and **Model** are mandatory.


 


Remember: the **model** that data is being imported to has to have been previously created. Please see " Adding A Model" for more information.
Areas under Region, Material, Manufacturer, Primary Process, Secondary Process and Type are all based on information added into General Management. These will appear as drop-down lists and cannot be written over. 


 


![](assets/image(76).png)




 


Fill out all necessary information in the template and save. 


 


![](assets/image(77).png)




 


Navigate to the Convergence PIM ThickClient and select Import Manager. 


Select Teardown Data. 


 


![](assets/image(78).png)




 


Once asked to choose the import format, there will be only one choice: this is for product data. 


 


![](assets/image(79).png)




 


The next screen is specifically asking what type of data is being loaded. 


It's possible to load segment data without fastener data and vice versa as long as the segments do already exist. 


In this case, data is on both the segment and fastener tabs so both are being imported and therefore both will be selected. 


 


![](assets/image(80).png)




 


The operation will be "create" on both Segment and Fastener data screens since although the user already created a model, they are now creating new segment data for that model. 


All other fields will be auto-mapped if the user is using the family template as recommended. 


 


![](assets/image(81).png)




 


As long as validations clear, the import can be completed. 


Now when navigating to SmartTeardown's home screen, select the family, manufacturer and then model. 


The final screen should appear as shown below: to the right now displays fastener and segment data. 


Gray nodes in the middle of the screen up and down the hierarchy indicate no data. Orange indicates data whether that's just segment data (on the top such as height, width, length) or fastener data displayed in terms of fastener type, location, total weight, etc. 


  

![](assets/image(82).png)




 


Lastly, there is an export function on this model screen as well


 


![](assets/image(83).png)




 


This export feature will only export information that is not blank: fastener and segment data. It will not import empty cells or total hierarchy if there is no data to show. 


 


![](assets/image(86).png)




 


![](assets/image(85).png)




 


 


 



