---
layout: kbase
title:  "Zebra - Status Lights"
kbid: "10442"
categories: cgs
---

### BarcodePrinter_Status Light Troubleshooting 

Status Light Troubleshooting for Zebra Printer Models
```
R402, DA/DT402, LP/TLP2824-Z, LP/TLP 2844-Z, TLP 3844-Z
```

What the status light is telling you

| [led color] | [status] | [refer to #] |
| ----------- | ------ | ---------- |
| off   | off | 1 |
| Solid Green |	On | 2 |
| Flashing Yellow |	Stopped | 3 |
| Flashing Green | Normal Operation | 4 |
| Flashing Red | Stopped | 5 |
| Double Flashing Green | Paused | 6 |
| Solid Yellow | Various | 7 |
| Alt Flashing Green + Red | Needs Svc | 8 |

**Resolutions**

```
01. The printer is not receiving power.
    a.  Have you turned on the printer power?
    b.  Check power connections from the wall outlet to the power supply, and from the power 
        supply to the printer.

02. The printer is on and in an idle state.
    a.  No action necessary

03. The printer has failed its power on self test (POST)
    a.  If this error occurs right after you turn on the printer, unit needs to be replaced, 
        escalate to PC Level 2.
    b.  If this error occurs after you have been printing, there is a shortage of memory. Turn 
        the printer power off and on, then, resume printing.

04. The printer is receiving data.
    a.  As soon as all of the data has been received, the status LED will turn green; then, 
        the printer will automatically resume operation.

05. Either the media is out or the print head is "open".
    a.  Load a roll of media, then press the feed button to resume printing.
    b.  Close the top cover. Then, press the feed button to resume printing.

06. The printer is paused.
    a.  Press the feed button to resume printing.

07. The print head is under temperature or over temperature.
    a.  If the print head is under temperature, continue printing while the print head reaches 
        the correct operating temperature
    b.  If the print head is over temperature. Printing will stop until the print head cools to 
        an acceptable printing temperature. When it does, the printer will automatically resume 
        operation.    

08. FLASH memory is not programmed.
    a.  Unit needs to be replaced. Advise branch this is a NON serviceable failure, to order a 
        new Barcode printer via ePortal, and return the defective printer to the Asset 
        Management Depot (Kb 11195). Update ticket details to advise a new printer is being 
        ordered and Resolve the ticket.
```