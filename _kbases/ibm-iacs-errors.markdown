---
layout: kbase
title:  "IBM iACS - Errors"
kbid: "11851"
categories: cgs
---

## IBM iACS – Errors When Launching Application

NOTE – IBM i Access Client Solutions is Java based, most error messages when attempting to launch the application are related to Java in some way.  When troubleshooting always start by making sure that the only version of Java that is installed is the latest approved version by UR.

This will cover various error messages, what they mean and how to resolve the issue.


1. Error – “The program can’t start because verify.dll is missing from your computer.  Try reinstalling the program to fix this problem.”
    a. Cause – Java is not installed or on a very old version.
    b. Resolution – Uninstall any existing version of Java and install the latest version from Software Center

2. Error - “**MSGGEN001** – The function did not complete successfully.”
    a. Cause – Usually related to the IBM signon credentials for the end user being disabled, despite being SSO this seems to be the cause.
    b. In RM go to 8 -> 1 from the main menu and check their RM account, enable if it shows disabled.  If the account shows enabled, but the client still will not start without this error message, follow the steps in KB13119 - EIM Table User Lookup Support Tool. Only send an email to as400@ur.com if you performed the self-service steps listed in KB13119 - EIM Table User Lookup Support Tool and did not find the user. Ask to have the user added to the EIM (SSO) table for RM. The response from the as400 team should be within 15 minutes for this check. If the account already exists on the EIM table escalate the issue to PC level 2 for further troubleshooting

3. Error – “**MSGSSL009** – An SSL certificate was encountered with a disallowed key length of 4096.  The maximum length allowed by your Java Runtime Environment is 2048.  To correct this, you may need to update the policy files of your Java Runtime Environment.”
    a. Cause – Either an old version of Java is installed or a 64 bit version is installed
    b. Resolution – Uninstall any existing versions of Java then update to the latest Java release from Software Center

4. Error – “**MSGKRB001** – Kerberos error for system %1$s.”
    a. Cause – Laptop user recently changed password or the network password is expired
    b. Resolution – Fully synchronize the network password with the laptop and ensure both Windows and PGP are using their new password.  If the network password is expired first have the end user update their password.

5. Error – “**MSGFI002** – The file could not be found”
    a. Cause – The following file has been corrupted – C:\users\username\IBM\i Access Client Solutions\config-Directory\username\IBM\iAccessClient\Primvate\username\cacerts
    b. Resolution – Navigate to the above directory and replace the cacerts file with the copy from \\fs3\Software\ITSupport\IBM i Access Client Solutions\ then re-launch Rentalman