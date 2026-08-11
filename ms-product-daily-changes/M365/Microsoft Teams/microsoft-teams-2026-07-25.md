# Microsoft Teams
**Date created:** 2026-07-25 UTC  
**Tags:** Administration, Analytics  

## Moderate Changes

- **Reference - Supported Configurations**
  
  Updated limits and scoping for Teams Phone Agent, Auto Attendant, and Call Queue to reflect current capabilities, including moving “Dial by name/number” to per Teams Phone Agent, setting holiday sets per Teams Phone Agent to 20, and increasing holiday sets per Auto Attendant to 20. Increased the Call Queue limit for “Maximum added as individual users” from 15 to 20, and aligned terminology and note numbering without changing functionality to improve clarity.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-reference-limits-supported-configurations

- **Reporting - Teams Phone Agent, Auto Attendant, and Call Queue historical reports**
  
  Clarified that publishing a customized report to the Power BI Service disables scheduled refreshes. This helps admins plan report customization versus automation trade-offs.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-report-historical

- **Manage transcript API access for Teams meetings**
  
  Expanded guidance to include management via both the Teams admin center and PowerShell, with clearer steps for enabling Microsoft Graph access and speaker attribution. Added PowerShell parameters (-EnableGraphTranscriptAccess, -EnableAttributedTranscripts) with an example and updated related links for easier administration.

  https://learn.microsoft.com/en-us/microsoftteams/meeting-transcript-api-access

- **New VDI solution for Teams**
  
  Added an ARM-based Citrix Workspace app download option to the plugin list. Introduced July 2026 release notes (2026.29.1.4) detailing fixes for MSIX provisioning/registration on thin clients or kiosk devices, a shift to supporting only split MSIX packages, and security enhancements.

  https://learn.microsoft.com/en-us/microsoftteams/vdi-2