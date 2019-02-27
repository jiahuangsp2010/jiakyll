---
layout: kbase
title:  "VPN - Cert Reinstall"
kbid: "12420"
categories: cgs
---

## Reinstall VPN Certificate
 
 
If needed the personal VPNuser certificate can be removed and reinstalled for an end user on a company provided laptop that is getting a certificate related error message such as “Certificate Validation Failure”
 
1. Click on Start then Control Panel
 
2. If in Categories view click Network and Internet
 
3. Click Internet Options
 
4. Click the Content tab then the Certificates button
 
The certificate is listed in three of the Certificate tabs.  Personal, Intermediate Certificate Authorities, and Trusted Publishers.
 
We can remove and reinstall the certificate under the Personal tab but the other two are locked in place and cannot be removed.
 
5. Click on the Personal tab
 
6. If a ”vpnuser” certificate is already listed click that listing then click Remove
 
7. Close the Certificates window
 
8. Reinstall the **VPN Security Certificate 1.2 – VPNuser Personal Certificate Deploy** from Software Center.  See kbase Installing Software from Software Center for more details.
 
For more details on the full suite of software and files needed for VPN connections on company provided laptops see kbase VPN – 2 Factor Authentication