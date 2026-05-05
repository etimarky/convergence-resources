



Custom\_Attributes - Design For Retrieval (DFR) Help




**Custom 
Attributes**


 


 


An attribute can have special properties to achieve certain 
functions.  This section describes some examples of DFR’s custom 
attributes.


 


**Vectors**


 


Vectors can have many **numeric attributes** associated with them.  
A numeric attribute can belong to multiple vectors.  Each attribute that 
belongs to a Vector custom attribute must be listed in the CustomDataConfig 
attribute property field.  Each attribute that comprises a vector can have 
different Units of Measure.  A vector can have any name you choose.  
Here are the attribute properties for a Vector custom attribute:


 




<table border="0" cellpadding="0" cellspacing="0" class="MsoNormalTable" style="border-collapse:collapse"><tr><td style="width:2.0in;border:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="192"><p class="MsoNormal"><b><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>Property Name</span></b></p></td><td style="width:1.25in;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="120"><p class="MsoNormal"><b><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>Value</span></b></p></td><td style="width:185.4pt;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="247"><p class="MsoNormal"><b><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>Description</span></b></p></td></tr><tr><td style="width:2.0in;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="192"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>CustomData</span></p></td><td style="width:1.25in;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="120"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>Vector</span></p></td><td style="width:185.4pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="247"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>The type of CustomData attribute is Vector.</span></p></td></tr><tr><td style="width:2.0in;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="192"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>CustomDataConfig</span></p></td><td style="width:1.25in;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="120"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>Length|Width|Height</span></p></td><td style="width:185.4pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="247"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>These are the attributes that make up the vector.  These 
  attributes are separated by a vertical slash.  The values listed here 
  are illustrative.  <b>The attribute names must match the sentence case 
  in DFR.</b></span></p></td></tr></table>

 


 


**Ranges**


 


Range custom numeric attribute has just two numeric associated 
with the limits of the range.  Like vectors each numeric attribute that 
makes up a range can have different Units of Measure, though it’s more common 
to have the same Units of Measure.  Here are the attribute properties for 
a Range custom attribute:


 




<table border="0" cellpadding="0" cellspacing="0" class="MsoNormalTable" style="border-collapse:collapse"><tr><td style="width:2.0in;border:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="192"><p class="MsoNormal"><b><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>Property Name</span></b></p></td><td style="width:1.25in;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="120"><p class="MsoNormal"><b><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>Value</span></b></p></td><td style="width:185.4pt;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="247"><p class="MsoNormal"><b><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>Description</span></b></p></td></tr><tr><td style="width:2.0in;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="192"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>CustomData</span></p></td><td style="width:1.25in;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="120"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>Range</span></p></td><td style="width:185.4pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="247"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>The type of CustomData attribute is Range.</span></p></td></tr><tr><td style="width:2.0in;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="192"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>CustomDataConfig</span></p></td><td style="width:1.25in;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="120"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>Max Pressure|Min Temperature</span></p></td><td style="width:185.4pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="247"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>These are the attributes that make up the vector.  These attributes 
  are separated by a vertical slash.  The values to the left are 
  illustrative.  <b>The attribute names must match the sentence case in 
  DFR.</b></span></p></td></tr></table>

 


**MultiVal**


 


MultiVal custom attributes can support multiple attribute 
values.  Each attribute value can be either a string or integer, units of 
measure are not supported for MultiVal attributes.  Here are the attribute 
properties for a MultiVal custom attribute:


 




<table border="0" cellpadding="0" cellspacing="0" class="MsoNormalTable" style="border-collapse:collapse"><tr><td style="width:2.0in;border:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="192"><p class="MsoNormal"><b><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>Property Name</span></b></p></td><td style="width:1.25in;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="120"><p class="MsoNormal"><b><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>Value</span></b></p></td><td style="width:185.4pt;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="247"><p class="MsoNormal"><b><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>Description</span></b></p></td></tr><tr><td style="width:2.0in;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="192"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>CustomData</span></p></td><td style="width:1.25in;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="120"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>MultiVal</span></p></td><td style="width:185.4pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="247"><p class="MsoNormal"><span style='font-size:10.0pt;font-family:"Arial",sans-serif; 
  color:black'>The type of CustomData attribute is MultiVal.</span></p></td></tr></table>

 


 


Return 
to [Attribute 
Manager](hs2000.md)


 


 




