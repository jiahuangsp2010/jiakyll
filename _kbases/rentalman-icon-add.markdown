---
layout: kbase
title:  "Rentalman - Icon Add"
kbid: "11499"
categories: cgs
---

## IBM iACS – Create Rentalman Icon

 

 

**Note** – IBM i Access Client Solutions uses a new file extension, HOD, for the 5250 emulation.  WS files will still open an IBM Client Solutions for Windows emulated sessions.

 

**Option 1 – Copy pre-built icon**

 

During the install of IBM I Access Client Solutions a default icon with all the default settings already saved was placed in the program’s install directory – C:\Program Files (x86)\IBM\i Access Client Solutions\Rentalman.HOD

 

1. Open Windows Explorer and navigate to the install directory – C:\Program Files (x86)\IBM\i Access Client Solutions\

 

2. This file - Rentalman.HOD can be copied to a convenient location for the end user such as the desktop or the home drive

 

    a. Right click on the file and select Copy

 

    b. Navigate to the destination the end user would like the icon to be, right click and select Paste.

 

3. Note – Creating a shortcut to this icon will cause an error message whenever the end user closes the application since settings cannot be saved to the file.

 

**Option 2 – Create new icon**

 

1. Click on Start and click All Programs

 

2. Scroll down and expand the IBM i Access Client Solutions folder

 

3. Open the ACS Session Manager

 

4. Click New Display Session

 

5. Session Manager will open a new window that will prompt you for the information needed for the sessions:

 

    a. Click the Connection option

        i. Session Name – Rentalman

        ii. Destination Address – RM.UR.COM

        iii. Destination Port – 992

        iv. Protocol – Telnet – TLS/SSL

        v. Screen Size – 27x132

 

    b. Click the Advanced option under Connection

        i. Password Prompting – Use Kerberos authentication; do not prompt

        ii. Bypass signon - Yes

 

6. Click OK and a new 5250 emulation window will open up and automatically sign in

 

7. After they have logged in and the application is showing the login screen for Rentalman click File and click Save As



8. Save the new session to a convenient location such as the end users Home drive or Desktop

 