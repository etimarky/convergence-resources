



CMDescription\_Generator\_IfThenElse - Design For Retrieval (DFR) Help




**Description Generator – Trim and If/or logic**


 


The category processing action **Description Generator** will create 
an issue when the attribute fields being used as the AV are empty.  If the user 
sets up 3 attributes with commas in between and 2 of the 3 attributes were 
empty, the commas will print out in the target attribute consecutively.  


 


For example, a template displaying the following: 


 


<AV:MyAttribute1>, <AV:MyAttribute2>, 
<AV:MyAttribute3> 


 


 And MyAttribute1, MyAttribute2 and MyAttribute3 were all 
empty values would display this in the Target Attribute:


 


            ,,  


 


Use the If/else logic to prevent empty values and replace them 
with alternate text, another attribute or no comma.


 


Operators


·         
== (equals)


·         
!= (not equals)


·         
&& (and)


·         
|| (or)


 


Operations


·         
IF


·         
ELSE


 


Scenarios


·         
Test for null/empty value


 


**Use the IF to test for a null/empty value.** 


 


<TA:MyDescription><IF CONDITION:”AV:MyAttribute1 
!= EMPTY”><AV:MyAttribute1>,<ENDIF>


<IF CONDITION:”AV:MyAttribute2 != EMPTY”><AV:MyAttribute2>,<ENDIF>


<IF CONDITION:”AV:MyAttribute3 != EMPTY”><AV:MyAttribute3><ENDIF>


 


Would generate descriptions like:




<table border="1" cellpadding="0" cellspacing="0" class="MsoTableGrid" style="margin-left:37.9pt;border-collapse:collapse;border:none"><tr><td style="width:41.4pt;border:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="55"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Item#</p></td><td style="width:1.0in;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">MyAttribute1</p></td><td style="width:1.0in;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">MyAttribute2</p></td><td style="width:1.0in;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">MyAttribute3</p></td><td style="width:135.0pt;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="180"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">MyDescription </p></td></tr><tr><td style="width:41.4pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="55"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">1</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">1</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">2</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">3</p></td><td style="width:135.0pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="180"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">1,2,3</p></td></tr><tr><td style="width:41.4pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="55"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">2</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal"> </p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal"> </p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">3</p></td><td style="width:135.0pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="180"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">3</p></td></tr><tr><td style="width:41.4pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="55"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">3</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">1</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal"> </p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal"> </p></td><td style="width:135.0pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="180"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">1</p></td></tr></table>

 


 


·         
Test for a specific value


 


**Use the IF to test for a specific value.  Make sure to enclose the 
value in quotes.** 


 


<TA:MyDescription><IF CONDITION:”AV:MyAttribute1 
== 1”><AV:MyAttribute1>,<ENDIF>


<IF CONDITION:”AV:MyAttribute2 == 2”><AV:MyAttribute2>,<ENDIF>


<IF CONDITION:”AV:MyAttribute3 != EMPTY”><AV:MyAttribute3><ENDIF>


 


Would generate descriptions like:




<table border="1" cellpadding="0" cellspacing="0" class="MsoTableGrid" style="margin-left:37.9pt;border-collapse:collapse;border:none"><tr><td style="width:41.4pt;border:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="55"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Item#</p></td><td style="width:1.0in;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">MyAttribute1</p></td><td style="width:1.0in;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">MyAttribute2</p></td><td style="width:1.0in;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">MyAttribute3</p></td><td style="width:135.0pt;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="180"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">MyDescription </p></td></tr><tr><td style="width:41.4pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="55"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">1</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">1</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">2</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">3</p></td><td style="width:135.0pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="180"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">1,2,3</p></td></tr><tr><td style="width:41.4pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="55"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">2</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">11</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">22</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">3</p></td><td style="width:135.0pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="180"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">3</p></td></tr><tr><td style="width:41.4pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="55"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">3</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">1</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal"> </p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal"> </p></td><td style="width:135.0pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="180"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">1</p></td></tr></table>

 


 


·         
Use the AND/OR


 


**Use AND** 



<TA:MyDescription><IF CONDITION:”AV:MyAttribute1 == 
1 && AV:MyAttribute2==2”>GOODVALUES<ENDIF>


Would generate descriptions like: 




