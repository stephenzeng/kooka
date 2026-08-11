# Microsoft Teams
**Date created:** 2026-08-06 UTC  
**Tags:** Administration, Analytics, Security  

## New Articles

- **Manage the Meeting Recaps app for your organization in Microsoft Teams**

  Introduced a new admin guide for configuring and governing the Meeting Recaps app. Explains recap types (intelligent text, video, and audio) and availability constraints, including the 30‑day window and requirement for recorded/transcribed meetings. Details licensing: Microsoft 365 Copilot for AI-generated audio/video recaps and Teams Premium or Microsoft 365 Copilot for intelligent text recaps, with transcripts available without Copilot. Provides step-by-step instructions to deploy and pin the app via Teams admin center app setup policies.

  https://learn.microsoft.com/en-us/microsoftteams/manage-meeting-recaps-app

## Major Changes

- **IT Admins - Private channels in Microsoft Teams**

  Expanded private channel capabilities to support channel meetings and aligned limits with the overall team channel cap (up to 1,000, with noted cloud exceptions). Removed outdated statements about a 30 private channel limit and scheduling restrictions, and updated SharePoint storage behavior to reflect new compliance defaults. These changes enable broader collaboration scenarios and simplify capacity planning for large teams.

  https://learn.microsoft.com/en-us/microsoftteams/private-channels

- **Microsoft Teams Rooms Maintenance and Operations**

  Added platform-specific guidance for log collection, separating instructions for Teams Rooms on Windows (PowerShell-based) and Android (OEM tools/portals). Introduced a dedicated section on audio processing and noise suppression, clarifying Windows defaults, DSP/AEC behavior, and the OEM-driven model on Android. Streamlined the article by removing legacy Group Policy, registry-based log cleanup, and remote PowerShell management content, and by renaming sections to clearly differentiate Windows vs. Android guidance. This improves clarity, reduces obsolete guidance, and helps admins follow the right operational procedures per platform.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/rooms-operations

## Moderate Changes

- **Reporting - Teams Phone Agent, Auto Attendant, and Call Queue historical reports**

  Added a notice that GCCH and DoD tenants can access only 28 days of historical data until September 30, 2026. This sets expectations for data retention and helps government cloud customers plan reporting needs accordingly.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-report-historical

- **Setup - Shared Call History for Call Queue**

  Expanded setup guidance with audience context, planning/licensing details, and prerequisites, including the requirement to enable Conference mode. Consolidated requirements and notes into structured sections and indicated that the Queues app is required, making deployment steps clearer and easier to follow.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-setup-call-queue-shared-history

- **Manage updates for Teams android devices in Pro Management portal (PMP)**

  Clarified minimum Admin Agent versions for commercial and government clouds, and explained that PMP controls automatic updates while TAC auto-updates are stopped. Emphasized non-pausable enforcement to reach minimum agent versions, pausing other updates until compliant, and outlined post-deprecation steps that may require OEM tools. This helps admins ensure devices remain supported and secure with predictable update behavior.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/androidupdatemanagementinpmp

- **What's new in Microsoft Teams devices**

  Added an August 5, 2026 release note for Teams phones (app version 1449/1.0.94.2026220406) with navigation performance improvements and faster dial pad interactions. Included multiple reliability fixes covering dial pad behavior, UI overlap, accessibility with large text, and password expiry flow, improving daily usability.

  https://learn.microsoft.com/en-us/microsoftteams/devices/devices-release-notes

- **Microsoft Teams Rooms on Windows and Teams Android device security**

  Updated Pro Management Portal network requirements by adding agent.rooms.microsoft.com for Teams Android devices. Clarified Azure IoT Hub port references and consolidated government cloud endpoint notes to simplify firewall configuration and compliance reviews.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/security

- **New VDI solution for Teams**

  Updated network requirements to include graph.microsoft.com alongside *.office.net for TCP 443/80 access. Added guidance for custom background effects, covering support for blur/change, image upload storage in OneDrive, client media engine requirements, and scenarios not supported (scripted file placement and guest join backgrounds), helping IT plan policies and user enablement.

  https://learn.microsoft.com/en-us/microsoftteams/vdi-2