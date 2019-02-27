---
layout: kbase
title:  "Rentalman - Barcode Printer Issue"
kbid: "11292"
categories: cgs
---

1. Verify the printer shows Ready and the IP is correct, and that the IP address can be pinged.  If not See KBase -Rentalman barcode printer IP address verification and reset (KBase 10902)

    a. If the printer is not ready, see Troubleshoot the Barcode Printer Status Lights (KBase 10442)

2. On Command line type WRKOUTQ UR###* (Replace the ### with the printer name followed by an *)

3. Verify that the Barcode printer is listed
 
    a. If a printer is not listed see Create a Barcode Printer in Rentalman (KBase 11122)

4. Check to see if there is a writer listed for the barcode printer
 
    a. If blank Start the writer (KBase 10726) by placing a 2 next to the printer and press Enter 
 
    b. Continue pressing Enter until you are back to the printer listing (3 times)

    c. Press F5 to refresh the screen and you should then see a writer listed

5. If there is a writer for the printer, and the status is valid, End the writer, and then restart the writer.

    a. Next to the printer select 9 (Work with Writers) and press Enter

    b. Next to the writer select 4 and without pressing anything press F4
 
    c. On the End Writer screen change the “When to end writer” field to *IMMED and press Enter
 
    d. The screen will return to the Work with Writers screen and at the bottom should indicate that it is ending.
  
    e. Press F5 to refresh and it should display (No Writers)
 
    f. Press F12 to go back to the Work with All Output Queue screen

    g. If blank Start the writer (KBase 10726) by placing a 2 next to the printer and press Enter 
 
    h. Continue pressing Enter until you are back to the printer listing (3 times)

    i. Press F5 to refresh the screen and you should then see a writer listed

If the Barcode Printer continues not to print, gather the following information and escalate to RentalMan Level 2

A. Location Number

B. User’s RentalMan user ID

C. RentalMan Printer name

D. IP Address in RentalMan

E. IP Address on device

F. Ping Results

G. Steps taken to trouble shoot the issue