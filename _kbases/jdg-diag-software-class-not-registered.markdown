---
layout: kbase
title:  "JDG Diag - Software Class Not Registered Error"
kbid: "12944"
categories: cgs
---

## Class not registered – JLG Diagnostic Software

 

 

 

Users may receive the following error message while trying to run diagnostics on JLG equipment using PGFLASHW Programming Software:

 

The dll file may be missing or not registered:

 

1. If missing, copy “**MSSTDFMT.DLL**” from FS3 (path below) to user’s laptop **c:\Windows\System32\** folder:

 

    [\\fs3\Software\ITSupport\Equipment_Diagnostics\JLG\PGFLASH_DLL_Files](\\fs3\Software\ITSupport\Equipment_Diagnostics\JLG\PGFLASH_DLL_Files)

 

2. Open an elevated command prompt (you should already be on c:\WINDOWS\system32\ directory)

 

3. Type “**regsvr32.exe MSSTDFMT.dll**” and click “Ok” on “succeeded” message

 

4. User should now be able to launch **PGFLASHW** Software

