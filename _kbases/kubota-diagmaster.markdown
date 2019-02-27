---
layout: kbase
title:  "Kubota - Diagmaster"
kbid: "12099"
categories: cgs
---

## Installing Kubota Diagmaster Bundle 431/432/400/236 from Software Center

 

 

 

NOTE1 – Takeuchi Updated the Password and Registration code for Diagmaster. Instructions on how to update this info in Diagmaster are included in “DiagMaster Registration 2019.doc” Word Document attached to this article.

 

NOTE2 – Installing software from the Software Center only applies to URI laptops properly connected to the UR network.

 

- For a successful installation minimize or close all running programs/applications, and do not interrupt the process. Once the SW has been requested, Software Center will also need to be minimized (SW Installation prompts could be hiding behind it)
    a. In case the process is interrupted and the installation failed re-run the install from Software Center under “Available Software” tab or “Installation Status tab” (it may take a few minutes for the Kubota Diagmaster Bundle to refresh and repopulate under Available Software)

 

- Kubota Diagmaster can be installed on all Service Techs’ Laptops

 

- No License needed

 

- The following cable/adapter Kit will need to be purchased from Rentalman in order to use the Diagnostic Software.
    **Software installation will fail or throw an error if the Interface is not connected to the computer.**
 

    Don’t order on ePRo. Write a RentalMan PO and fax it in to Takeuchi.

 

The following is the 2019 Diagmaster User ID, Default Password, and Registration Code. All registration information is case sensitive and must be entered exactly as it reads below.

 

- Login User ID: TakeuchiUSA001
- Password: Zmupuaq0
- Registration Code: QFUP7ZMSf9CvxfltWRearFal70hxHHkw

 

NOTE3 – Any version of Takeuchi Diagmaster Kubota Bundle already installed will need to be removed from Control Panel in order for this Application to be installed successfully:

 

**Uninstall the following Software via Programs and Features:**

 

 

1. Launch Software Center (Check Kbase #12030 - Installing Software from Software Center)

 

2. When the program opens it will default to the Available Software tab

 

3. Here there will be a list of any software that is not currently installed that is available from SCCM

    a. NOTE – If a piece of software was installed but wasn’t installed by SCCM it will still show as an available option in Software Center

 

4. Click the check box next to “Takeuchi Diagmaster Kubota Bundle 431/432/400/236”

 

5. Click the Install Selected button to start the installs

 

6. Four Software packages will be installed with this bundle. This is a verbose installation and users will need to click on prompts in order to proceed. Minimize all other applications/windows first. 

 

7. Installation Status tab will show download percentage and “Installing” message once the downlod is complete

 

8. The following window will display, and users will need to click on “Next”

 

9. Users will need to do the same for all other windows displayed. Leave all settings by default and click on next each time.

 

10. The following window will display. Users will have to connect the DST-I interface to the computer and click on “Next”. Software will then install.

 

11. Click “Next” on this next window. (The warning will display only if the Interface firmware/software is already up to date)

 

12. The following window will display. Click on “Next”

 

13. Click  “Finish” on the following window

 

 

- **If the user gets the following error on Step 10:**

i. Close the DST-i program and have the user disconnect the DST-i Interface

ii. Reconnect the DST-i adapter interface and make sure it’s being detected properly in Device Manager. Should look like this:

iii. Have the user try the DST-i Software Update Wizard again:

    No need to re-run the entire package from Software Center. Navigate to “C:\Windows\ccmcache\” 
    folder and search for “DSTi_Interface”. Launch the Software by double clicking on it and 
    follow the prompts (Step 8)

iv. If Device Drivers are properly installed, but the Software is still crashing, make sure they are using the correct DST-i interface (could be using a Doosan Interface instead and they might need a completely different Software)

v. check the model of laptop this Software is being installed on:

- There seems to be a compatibility issue with older Dell Latitude E64xx series laptops and Kubota Software. If they’re using these old models (E6430/E6420) they may need to send the old laptop back to AMD and get them replaced with a newer model (E7440 or newer)

 

 

 

**Checking Installation Status and Reinstalling Software**

 

1. Once Software Center is open click the Installed Software tab

 

2. All software that has been installed either from the Software Center or from SCCM when it is set to list in the Software Center will be listed here

 

3. For “Kubota Diagmaster Bundle”, Installed Software tab will show the following:

 

4. Although this is an “Available” Application, it cannot be uninstalled directly from Software Center.

 

5. To Reinstall it:

    a. Manually uninstall the following Software from Programs and Features
 
    b. Launch Configuration Manager and run an “Application Deployment Evaluation Cycle”
 
    c. Launch Software Center (If already open, close and re-launch it) and you’ll be able to find the software under “Available Software”

    d. “Kubota Diagmaster Bundle” can now be re-installed from Software Center

 

 

For more details on installation status of a given program from SCCM or Software Center see kbase SCCM_Check Advertisement Status for a Specific Computer