# Microsoft Teams
**Date created:** 2026-07-21 UTC  
**Tags:** Administration, AI, Governance, Other, Security  

## New Articles

- **Set up compliance recording in Microsoft Teams**

  Introduced an end-to-end how-to guide for deploying compliance recording, including creating and syncing a compliance recording application instance and obtaining the provider’s recorder application ID. Added detailed steps and PowerShell examples to create, configure, and assign Teams compliance recording policies, including specifying recording applications. Included verification commands and links to related policy and recording guidance to streamline deployment and ensure regulatory coverage.

  https://learn.microsoft.com/en-us/microsoftteams/teams-compliance-recording-setup

## Major Changes

- **Microsoft Teams compliance recording (third-party)**

  Reorganized the article by removing step-by-step setup procedures and PowerShell examples for creating application instances and managing recording policies. The content now focuses on conceptual guidance, with implementation details moved to dedicated setup documentation. This change reduces duplication and helps admins find definitive deployment steps in one place.

  https://learn.microsoft.com/en-us/microsoftteams/teams-recording-compliance

## Moderate Changes

- **Manage external bots and their access to meetings hosted in your organization**

  Updated applicability to consolidate Webinars and Town halls into a single Events category, alongside Meetings. This clarifies where external bot controls apply across meeting types and event scenarios.

  https://learn.microsoft.com/en-us/microsoftteams/manage-external-bots

- **Overview- Recording and transcription for Teams meetings, events, and calls**

  Clarified which policies govern recording and transcription, where each applies, and where to configure them. Added concise definitions for convenience recording, transcription, explicit recording consent, and intelligent recap, including transcript and licensing dependencies, helping admins set accurate expectations and configurations.

  https://learn.microsoft.com/en-us/microsoftteams/recording-transcription-overview

- **Release notes for Microsoft Teams Rooms**

  Added a new 5.6.137.0 (7/20/2026) entry introducing ad-hoc room reservation for Teams Rooms with a Pro license, managed via the Pro portal, and noted deprecation of Together mode across Teams clients. Removed the earlier SIP/H.323 dialing capability note and made minor editorial fixes. These updates help admins plan feature availability and adjust deployment expectations.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/rooms-release-note

- **Certified Teams phones**

  Adjusted a prior firmware release date for the C456HD and added a new Poly firmware release (9.5.0.1321 AOSP) with updated Teams client, Intune, Authenticator, and Admin Agent versions dated July 20, 2026. This helps device admins schedule rollouts and validate compatibility.

  https://learn.microsoft.com/en-us/microsoftteams/devices/teams-phones-certified-hardware

- **Troubleshooting the new optimization**

  Expanded guidance for error code 110 to cover AVD/Windows 365 by enabling Background app permissions for Windows App and, if needed, setting the GlobalUserDisabled registry value to 0. Updated the error mapping table with a new code for unsupported Citrix Workspace versions and refined several entries (including proxy-related and minimum-version notes), improving diagnosis accuracy and resolution speed.

  https://learn.microsoft.com/en-us/microsoftteams/vdi-2-troubleshooting