---
title: "Control access based on network location or app"
ms.author: kaarins
author: kaarins
manager: pamgreen
ms.date: 06/21/2018
ms.audience: Admin
ms.topic: article
ms.service: one-drive
localization_priority: Normal
ms.collection: Strat_OD_admin
search.appverid:
- ODB160
- ODB150
- MET150
ms.assetid: 59b83701-cefd-4bf8-b4d1-d4659b60da08
description: "Learn how to apply conditional access settings in the OneDrive admin center."
---

# Control access based on network location or app

To prevent users from accessing OneDrive and SharePoint content on devices outside of specific domains, and to prevent them from accessing files in apps that don't check for device status, use the Device access page of the [OneDrive admin center](https://admin.onedrive.com/?v=AccessPolicySettings).
  
![The Device access tab of the OneDrive admin center](media/4b5811ac-01e5-4fca-99f2-e9db8bb6237e.png)
  
## Control access based on network location

You can choose a specific IP addresses or IP address ranges from which you want to allow users to access their OneDrive files. For example, you might want your users to only access OneDrive files using network addresses that your organization owns.
  
 **To allow access only from defined network locations**
  
1. Under **Control access based on network location**, select the **Allow access only from specific IP address locations** check box. 
    
2. Click **Edit**.
    
3. Enter the **public IP address ranges** that you want to allow using CIDR notation. Enter one IP address range per line, and make sure there are no overlapping IP addresses.
    
4. Click **Save** on the Device access page. 

**Note:**
The following IP addresses ranges are considered as private and the system will not block them:

- **10.0.0.0/8 IP addresses**: 10.0.0.0 -- 10.255.255.255

- **172.16.0.0/12 IP addresses:** 172.16.0.0 -- 172.31.255.255

- **192.168.0.0/16 IP addresses:** 192.168.0.0 – 192.168.255.255


    
## Control access from apps that don't use modern authentication

Some third-party apps and versions of Office prior to Office 2013 don't use modern authentication and can't enforce device-based restrictions. This means they allow users to bypass conditional access policies that you configure in Azure.
  
 **To block access from apps that don't use modern authentication**
  
1. Under **Control access from apps that can't enforce device-based restrictions**, clear the **Allow access from apps that don't use modern authentication** check box. 
    
2. Click **Save**.
    
## See also

[Manage OneDrive for Business mobile access](control-access-to-mobile-app-features.md)
  