<table border="1" cellpadding="0" cellspacing="0" class="MsoTableGrid" style="margin-left:37.9pt;border-collapse:collapse;border:none"><tr><td style="width:41.4pt;border:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="55"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Item#</p></td><td style="width:1.0in;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">MyAttribute1</p></td><td style="width:1.0in;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">MyAttribute2</p></td><td style="width:1.0in;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">MyAttribute3</p></td><td style="width:135.0pt;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="180"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">MyDescription </p></td></tr><tr><td style="width:41.4pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="55"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">1</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">1</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">2</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">3</p></td><td style="width:135.0pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="180"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">GOODVALUES</p></td></tr><tr><td style="width:41.4pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="55"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">2</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">11</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">22</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">3</p></td><td style="width:135.0pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="180"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal"> </p></td></tr><tr><td style="width:41.4pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="55"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">3</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">1</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal"> </p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal"> </p></td><td style="width:135.0pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="180"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal"> </p></td></tr></table>

 


**Use Multiple AND OR** 


 


<TA:MyDescription><IF CONDITION:”AV:MyAttribute1 == 
0 && AV:MyAttribute2==2 || AV:MyAttribute3==3“>GOODVALUES<ENDIF>


Would generate descriptions like: 




<table border="1" cellpadding="0" cellspacing="0" class="MsoTableGrid" style="margin-left:37.9pt;border-collapse:collapse;border:none"><tr><td style="width:41.4pt;border:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="55"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Item#</p></td><td style="width:1.0in;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">MyAttribute1</p></td><td style="width:1.0in;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">MyAttribute2</p></td><td style="width:1.0in;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">MyAttribute3</p></td><td style="width:135.0pt;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="180"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">MyDescription </p></td></tr><tr><td style="width:41.4pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="55"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">1</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">1</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">2</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">3</p></td><td style="width:135.0pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="180"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">GOODVALUES</p></td></tr><tr><td style="width:41.4pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="55"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">2</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">11</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">22</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">3</p></td><td style="width:135.0pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="180"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">GOODVALUES</p></td></tr><tr><td style="width:41.4pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="55"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">3</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">0</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">2</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal"> </p></td><td style="width:135.0pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="180"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">GOODVALUES</p></td></tr></table>

 


\***Note**: Currently, multiple 
conditions are allowed for && and ||, however the order of precedence 
is from left to right.  Grouping conditions could be supported in the future, 
but it would be necessary to add support for parenthesis to show order of 
operation. 


For example, the following are valid:


<IF CONDITION:”AV:MyAttribute1 == 1 && 
AV:MyAttribute2==2 || AV:MyAttribute3==3”>


<IF CONDITION:”AV:MyAttribute1 == 1 || 
AV:MyAttribute2==2”>  
  



The following are invalid:


<IF CONDITION:”AV:MyAttribute1 == 1 && 
(AV:MyAttribute2==2 || AV:MyAttribute3 == 3”)>


<IF CONDITION:”(AV:MyAttribute1 == 1 || 
AV:MyAttribute2==2) && AV:MyAttribute3 ==3”>


**Use ELSE** 


 


<TA:MyDescription><IF CONDITION:”AV:MyAttribute1 
== 1”> <AV:MyAttribute1>,<ELSE> BADVALUES<ENDIF>




<table border="1" cellpadding="0" cellspacing="0" class="MsoTableGrid" style="margin-left:37.9pt;border-collapse:collapse;border:none"><tr><td style="width:41.4pt;border:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="55"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">Item#</p></td><td style="width:1.0in;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">MyAttribute1</p></td><td style="width:1.0in;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">MyAttribute2</p></td><td style="width:1.0in;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">MyAttribute3</p></td><td style="width:135.0pt;border:solid windowtext 1.0pt; 
  border-left:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="180"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">MyDescription </p></td></tr><tr><td style="width:41.4pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="55"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">1</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">1</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">2</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">3</p></td><td style="width:135.0pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="180"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">1</p></td></tr><tr><td style="width:41.4pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="55"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">2</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">11</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">22</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">3</p></td><td style="width:135.0pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="180"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">BADVALUES</p></td></tr><tr><td style="width:41.4pt;border:solid windowtext 1.0pt; 
  border-top:none;padding:0in 5.4pt 0in 5.4pt" valign="top" width="55"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">3</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">1</p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal"> </p></td><td style="width:1.0in;border-top:none;border-left:none; 
  border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="96"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal"> </p></td><td style="width:135.0pt;border-top:none;border-left: 
  none;border-bottom:solid windowtext 1.0pt;border-right:solid windowtext 1.0pt; 
  padding:0in 5.4pt 0in 5.4pt" valign="top" width="180"><p class="MsoNormal" style="margin-bottom:0in;margin-bottom:.0001pt;line-height: 
  normal">1</p></td></tr></table>

 


 


Return to [Using the Description Generator](CM-Using%20Description%20GeneratorMenu.md) 


 


 




