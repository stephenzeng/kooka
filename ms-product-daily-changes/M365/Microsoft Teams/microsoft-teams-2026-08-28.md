# Microsoft Teams
**Date created:** 2026-08-28 UTC  
**Tags:** Compliance, Configuration, Governance, Guidance, Performance, Security  

## New Articles

- **Zero-Day Updates for Microsoft Teams Rooms, Teams panels, and Teams phones**

  Introduced zero-day (out-of-box) update behavior for Teams Rooms on Windows and for Teams Rooms on Android, Teams panels, and Teams phones to ensure devices are secure and up to date on first use. Added step-by-step workflows covering prompts, timing, and background actions, plus prerequisites and minimum versions (Teams Rooms on Windows app 4.19.82.0+; Teams Admin Agent 1.0.0.202507210031+ for Android/panels/phones). Included references to release notes and supported versions, and FAQs on why updates can’t be skipped, interaction with manufacturer updates, behavior in government clouds, and URL requirements. This helps admins plan deployment, meet security expectations, and reduce setup friction.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/zero-daydeviceupdates

## Major Changes

- **Manage user feedback in Microsoft Teams**

  Shifted feedback management from Teams-specific policies and PowerShell to the Cloud Policy service for Microsoft 365, centralizing governance and streamlining administration. Removed legacy policy parameters and PowerShell examples, along with platform-specific policy tables and availability notes. Updated end-user “Report a problem” steps and clarified that submitted data is treated as Feedback Data, with links consolidated to new privacy-based feedback management guidance. This aligns feedback handling with Microsoft 365 standards and simplifies policy management.

  https://learn.microsoft.com/en-us/microsoftteams/manage-feedback-policies-in-teams

## Moderate Changes

- **Teams Rooms (Windows and Android) home screen and admin controls**

  Updated the “Give feedback” section to classify submissions as Feedback Data and pointed admins to “Manage Microsoft feedback for your organization.” This clarifies data handling under Microsoft 365/Office 365 agreements and directs admins to the correct governance guidance.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/mtr-home-refresh

- **Teams Bot Identification Program**

  Noted that the public preview has reached capacity and removed onboarding steps, including the intake form and contact details. New onboarding guidance will be published when the program reaches general availability, setting expectations for prospective participants.

  https://learn.microsoft.com/en-us/microsoftteams/teams-bot-identification

- **New VDI solution for Teams**

  Clarified allow-listing guidance for Split MSIX Package architecture with specific SlimCore packages and a consolidated regex pattern. Added Intune configuration details, including the OMA-URI path and an XML example, to enable AllowedNonAdminPackageFamilyNameRules. These updates help ensure reliable deployments and reduce configuration errors.

  https://learn.microsoft.com/en-us/microsoftteams/vdi-2

- **Manage voice recognition for Intelligent Speaker**

  Clarified attendee guidance: limiting in-room participants to 10 is recommended for transcript precision, but more attendees are supported, and the 50 invitee limit applies regardless of in-room count. Increased the recommended upload bandwidth from 7 Mbps to 10 Mbps to improve meeting audio and video quality.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/voice-recognition