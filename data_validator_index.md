



Data\_Validator\_Index - Design For Retrieval (DFR) Help




**Data Validator**


 


 


The Data Validator Module validates a specific batch of data 
against any validation criteria that has been defined in the DFR 
software.  Validations can be customized using [Configuration Objects](javascript:popuplink('hs1903.htm')) to cover 
any specific validation tests a user may require.  


 


The purpose of running validations is to automatically inspect 
data to confirm that attribute values match the expected input, and flag any 
validation errors. This should be performed prior to an export of this data, or 
to mitigate potential problems with future use of the data in other 
systems.  For example, if a user wants to publish data from DFR to a PLM 
or ERP system, the user will want to make sure there are no errors in the data 
that could interfere with the loading of the data or the use of the data in 
those systems.


 


**Standard Validations**


DFR provides a standard set of validation routines that may be run 
against a batch of data. These include:


- Confirmation of 
 data type.
- Verification 
 that the data is within an allowable range.
- Verification 
 that the data does not exceed defined lengths.
- Verification 
 that there are no null values.
- Authentication 
 against a mask defined through the use of regular expressions.

 


**Allowed Value Lists**


In addition to the validations listed above, a user may use the [Allowed Values 
Manager](hs7000.md) to define a list of values that are allowed for an attribute. 
This is particularly useful when checking the validity of string data type 
values, or when checking for specific numeric values rather than a range of 
values.


 


**When to Run Validations**


Data Validator is run after attribute values have been imported 
and checked using the Data Developer. During data development, the assigned 
user has the opportunity to manually review the data, check for duplicates and 
check attribute data against any allowed values lists. Then, running the Data 
Validator continues this process by flagging items that do not match basic 
criteria. 


 


[Setting up the 
Validations](hs5010.md)


 


[Running a Validation](hs5020.md)


 


[Using the Allowed 
Value Manager](hs7000.md)


 


Return to [**Welcome**](hs100.md)page 


 




