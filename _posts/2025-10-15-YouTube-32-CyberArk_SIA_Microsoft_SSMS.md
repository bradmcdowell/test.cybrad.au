---
title: "#32 - CyberArk SIA - Microsoft SQL SMS"
date: 2025-10-15 09:10:10 +1100
categories: [CyberArk SIA]
tags: [cyberark,privilegecloud,Identity,SIA,SSMS]     # TAG names should always be lowercase
---
This video demonstrates how to implement CyberArk Secure Infrastructure Access (SIA) to enforce Zero Standing Privilege (ZSP) for Microsoft SQL Server. Learn how to securely manage database access using vaulted credentials and just-in-time, least-privilege access policies.

[![Video Preview](https://i.ytimg.com/vi/ybIieKUkD2c/maxresdefault.jpg)](https://www.youtube.com/watch?v=ybIieKUkD2c)

## Objectives

- TLS Certificates – Discuss the importance of TLS certificates in securing communications between SIA and the target SQL Server.
- Connect to Microsoft SSMS via SIA Using Vaulted Credentials – Connect to Microsoft SQL Server Management Studio (SSMS) through SIA using vaulted credentials.
- Create AD Account/Group for ZSP (Zero Standing Privilege) – Create an Active Directory Strong Account and ZSP group that represent your Zero Standing Privilege access model.
- Create Platform / Safe for ZSP Strong Account – Set up a dedicated platform and safe in the CyberArk Vault to store and manage the Strong Account credentials.
- Configure Strong Account in SIA – Register the Strong Account in SIA.
- Onboard Database in Resource Management – Add the SQL Server instance as a managed resource within SIA for policy-based access control.
- Create SIA Policy for ZSP Access – Define an access policy granting just-in-time, least-privilege access to the SQL resource via SIA.
- Test SIA Policy – Connect to the Microsoft SQL database as an end user to validate policy functionality.
- Review Session Diagnostics – Use SIA’s session diagnostics to confirm activity and verify access auditing.

## Timeline

- Intro 0:00
- TLS Certificates 1:23
- Connect to Microsoft SSMS via SIA Using Vaulted Credentials 3:20
- Create AD Account/Group for ZSP (Zero Standing Privilege) 5:28
- Create Platform / Safe for ZSP Strong Account 8:00
- Configure Strong Account in SIA 10:38
- Onboard Database in Resource Management 12:40
- Create SIA Policy for ZSP Access 14:05
- Test SIA Policy 15:32
- Review Session Diagnostics 18:00

Brad McDowell LinkedIn: https://au.linkedin.com/in/bradmcdowell

#CyberArk #ISPSS #Identity #MicrosoftSSMS #SQL #SIA #privilegeaccessmanagement