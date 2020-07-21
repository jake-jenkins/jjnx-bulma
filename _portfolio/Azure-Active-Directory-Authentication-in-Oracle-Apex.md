---
title: Azure Active Directory Authentication to Oracle Apex
date: 2020-03-01 00:00:00 Z
categories:
- Apex
tags:
- active directory
- ad
- apex
- authentication
- authorisation
- azure
- business app
- cloud
- domain
- enterprise
- enterprise application
- login
- oracle
- security
- single sign on
- sso
language: Active Directory
icon: azure
color: grey
layout: portfolio
---

I have recently integrated an Oracle Apex app to utilise Microsoft Azure Active Directory to authenticate users. The authentication sends the username from Azure and permissions are granted in an authorisation table in the Apex app.

Users email addresses are matched to a people table with a specified role. A seperate authorisation scheme sets the session to the matching role.

This was performed for a live project management application I have been developing for a client.
