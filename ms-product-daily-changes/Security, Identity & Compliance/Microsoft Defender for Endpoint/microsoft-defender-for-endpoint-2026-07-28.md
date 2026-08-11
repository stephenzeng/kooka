# Microsoft Defender for Endpoint
**Date created:** 2026-07-28 UTC  
**Tags:** Administration, Security  

## New Articles

- **Android Mobile Threat Defense (MTD) Role for Microsoft Defender for Endpoint**

  Introduced a new article explaining the Android MTD Role and how it strengthens Defender’s resilience on managed devices by preventing force-stop and data clearing, and exempting the app from battery optimizations on Android 14+ for improved reliability. It outlines prerequisites (Intune-managed devices, MTD connector, Android Management API enrollments, and required app assignment) and supported enrollments (COBO, COPE; BYOD not supported). The article details deployment via the Intune MTD connector, including an optional auto-launch toggle during setup, and provides guidance for assigning the role to existing deployments. It also lists platform limitations and steps to verify protections are active on devices.

  https://learn.microsoft.com/en-us/defender-endpoint/android-mobile-threat-defense-role

## Major Changes

- **Configure Defender for Endpoint on Android features**

  Added support for scanning non-APK files on Android, extending malware protection beyond apps to documents, archives, and scripts. Updated guidance clarifies privacy boundaries across work and personal profiles and covers supported management scenarios (BYOD, COPE, COBO). The article now includes prerequisites to add and sync Microsoft Defender Antivirus from managed Google Play and step-by-step instructions to enable the feature via Intune app configuration, including verification on devices and how detections surface in the Defender portal.

  https://learn.microsoft.com/en-us/defender-endpoint/android-configure

## Moderate Changes

- **Configure Microsoft Defender for Endpoint on Android risk signals using App Protection Policies (MAM)**

  Updated guidance to enable non-APK file scanning via an Intune Managed apps app configuration policy by targeting the Defender Android app and setting EnableNonAPKFileScan=1 and DefenderMAMConfigs=1. The edits also clarify that Defender respects Android profile boundaries, along with minor formatting and path notation updates.

  https://learn.microsoft.com/en-us/defender-endpoint/android-configure-mam

- **Microsoft Defender for Endpoint - Mobile Threat Defense**

  Clarified the difference between the Defender for Endpoint Mobile Threat Defense solution and the separate Android MTD Role, with links to deeper guidance. Expanded the Android Malware Protection capability to include non-APK file scanning and pointed to configuration instructions, plus added a resource link to the Android MTD Role article.

  https://learn.microsoft.com/en-us/defender-endpoint/mtd