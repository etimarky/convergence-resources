



SmartLink - Design For Retrieval (DFR) Help



# SmartLink


**SmartLink** is a type of integration that allows external applications to display hyperlinks that allow a user to "jump into" Convergence PIM and view the details of a particular item or items.  


 


This type of integration works best when the customer is trying to keep custom development to a minimum and/or the application they are extending has very limited capabilities.  


 


In order to provide the best user experience when jumping from one application to another, it is preferable to have Single Sign On (SSO) in place between Convergence PIM and the source application so that the user is not forced to log in when they navigate into the Convergence PIM application.


 


The SmartLink syntax for viewing a particular item/item(s) is as follows:


 


           **https://<Convergence PIM Web application root URL>/<catalog>/link/search?itemNum=<item number>**


 


**<Convergence PIM Web application root URL>** - Convergence PIM Online's base URL


**<catalog>** - The Convergence PIM catalog containing the item


**<item number>** - The Convergence PIM Item Number you wish to see (This could be a part number or product number depending on the data)



