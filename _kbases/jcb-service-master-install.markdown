---
layout: kbase
title:  "JCB Service Master Install"
kbid: "12353"
categories: cgs
---

## JCB Service Master Full Version

NOTE: This software requires approval from the Maintenance Team before it can be installed on users’ laptops.  

 

- The target laptop must be linked to the ticket and the computer name be listed in the Description

 

NOTE1: In order to install the software, you will need to select it and Install it from “Available Software” in Software Center. The package is over 7GB and it could take up to 10 hours to download (depending on network connection). The installation is fully silent.

 
1. From the Support Center ticket, send an email to MaintenanceTechnical@ur.com and Cc the user requesting the software.

    NOTE: If the request is coming directly from the Maintenance Team, proceed to step 3

    a. Use the following email template adding the employee name, Job Title and Location n.:

    **<Employee> who is a <Job Title> at <LOC#> is requesting approval to install the JCB Service Master Software - Full Version. Per the defined procedure, your team will verify that the user has received the proper training and has the proper JCB Service Master user account.**
 
    **Do you approve this install?**

2. Maintenance Team usually replies within the same day, but in case they don’t, send a follow up email

    a. If the request is denied, have the user follow-up directly with the Maintenance Team

3. If approved:

    a. Contact the user and remote to the laptop

    b. Ensure there is enough space on C: Drive. If not, free some space by removing unneeded files (Disk Cleanup utility, Clear Temp files, move user’s files over to Home drive and if possible have the user check and delete files that are no longer needed)

    c. Check power options and make sure the computer never goes to sleep on AC power, and connect the unit to AC power

    d. Increase Configuration Manger cache size:

    - Launch Configuration Manager client from Control Panel
    - Click on “Cache” tab and then on “Configure Settings”
    - Increase the cache size by setting the size to 15120 MB and click “Apply”

4. Launch the SCCM Configuration Manager Console from ITSUPPORT Server

    a. See kbase – Accessing SCCM Manager Console

5. Assets and Compliance should be selected by default, if not click the option at the bottom of the navigation pane.

 

6. Expand Device Collections

 

7. Select the PC Software Deployments Collection

 

8. Open “JCB Service Master Full” collection by double clicking on it

 

9. Verify the target computer is not already listed in the container

    a. If the unit is already added, launch Configuration Manager on user’s laptop and run a “Machine Policy Retrieval & Evaluation Cycle”. Launch Software Center and check “Available Software” Tab, Service Master should be showing in available Software. Check for duplication tickets for this request and see if another agent is also working this same ticket.

 

10. Right-click on the collection that is listed under Devices and select Add Resources

 

11. Enter the computer name in the field for the Name string and click Search.  (leaving the Resource type as System Resources and the search in collection field as <All Collections>)

 
    a. If the computer name is not showing in the search results, this means the computer name cannot be found in SCCM.  This can occur if the computer name is wrong or if the unit was just added to the domain and it hasn’t been imported from AD yet.

 

    b. If the computer was just added to the domain, the AD import will occur on its own.  You will need to check back and attempt to add again.  You will need to update the All Systems collection after 60 minutes and attempt to add again.

 

12. Click on the listing for the client in the search results and click Add

 

13. Click Ok to close out the Add Resource to Collection window.

 

14. Right click on “JCB Service Master Full” container and select Update Membership to refresh the collection membership

 

15. Click the Refresh icon to the right of the address bar and the client you targeted should be listed in the collection (try again after a minute or so if it still isn’t displayed).

 

16. Create a new comment in Support Center for the ticket and note that the unit was targeted for install and any other applicable notes.

 

17. The user’s computer will automatically pick up the advertisement for this software when it checks in with the SCCM system as long as the SCCM client is installed, working properly and the client is pingable on the URI network.

 

    a. If the SCCM Client isn’t installed please refer to the SCCM Client Install kbase.

 

    b. To force the user’s computer to check in right away,  right click on the user’s computer in SCCM and select Client Accounts > Machine Policy Evaluation and Update Cycle.

 

    c. SCCM will popup a status window indicating the results of the forced policy update.

 

    **This could also be executed from the user’s laptop by launching Configuration Manager Client in Control Panel (Actions tab)**
 

18. From the user’s laptop, launch Software Center and “JCB Service Master Full 2.0” should display under “Available Software”