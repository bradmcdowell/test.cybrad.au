---
title: "#26 - CyberArk SIA Windows Strong Account"
date: 2025-07-22 08:10:10 +1100
categories: [CyberArk SIA]
tags: [cyberark,privilegecloud,Identity,SIA,ZSP,CPM]     # TAG names should always be lowercase
---
Welcome back to the CyberArk SIA series! In this video, we take a deep dive into the SIA Windows Strong Account, focusing on how to enforce least privilege wherever possible through secure configuration and testing.

[![Video Preview](https://i.ytimg.com/vi/EsSILQWNVQI/maxresdefault.jpg)](https://www.youtube.com/watch?v=EsSILQWNVQI)

## CyberArk Docs
[What is a Windows strong account?](https://docs.cyberark.com/ispss-access/latest/en/content/introduction/dpa_strong-account.htm)

## Strong Account
The script bellow allows the Strong Account to be able to edit the members of the AdminSDHolder template.

```powershell
# Set the AD account that will be used for the Strong Account
$StrongAccount = "DOMAIN\<CyberArk_Strong_Account>"

# This gets the AD domain in DN format
$DistinguishedName = (Get-ADDomain).DistinguishedName
Write-host "Domain OU is =" $DistinguishedName

# This gets the AdminSDHolder DN
$AdminSDHolerDN = "CN=AdminSDHolder,CN=System,"+$DistinguishedName
Write-host "AdminSDHolder DN is =" $AdminSDHolerDN

# Grant permissions to allow modifying group membership
dsacls.exe $AdminSDHolerDN /G $StrongAccount":WP;member"
```

## Objectives

- Platform and Safe settings – SIA Strong Account
- Remove SIA Strong Account from Domain Admins
- Delegate permissions for SIA Strong Account
- Group Policy restrictions for SIA Strong Account
- Test (Server Admin and Domain Admin) ZSP use cases
- Allow SIA Strong Account to create Domain Admins
- Test – Domain Admin ZSP use case
- Test – Local Admin ZSP use case
- Multiple SIA Strong Accounts – Least Privilege

## Timeline

- Intro 0:00
- Platform and Safe settings 1:30
- Remove from DA 5:47
- Set Permissions 6:28
- Group Policy Settings 8:40
- Test Server Admin ZSP Account 9:35
- Test Domain Admin ZSP - Failure 11:40
- Allow Strong Account to mange Domain Admins 12:45
- Test Domain Admin ZSP - Success 17:24
- Test Local ZSP Account 18:40
- Multiple SIA Strong Accounts 19:56

LinkedIn: https://au.linkedin.com/in/bradmcdowell