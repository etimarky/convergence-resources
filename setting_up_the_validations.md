



Setting\_up\_the\_Validations - Design For Retrieval (DFR) Help



**Setting up the Validations**


 


Validations are performed against one batch of data at a time. The batch may be the original batch loaded with the Item Loader module, or it may be a temporary batch created in the Item Browser.


 


The first step in running a validation is to define the rules for the data validation in the Classification Manager Module.


 


**A user must be assigned the Category Developer role.**


 


**To set up Validation Rules in the Classification Manager:**


 


- Select the Classification Manager Module.

 


- Move the cursor down the classification structure opening categories until the target category has been selected.

 


- The attributes assigned to this category will be listed in the right hand column. Select the attribute for which the validation criteria will be set.

 


- Right click on the attribute and select **Edit…**

 


Validation criteria are set in the **Validation:** section of the Attribute Editor window. 


 


- **Range Validation** is available for Numeric and Integer data types. When the Range Validation box is checked, the **Lower limit** and **Upper limit** boxes are activated. Enter the upper and lower values that consititute a valid range of values for the attribute. An attribute value outside of this range will trigger a validation error.

 


- **String data** can be checked against a mask that is defined using regular expressions. The **Mask** field is available for String data types only.
- The Data Validator automatically checks for **data type**. The DFR data base stores all attribute values as string data. However, it automatically checks the data against the data type to make sure it will translate properly to the data type specified in the attribute definition.
- The user may specify whether a value is required for the attribute or if a NULL value is allowed. A check in the Required field indicated that a value must be entered for the attribute. The attribute column header will be displayed in red in the Data Developer Module, and a NULL value will trigger a validation error.
- When the validation criteria have been entered, press the **Save** button to exit the Attribute Editor window.

 


Return To [Data Validator](data_validator_index.md)





