# Microsoft Teams
**Date created:** 2026-08-19 UTC  
**Tags:** Compliance, Configuration, Deprecation, Get Started, Guidance, Licensing, Security, Troubleshooting  

## Major Changes

- **Setup - Compliance Recording for Call Queues template**

  Restructured the article from an overview to a comprehensive planning and licensing guide, with clear prerequisites and links to related planning content. Added step-by-step instructions to create and assign Compliance Recording templates in the Teams admin center, including strict recording options, paired bot configuration, and concurrent invitation limits. Clarified unsupported calling scenarios and renamed greeting sections to align with the UI, consolidating audio guidance. Centralized “What’s New” and “Known issues (None)” content and removed the prior PowerShell-centric approach to reduce confusion.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-setup-call-queue-template-recording-compliance

- **Setup - Shared Call History template for Call Queue**

  Removed the entire PowerShell examples section that previously walked through creating and assigning Shared Call Queue History templates. This streamlines the article and reduces duplication, but admins who relied on those scripts will need to use alternative references or UI-based guidance. The change emphasizes consolidated, maintainable configuration guidance.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-setup-call-queue-template-shared-history

- **Remote provisioning and sign in for Teams Android devices**

  Reworked the procedure to use the Teams Rooms Pro Management Portal instead of the Teams admin center. Added a guided flow: add device identifiers (including bulk upload), generate verification codes for one or many devices, enter the code on the device, and complete first-time remote sign-in via microsoft.com/devicelogin. Introduced guidance for devices that were previously signed in and a remote sign-out option from the Rooms > Account tab. Removed older admin center instructions and legacy links to focus on the new, portal-based process.

  https://learn.microsoft.com/en-us/microsoftteams/devices/remote-provision-remote-login

## Moderate Changes

- **Setup - Auto Attendant**

  Replaced the in-page “What’s new” with a centralized include and added a “Known issues” section indicating none. This improves consistency across articles and makes it easier to track updates in one place.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-setup-auto-attendant

- **Setup - Create an Auto attendant via PowerShell**

  Centralized shared guidance using multiple content includes for common, Auto Attendant–specific, and setup topics, plus a “What’s New” insert. The structure is cleaner and easier to maintain, with no behavioral or procedural changes.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-setup-auto-attendant-cmdlets

- **Setup - Call Queue**

  Replaced the in-page “What’s new” with a centralized include and added a “Known issues” section indicating none. This aligns the page with a consistent updates model and reduces duplicate, dated entries.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-setup-call-queue

- **Transitioning Teams Android Device Management from Teams Admin Center to the Teams Rooms Pro Management Portal**

  Removed the “Admin Agent update readiness” section that outlined accelerated minimum versions and forced updates across clouds. This simplifies deprecation guidance and avoids outdated or conflicting requirements.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/aboutunifieddevicemanagement-pmp1

- **Teams Rooms on Android certified devices**

  Added GCCH firmware release entries for multiple Logitech and Neat devices, including latest firmware and app versions. This helps admins validate baseline versions and plan compliant updates across government cloud environments.

  https://learn.microsoft.com/en-us/microsoftteams/devices/certified-hardware-android

- **Overview of AI in Microsoft Teams for IT admins**

  Updated terminology from “Microsoft 365 Copilot” to “Microsoft Copilot” across headings, app names, and license references. Clarified licensing context, including multitenant scenarios, without changing features or structure.

  https://learn.microsoft.com/en-us/microsoftteams/copilot-ai-agents-overview

- **Teams settings and policies reference**

  Added a new meeting policy: “Allow numeric-only meeting passcodes” (default Off). Enabling it allows 8-digit numeric-only passcodes, which are less complex and may increase risk; it applies only to newly scheduled meetings.

  https://learn.microsoft.com/en-us/microsoftteams/settings-policies-reference

- **Certified Teams displays**

  Introduced a Firmware tab listing TAC-released firmware (including Neat Frame) with app versions and release dates. Added an End of certification tab detailing certification and Microsoft support end dates by model, improving lifecycle and compliance planning.

  https://learn.microsoft.com/en-us/microsoftteams/devices/teams-displays-certified-hardware

- **Certified Teams panels**

  Added new GCCH firmware entries for Logitech TAP Scheduler and Neat Pad, including latest firmware and updated app versions with release dates. This provides clear baselines for validating and maintaining panel deployments in government cloud environments.

  https://learn.microsoft.com/en-us/microsoftteams/devices/teams-panels-certified-hardware