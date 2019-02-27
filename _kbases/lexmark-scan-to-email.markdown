---
layout: kbase
title:  "Lexmark - Scan To Email"
kbid: "10882"
categories: cgs
---

## Lexmark Printers Scan to email

 

**Note: Follow directions from attached  Word document for Printer Relay settings**



 

If users are not receiving the email after they scanned a document from Lexmark printers, do the following:

 

1. Make sure the printer DNS Settings are as follows, and check if the printer is already on the relay:


    a. Go to SETTINGS > NETWORK/PORTS > TCP/IP



    - DNS Server Address: 10.6.128.37
    - Backup DNS Server Address: 10.6.128.40



2. If the printer is not showing any errors after scanning to email, make sure that “Reply Address” in printer settings has a valid email address format (i.e. URXXP1@ur.com):


    Primary SMTP Gateway is required: [relay.ur.com](relay.ur.com) (check attached document for more info and screenshots)

 

Have the user try again.

If they’re still having problems, gather all required info and escalate the ticket to PC Level2.