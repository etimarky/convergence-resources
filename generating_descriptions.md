



Generating\_Descriptions - Design For Retrieval (DFR) Help



# Generating Descriptions


The Description Generator is a useful tool when mass-creating multiple descriptions for any attribute, built on multiple attribute values concatenated.


 




<iframe src="https://www.youtube.com/embed/-XfBjI23Y_A/?wmode=transparent" width="560" height="315" frameborder="0" allowfullscreen></iframe>


 


 


 


The Description Generator is located in the ThickClient under it's own section: Description Generator


  

![](assets/image(1134).png)




 


 


The screen you are immediately directed to is the Description Generator.


Template Validator is also shown as a separate tab.  This functionality is explained in "Fixing Validation Errors," shown [here.](#)


 


Note in the top right that there are two options: Configure and Run.


Create a new template by selecting the green plus symbol.


Name the new template and select " Save Template."  

  

![](assets/image(1135).png)

  

 


Choose the target attribute. 


The target attribute will be the attribute in which descriptions will be generated.


Select the target attribute and then on the bottom right, select " Insert" and then "Target."


 


![](assets/image(1136).png)




 


Now your attribute is selected and you can begin building your description.


 


The next string of attributes will make up your description.


Select an attribute and select "insert."


 


![](assets/image(1137).png)

  

 


From there, options will allow the user to input the *attribute **name**- which will appear as the attribute name and not the value.*


The option is also available to input the *attribute **value**, such as "50V" or " Compressor."*  

 


If the attribute value has a Unit of Measure, that can also be applied using the "**Value with UoM**" function or by manually typing it at the end of the attribute value. *This would allow the "Volt" Unit of Measure to appear as in the example above.*


 


The last most commonly used function is the **abbreviation** function. This is set up in the Allowed Values section of SmartClass and the description generator *will pull that abbreviation into the description.*  

 


After adding all of the desired attributes with their values, names or abbreviations, save the template.


In the top right, change from Configure to Run.


 


 


It is important to note that the only attribute that is not listed in the Description Generator attribute list is the Item Description.   

For this example, I am going to use that function.   

Instead of " <TA:Standards>, I will use " **<TD>**  

The **"TA" stands for Target Attribute**, whereas **"TD" stands for Target Description.**
 


![](assets/image(1138).png)




 


On this screen, there will be a few options.  

To begin with, the top of the screen will display the category that the template is going to be generation descriptions in, as well as displaying the template the user created.


It is important to mention that the template cannot be changed from this screen. That would have to be in the Configure screen again.  

 


![](assets/image(1139).png)




 


If your template is set up correctly, the template name will appear in a drop down list under the template display.


Alternatively, if the template is not set up correctly, it will not show up and the user will have to either change the template, or change the drop down action from Description Generator to Description Template Validator and select validate.


For more on fixing validation errors, click [here.](#) 


 


![](assets/image(1140).png)




There are 3 boxes that can be checked.


1. One will allow generation of descriptions that are in an in-work, pending or approved status, meaning new and rejected will not be touched.
2. One will allow generation of descriptions only in the in-work status, meaning that anything in new, pending, approved or rejected won't be included.
3. One will restrict the items being worked on to specifically those under the users name who is logged in.
	1. The last option, restricting items to assigned user can be combined with the first two options.
4. There is one more option that will restrict items being worked on to a particular batch or deliverable.


        This means that only items within that batch or deliverable will be worked on.  

 


Now select Run on the bottom right.


 


A box will be prompted that displays the amount of descriptions generated.


 


![](assets/image(1141).png)




 


To check your work, locate the category in Data Developer or SmartFind and view the generated descriptions.


 


![](assets/image(1142).png)




 



