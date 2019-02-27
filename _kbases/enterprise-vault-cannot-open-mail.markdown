---
layout: kbase
title:  "Enterprise Vault - Cannot Open Mail"
kbid: "10277"
categories: cgs
---

## Email Cannot Retrieve Mail Archived by Enterprise Vault

 

The Current Version of the Outlook Vault Software is: Veritas Enterprise Vault Outlook Add-in (x64)

 

 

1. Determine if the Current version of  the Outlook Enterprise Vault SW is installed on the user’s laptop.

2. Go to the Control Panel “Programs and Features” for Windows 7 and check for the existence of the “Symantec Enterprise Vault HTTP-Only Outlook Add-In” ver. 10.X: If this version exists remove it by uninstalling the software.

3. Go to the Start Menu > All Programs > Microsoft System Center > Configuration Manager > Software Center on the users laptop.

4. Attempt to install the Enterprise Vault Outlook Add-In (x64) 12.1.9723 (Veritas Technology)

5. If no client is listed in the software center, install the proper client package manually from \\FS3\Software\ITSupport\Veritas Enterprise Vault\Version12\Outlook Add-In\x64 

6. Close and re-launch Outlook.

7. Have the user open a message that has been archived.