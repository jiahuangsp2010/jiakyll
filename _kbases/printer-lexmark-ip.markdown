---
layout: kbase
title:  "Printer - Lexmark - IP Configuration"
kbid: "10380"
categories: cgs
---

### Configure the IP on a Lexmark Printer

 
```
01. Obtain the current IP address of the printer from the configuration page
    a. Lexmark e250dn - Hold down the green button until paper prints.
    b. Lexmark T630 series – MENU > UTILITIES > PRINT SETUP
    c. Lexmark T644 X644 X654 – MENU > REPORTS > NETWORK SETUP
    
02. Open Internet Explorer and go to http://X.X.X.X (X = IP Address from config page) 

03. Click on "Settings"

04. Under Other Settings click on "Network/Ports"

05. Click on TCP/IP

06. Click "Set static IP address" next to the current IP address.

07. Set the "IP Address" to the correct IP format 
    a. Ex: 10.72.155.51 (printers should be in range from .50-.69)
    
08. Click Submit Changes.

09. Wait about 30 seconds and try to navigate to the new IP Address http://X.X.X.X  
    and you should see the screen from step 2.

10. If you see this the new IP has been configured correctly.

11. If necessary, change the password in Rentalman to align with the new IP.
```