---
layout: kbase
title:  "Query - ODBC Refresh Files"
kbid: "12439"
categories: cgs
---

### Windows 10 - Query ODBC Settings for Refresh Files
 
NOTE – Configuring or installing ODBC connections through IBM iSeries is no longer supported.  Users will need to configure the connection through IBM i Access Client Solutions.  While installed by default on the Windows 10 image if missing the software can be reinstalled from Software Center, see kbase IBM iACS - Installing ODBC
 
[Query.ur.com](http://query.ur.com) is accessed from a number of Refresh files used by various departments throughout United Rentals.  For those to run properly the ODBC Administration program will need to be configured on an end user’s machine before they files can access data from [Query.ur.com](http://query.ur.com)

``` 
01. Click on Start

02. Scroll to the bottom of the list of installed applications and expand the Windows 
    Administrative Tools folder
    
03. Launch the ODBC Administration application 32-bit

04. Under the User DSN tab click the Add button

05. Select Client Access ODBC Driver (32-bit) and click Finish

06. Under the General tab enter the following information
    a.  Data source name –   Query
    b.  System – QUERY.UR.COM
    i.  Note – you won’t have the option to drop down the system and select QUERY.UR.COM 
        the first time the ODBC connection is configured, it will need to be manually typed in
    c.  Click Connection Options, select the User Kerberos Principal option
    
07. Click the Server tab
    a.  Under Default SSQL Schema or Library type in WSDATA
    
08. Click OK
```
 
Have the end user open the refresh file, they should not be prompted to enter a password with the connection property having been set to use the Kerberos principal.  If they get a popup when running the refresh to select a data source have them select the connection that was just created.  They may get that prompt multiple times from the same refresh file, select the Query listing and click OK on each popup until the file completes the refresh

Note that we do not support Refresh files beyond getting the ODBC for iACS application package installed and the ODBC data source configured for query.ur.com.  For support on a Refresh file the user will need to reach out to the creator of that Refresh file.windows 

 
For issues with their query account being disabled have them navigate to query.ur.com in a web browser, there will be an option there to enable their query account.

