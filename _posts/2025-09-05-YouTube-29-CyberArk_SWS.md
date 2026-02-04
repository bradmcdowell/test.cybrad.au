---
title: "#29 - CyberArk Secure Web Sessions (SWS)"
date: 2025-09-05 08:10:10 +1100
categories: [CyberArk Identity]
tags: [cyberark,privilegecloud,Identity,WPM,SWS]     # TAG names should always be lowercase
---
In this video, I walk you through the key features and setup process of CyberArk Secure Web Sessions (SWS) — a powerful solution designed to secure, monitor, and protect sensitive web sessions. You’ll see how SWS helps organisations maintain visibility and control over privileged web activities, reduce security risks, and strengthen compliance.

[![Video Preview](https://i.ytimg.com/vi/OMGOcOmWWog/maxresdefault.jpg)](https://www.youtube.com/watch?v=OMGOcOmWWog)

## Gitea Web App

This is the logon sequence script for Gitea. This needs to be pasted into the Advanced tab. This script appends the domain name to the username.

``` javascript
loginData.applicationUrl = "https://gitea.domainname.example/user/login";
loginData.addField("username", "input#user_name", LoginUsername+"@domainname.example");
loginData.addField("password", "input#password", LoginPassword);
loginData.submitPattern = "button.ui.primary.button";
```

## Objectives

- Review PSM Web App use case
- Add and configure the Web App using user credentials
- Switch Web App to shared credential model
- Set up Secure Web Sessions tenant
- Enable Secure Web Sessions on the Web App
- Review Secure Web Sessions audit and recording

## Timeline

- Review PSM Web App use case 0:40
- Add and configure Web App using user credentials 1:40
- Switch Web App to shared credential model 6:25
- Set up Secure Web Sessions tenant 10:38
- Enable Secure Web Sessions on the Web App 14:00
- Review Secure Web Sessions audit and recording 16:40

Brad McDowell LinkedIn: https://au.linkedin.com/in/bradmcdowell

#CyberArk #ISPSS #WPM #SWS #SecureWebSessions #Identity #identity #privilegeaccessmanagement