# Microsoft Teams
**Date created:** 2026-08-29 UTC  
**Tags:** Best Practices, Compliance, Configuration, Guidance, Licensing, Security, Troubleshooting  

## Major Changes

- **Manage end-to-end encryption for Microsoft Teams meetings and one-to-one calls**
  
  Expanded guidance from one-to-one calls to include meetings, with prerequisites, role requirements, and a Teams Premium license requirement for meeting organizers. Added a comprehensive list of features unavailable with E2EE, admin center steps to manage calls and meetings separately, and instructions to verify calls using a 20‑digit security code. Consolidated PowerShell management with examples and detailed platform support and limits, including no Web/VDI/CVI support and a 200‑participant cap for E2EE meetings. The article is reorganized to clarify configuration flow and help admins educate users about security tradeoffs.
  
  https://learn.microsoft.com/en-us/microsoftteams/teams-end-to-end-encryption

## Moderate Changes

- **Setting up Bookable Desks in Microsoft Teams**
  
  Clarified that bookable desks support only peripherals that report a unique serial number to Teams and linked a PowerShell script to verify this. Specified that peripherals are unsupported if the serial number is missing, non-unique, or includes special characters, helping admins prevent deployment issues.
  
  https://learn.microsoft.com/en-us/microsoftteams/rooms/bookable-desks

- **Release Notes for Teams Android Devices Management Apps**
  
  Added release 26.6.3 for Cisco Teams certified devices, including improved root detection for more accurate compliance evaluation and better diagnosability for troubleshooting. This update enhances device security posture and supportability.
  
  https://learn.microsoft.com/en-us/microsoftteams/devices/certified-device-apps

- **Microsoft Teams Premium - Overview for admins**
  
  Clarified E2EE licensing: meeting organizers need Teams Premium to enable E2EE for meetings, while one-to-one E2EE calls do not require Teams Premium. This helps admins plan licenses and set appropriate security expectations.
  
  https://learn.microsoft.com/en-us/microsoftteams/enhanced-teams-experience

- **Plan your deployment for Teams Phones**
  
  Updated best practices to use Teams Pro Management Portal with update rings instead of Teams Admin Center auto-update phases, while retaining phased rollout stages (Validation, General, Final). This aligns device and app updates with modern tooling for more predictable deployments.
  
  https://learn.microsoft.com/en-us/microsoftteams/phones/plan-device-deployment

- **Encryption in Microsoft Teams**
  
  Added notes that E2EE meetings have participant limits and device requirements, and that E2EE is incompatible with compliance recording. Users under compliance recording policies cannot join E2EE calls or meetings, ensuring compliance controls are preserved.
  
  https://learn.microsoft.com/en-us/microsoftteams/teams-encryption

- **Security guide for Microsoft Teams overview**
  
  Refocused encryption coverage on Teams-specific layers and media paths, expanding SRTP details and key negotiation over TLS signaling. Consolidated E2EE key derivation into references to dedicated articles and updated the traffic encryption table, improving clarity and reducing duplication.
  
  https://learn.microsoft.com/en-us/microsoftteams/teams-security-guide