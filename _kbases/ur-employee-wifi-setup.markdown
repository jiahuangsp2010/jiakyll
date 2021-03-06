---
layout: kbase
title:  "UR-Employee WIFI Setup"
kbid: "12362"
categories: cgs
---

## Windows 10 – Connecting to UR-Employee
 
 
While the Settings app in Windows 10 (and by proxy the wi-fi icon on the taskbar) gives us the options to connect to most wireless networks we can’t make the settings changes needed there to properly connect to UR-Employee
 
By default the connection for UR-Employee should be created on all Windows 10 computers through an SCCM policy so first attempt to connect to the network from the taskbar wi-fi icon.  If the user is prompted for a User ID and Password click Cancel and follow these steps to create the wireless connection:
 
1. Click on Start
 
2. Scroll down and expand the Windows System folder
 
3. Launch Control Panel
 
4. Click Network and Sharing Center
 
5. Click Set up a new connection or network
 
6. Select Manually connect to a wireless network and click Next
 
7. Enter the following information
 
    a. Network Name: **UR-Employee**
 
    b. Security Type: **WPA2-Enterprise**
 
8. Click Next
 
9. Click Change Connection Settings
 
10. Click the Security tab
 
11. Click the Settings button next to network authentication method drop down
 
12. **Uncheck the box to Validate Server Certificate**
 
Click OK on all the windows for the wireless networks and connect to UR-Employee from the taskbar wi-fi icon.
 
If you need to delete the UR-Employee wireless profile on a computer to retry the steps to create it do the following:
 
1. Click on Start
 
2. Scroll down and launch Settings
 
3. Click Network and Internet
 
4. Click Wi-Fi
 
5. Click Manage Known Networks
 
6. Click the listing for UR-Employee then click Forget