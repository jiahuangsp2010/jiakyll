---
layout: kbase
title:  "Rentalman - Only - Print Issue"
kbid: "10664"
categories: cgs
---

User can’t print from RM, but can still print Local Documents i.e. Office Products from Windows like Email, Word, Excel, etc.


1. Have the user hit F11 from any main Rentalman menu and inform you of the Printer ‘Sts’ (Status)

 

2. If Sts is END, user can use Option 1 to Start, if Sts is MSGW (Message Waiting), the writer needs to be Ended first, then can be started. (see following details on how to End the writer).

 

**NOTE:** Two of the main reasons a printer status gores to MSGW are Paper Jam, or Printer running out of Paper. Have user check the physical printer itself to confirm it is ready.

 

1. Obtain the Network Printer name in Question i.e. UR091P22

 

2. From Command line, you will type the command WW, then a space, then UR###* (### will be the location number). Hit <enter>

 

3. Find the Printer in question. If in MSGW status start here, if in END status skip to step 5


    a. Most users can hit F11 from any main Rentalman Menu at the location level and do these same steps on their own without involving Support.



**NOTE: the user may need to adjust their Assistance Level to accomplish this:**

Within the F11 screen (Work with All Printers) User will Press F21 ( Shift + F9 )

Change or verify that the assistance level is 2 (Intermediate) then press enter and continue.

 

4. Use option 4 next to the printer in question, then F4

    NOTE: do not press enter between the 4 and F4

 

5. Change *CNTRLD to *IMMED and hit press Enter

    a. It should return the user to the Work with all Printers, with confirmation of the printer ending


6. Hit F5 to refresh the screen, it should now say END for Sts, if not refresh again.


7. When in END status, Use Option 1 to restart the writer and press Enter twice

    a. After Entering you should see the confirmation stating it was submitted

 

8. F5 to Refresh and Sts should show *STR (Started)

 

9. Verify that the printer is printing.


10. If not, use option 8 next to the printer to work with output queue

 

11. Check if there is anything waiting to print

 

12. Press F5 to refresh the screen


13. If you see the status of pending, continue to press F5 several times.

 

If the job Prints, Issue resolved



If the job does not go thru and stays at PND (Pending) or goes to MSGW (Message Waiting) again proceed to the next step

 

NOTE: This is as far as the user can go with F11, the next Steps are done from the Support side.

  

14. Obtain the IP address for the Printer in question.


a. You can use one of two methods to get the IP address

    i. Use http://rm.ur.com/printers.html and locate the IP by printer name

    ii. On the command line type the following command:

    A. WRKDEVD (then a space) then the printer name, and press Enter

    B. Chose Opt 2 to Change, press Enter and page down twice

    C. You should now see the IP listed under Remote Location

    D. Press F3 until you are at a screen with a command line at the bottom

    E. On Command line type Call QCMD, Hit <Enter>

    F. Type in PING ‘IP Address’ (make sure to include the beginning, and ending apostrophes), 
    and press Enter
                
    Note: If there are no replies, or several unsuccessful attempts, it is not a good ping.  
    The printer may not be connected to the network, has a bad cable – Or – the IP address 
    is different on the printer.

    G. Verify that the IP Address is correct on the printer (see IP verification K-Base).
                
    Note: If the IP is correct on the printer and in Rentalman, yet it is still not pinging, 
    you will need to perform Network Connectivity Troubleshooting (see additional K-Bases)