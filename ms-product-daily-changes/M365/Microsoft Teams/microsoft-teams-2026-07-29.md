# Microsoft Teams
**Date created:** 2026-07-29 UTC  
**Tags:** Administration, Agent, Monitoring, Other, Security  

## Major Changes

- **Overview of Microsoft Teams panels**

  Streamlined guidance by removing outdated FAQs and narrowing the remote device management description to where licensed panels can be viewed. Also removed best practices for managing firmware and Teams app updates, including rollout ring recommendations and manual update notes. This reduces confusion and aligns the article with the current, simplified device management experience.

  https://learn.microsoft.com/en-us/microsoftteams/devices/overview-teams-panels

- **Microsoft Teams PowerShell Release Notes**

  Updated the July 2026 GA entry to version 7.9.0 with broad cmdlet and policy enhancements across channels, meetings, calling, events, and voicemail. Introduced new controls for synthetic media detection, attendee verification, consent, authentication contexts, transcripts, and engagement reporting, plus additional Teams Channels Policy settings. Notably, removed all Teams Shifts Connection cmdlets (breaking change). Added a July 2026 7.8.1-preview entry and expanded the May 2026 7.8.0 notes with AI knowledge cmdlets and multiple policy parameter updates to help admins manage security, compliance, and meeting experiences more precisely.

  https://learn.microsoft.com/en-us/microsoftteams/teams-powershell-release-notes

## Moderate Changes

- **Manage - Resource accounts for Teams Phone Agent, Auto Attendant, and Call Queue**

  Added two application IDs for Skype for Business Server 2019 scenarios to support creating application instances for AI Agent and Standalone. Minor terminology refinements improve clarity without changing procedures.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-manage-resource-accounts

- **Reference - Answer Teams Phone Agent, Auto Attendant, and Call Queue calls**

  Modularized the article with standardized include sections for common guidance and each workload, aligning structure and terminology. This improves consistency and makes it easier to maintain and reuse core instructions.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-reference-answer-calls

- **Reference - Dial by Name and Dial by Number**

  Reworked the structure and terminology, adding standard includes and clear separation of DTMF vs. speech input for Dial by Name. Clarified that Auto Attendant Dial by Extension doesn’t support Teams-assigned phone numbers (LineURI), added supported number/extension formats with PowerShell examples, and refined search and dial scope guidance. Expanded language support details and recognized voice commands to reduce misconfiguration and improve caller experiences.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-reference-dial-by-name-number

- **Setup - Shared Call History for Auto Attendant**

  Added audience guidance and a planning/licensing review, with standardized terminology for Shared Call History. Expanded, UI-aligned steps for creating and assigning templates, and clarified that call flows sharing the same voicemail destination must use the same template. These updates help admins plan correctly and configure templates consistently.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-setup-auto-attendant-shared-history

- **Setup - Call Queue**

  Substantially expanded setup guidance with Quick vs. Advanced options, standardized terminology, and reusable content includes. Added details on supported languages, Shared Call History templates and licensing, membership models (users/groups, channels, Shifts), presence-based routing, and conference mode. Clarified callback behavior and exception handling, updated authorized users, corrected PowerShell-only options, described automatic/compliance recording, and enhanced diagnostics instructions—enabling more reliable, compliant, and supportable deployments.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-setup-call-queue

- **Setup - Automatic Recording for Call Queue**

  Added a reusable include to align with other call queue content and corrected PowerShell examples for creating/assigning recording templates. Clarified how to obtain the CallQueueGUID and apply templates, reducing configuration errors.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-setup-call-queue-recording-automatic

- **Setup - Compliance Recording for Call Queues**

  Introduced modular includes for standardized prerequisites and setup, and reorganized PowerShell steps to list templates before assignment. Improved configuration examples, including text-to-speech announcements, to streamline compliant recording enablement.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-setup-call-queue-recording-compliance

- **Microsoft Teams apps/Line of Business (LOB) app support on Teams panels**

  Clarified that LoB apps aren’t currently displayable on panels and only the Nearby Rooms app is enabled, removing the prior version-specific requirement note. Simplified the intro to reflect that the current release supports static web content, aligning expectations with actual capabilities.

  https://learn.microsoft.com/en-us/microsoftteams/app-support-on-Teams-panels

- **Teams Rooms on Android certified devices**

  Added four Cisco devices (Desk Pro G2, Room Kit Pro G2, Board Pro G3 55, Board Pro G3 75) with firmware, app versions, and release date details. This keeps procurement lists current and helps ensure device compatibility.

  https://learn.microsoft.com/en-us/microsoftteams/devices/certified-hardware-android

- **End user reporting for security**

  Added instructions for reporting suspicious external users during blocking from chat requests and profile cards, with an illustrative image. Updated settings to distinguish user vs. message reporting and noted that Microsoft Defender currently supports message reporting only, helping admins set accurate expectations.

  https://learn.microsoft.com/en-us/microsoftteams/end-user-reporting-security

- **Release notes for Microsoft Teams Rooms**

  Corrected and consolidated version 5.6.137.0 entries under a single published date, with a note that some features arrived via a web client build. Clarified feature and issue labels to prevent confusion in release history tracking.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/rooms-release-note

- **Supported Conditional Access and Intune device compliance policies for Microsoft Teams Rooms and Teams Android Devices**

  Updated Conditional Access guidance to include Microsoft Intune Enrollment among services that must not be blocked for functionality. This helps avoid device onboarding and management failures.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/supported-ca-and-compliance-policies

- **Teams Bot Identification Program**

  Updated program status to Public Preview and added a Next steps section with a vendor intake form and contact email. This enables partners to join the program and align their bots with identification standards.

  https://learn.microsoft.com/en-us/microsoftteams/teams-bot-identification

- **Teams Device feature comparison (Windows, Android, & Panels)**

  Removed the “Line of business apps” row from customization tables to match current platform capabilities. This prevents misinterpretation when comparing device features.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/teams-devices-feature-comparison

- **Teams Unify Integration Model for Voice Agent**

  Updated certification program messaging to indicate the program is coming soon and removed prior onboarding guidance (intake form and contact). This clarifies current availability and avoids directing vendors to a process that isn’t active yet.

  https://learn.microsoft.com/en-us/microsoftteams/teams-voice-agents

- **Troubleshooting the new optimization**

  Added a Teams Client Health dashboard section in Teams admin center to diagnose VDI issues, including “VDI optimization failure” errors, likely causes, and remediation steps. Encourages proactive monitoring with error code mapping and reporting to reduce end-user impact.

  https://learn.microsoft.com/en-us/microsoftteams/vdi-2-troubleshooting