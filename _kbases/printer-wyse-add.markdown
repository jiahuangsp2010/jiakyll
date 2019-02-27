---
layout: kbase
title:  "Printer - WYSE Add"
kbid: "10170"
categories: cgs
---

# 10170
***

## Add Printer to Print Server for WYSE Windows Sessions

Required information for this type of request:

- Printer Make
- Printer Model
- IP address
- Location Number (e.g. 586)
- City and State where location is based
- Printer Name (e.g. UR586P2)
- Printer Asset Linked to the Ticket

1. Confirm the unit is not already created on \\PS2, \\PS1, \\ PS3 (for Legacy NES Locations only), \\CTXUPS1 or \\CTXUPS2 (for Legacy NES Locations only)

2. If the printer isn’t created on either server, collect the required information and record in the Description field.

3. Verify that the printer is setup with the proper static IP range.
    a. e.g.URxxxP1 = 10.x.x.51, URxxxP2 = 10.x.x.52 etc.

4. Verify that the device can be reached on the network.

5. Assign the ticket to PC Level 2 stating that the printer needs to be added to the print server.

6. The PC Level 2 team will create the printer and update the ticket and the user when the request has been completed.

7. If assistance in adding the printer to the users Windows session is needed, please refer to the device and environment specific kbase document.

## Legacy NES Location Printer Procedures Only

With the acquisition of NES there has been some changes to the Print Servers specific to legacy NES sites only. Please refer to the notes below

**Citrix Based Printing**

- NES printers have been added to a new server called CTXUPS2. Only legacy NES location printers will be on this server. (Refer to the attached list of NES Locations)
- Any user in a Citrix session should have the location printer’s auto created at log on from CTXUPS2. The user will need to select the default printer the first time.
- If a NES location printer needs to be added to CTXUPS2, the printer will need to be added by PC L2 with the information required and outlined in this kbase. (see above)

**WYSE Base Session Printing**

- NES printers are going to be added to PS3 Server. Only legacy NES location printers will be on this server and PS3 should only be used for WYSE base session printing.
- If a NES location printer needs to be added to PS3, the printer will need to be added by PC L2 with the information required in this kbase (see above)

**Laptop Based Printing**

- Users who need to print to a legacy NES printer from a laptop need to have the printer added will need to add a local printer to the unit and print by IP port. Please refer to kbase #10183 for the process. The proper driver will need to be used during the install process and will vary till their printers are refreshed with Lexmark units.
- Laptop users should NOT use any PS or CTXUPS server to print. This applies to All UR and Legacy NES users