



Running\_a\_Validation - Design For Retrieval (DFR) Help



**Running a Validation**


 


Once the validations have been defined and data cleansing has been performed in the Data Developer, a validation is run against the data using the Data Validator. 


 


**To perform validations on a batch of data, the data must be assigned to the user.** 


**To run a validation:**


- Open the Data Validator Module.

 


- Press the down arrow to the right of the **Batch** field and select thebatch to be validated.

 


- Press the down arrow to the right of the **User** field and select the owner of the batch.

 


- Press the down arrow to the right of the **Status** field and select the status of the items to be validated.

 


- Press the down arrow to the right of the **Error Type** field and select the type of validation to be run. This field will list the standard validation routines as well as any site specific, or custom validations included in the installation.

 


- If an Allowed Values List has been used to restrict the attribute to a specific set of values, check the **Restrict to Allowed Values** check box.

 


- Move the cursor through the classification tree opening categories to expose the target category. Select the target category.

 


- Press the **Retrieve** button to retrieve and display the data.

 


The Data will be displayed in spreadsheet format. The [spreatsheet display can be customized](javascript:popuplink('hs4020.htm')) to better view the data.


 


If the data has been validated in the past, that date will be displayed in the **Last Validated:** field.


 


- Press the **Validate** button to begin the validation. A **Validation Progress** window will appear and report the progress of the validation.

 


- A **Validation Complete** window will confirm that the operation has concluded. Press **OK**.

 


**To retrieve the validation results:**


 


Attribute fields containing errors will be shaded in pink.


 


- Use the arrows at the right and bottom of the spreadsheet to scroll through the data. Attribute fields containing errors will be shaded in pink. Run the cursor over the pink shaded fields to view the error.

 


- Press **View Report** to generate a detailed report of the validation. Each item in the batch will be listed along with its current status.

 


**To fix validation errors:**


 


Validation errors can be corrected in the Data Validator spreadsheet in the same manner as in the Data Developer Module. Once the errors have been corrected, save the changes by pressing the **Save to DB** button at the top of the screen.


 


 


Return To [Data Validator](data_validator_index.md)





