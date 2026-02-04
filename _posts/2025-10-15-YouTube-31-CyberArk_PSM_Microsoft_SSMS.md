---
title: "#31 - CyberArk PSM - Microsoft SQL SMS"
date: 2025-10-15 08:10:10 +1100
categories: [CyberArk Privilege Cloud,PSM]
tags: [cyberark,privilegecloud,Identity,PSM,SSMS]     # TAG names should always be lowercase
---
In this video, we’ll walk through the process of configuring Microsoft SQL Server Management Studio (SSMS) to work securely through CyberArk Privileged Session Manager (PSM).
You’ll learn how to install SSMS, add it as a PSM application, configure your platform and connection components, onboard your domain account, and verify a successful connection through the PSM server.

[![Video Preview](https://i.ytimg.com/vi/W4tKdJnAyog/maxresdefault.jpg)](https://www.youtube.com/watch?v=W4tKdJnAyog)

## Microsoft SSMS Download

You can download Microsoft SMSS v19 from [here.](https://learn.microsoft.com/en-us/ssms/release-history)

## CyberArk KB

[How to use Add-PSMApps to create new connection components](https://community.cyberark.com/s/article/How-to-use-Add-PSMApps)

## Objectives

- Install SQL Server Management Studio (SSMS) - Download from Microsoft and install on each PSM server.
- Run Add-PSMApps.ps1 Script – Adds SSMS to the list of allowed PSM applications on each PSM server.
- Configure Platform & Connection Component - Ensure the SQL exe path is set and linked to the correct platform.
- Onboard Domain Account – Add a domain account that has access to the SQL server.
- Test Access via PSM Server – Launch Microsoft SSMS through a PSM connection and verify secure access.

## Timeline

- Intro 0:00
- SQL Overview 0:43
- Install Microsoft SSMS 1:43
- Connection Component Setup 2:57
- Platform Setup 4:38
- Create Safe 6:09
- Onboard Account 7:15
- Test SSMS 8:13

Brad McDowell LinkedIn: https://au.linkedin.com/in/bradmcdowell

#CyberArk #ISPSS #Identity #MicrosoftSSMS #SQL #PSM #privilegeaccessmanagement