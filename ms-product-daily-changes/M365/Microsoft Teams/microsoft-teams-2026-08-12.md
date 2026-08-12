# Microsoft Teams
**Date created:** 2026-08-12 UTC  
**Tags:** Compliance, Configuration, Get Started, Governance, Guidance, Licensing, Monitoring, Security, Troubleshooting  

## New Articles

- **Setup - Automatic Recording for Teams Phone Agent**

  Introduced end-to-end guidance to create and assign automatic recording templates for Teams Phone Agent, including prerequisites and SharePoint host/site requirements. Added instructions for configuring template fields such as owner, recording and transcription toggles, and customizable announcements. Provided PowerShell setup and assignment examples with verification steps, plus troubleshooting for template creation, file uploads, and validation issues. This helps admins standardize recording policies and streamline deployment at scale.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-setup-teams-phone-agent-template-recording-automatic

## Moderate Changes

- **Planning - Authorized users for voice applications**

  Updated the article scope from specific components to broader “voice applications” and added a related resource for spam detection. This improves clarity and directs readers to relevant security guidance.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-plan-authorized-users

- **Planning - Agents and Queues for Teams Phone Agent**

  Retitled the page and adjusted navigation by updating the Next step link to spam detection and moving third-party voice agents into remaining planning articles. These changes streamline the reading path and make related resources easier to find.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-plan-teams-phone-agent-agents-queues

- **Reference - PowerShell cmdlets for voice applications**

  Retitled the reference to align with the expanded “voice applications” terminology without changing cmdlet content. This keeps guidance consistent while preserving existing scripts and workflows.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-reference-cmdlets

- **Setup - Teams Phone Agent**

  Added a Directory search subsection to business-hours, after-hours, and holidays call flows via a common include. This clarifies configuration steps and helps ensure consistent caller routing.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-setup-teams-phone-agent

- **Teams Rooms on Android certified devices**

  Added August 11, 2026 firmware entries for Barco ClickShare Hub Core, Neat devices, and Shure IntelliMix with corresponding Teams client and app versions. The updates expand supported versions so admins can validate compatibility and plan upgrades confidently.

  https://learn.microsoft.com/en-us/microsoftteams/devices/certified-hardware-android

- **Manage Teams meeting transcription**

  Clarified that, subject to Microsoft Purview retention policies, Copilot prompts and responses may be retained for compliance even when recording and transcription are off in Commercial cloud. Updated availability to note Copilot in Teams isn’t currently available for GCC High and removed a statement limiting post-meeting access, improving compliance and availability guidance.

  https://learn.microsoft.com/en-us/microsoftteams/copilot-teams-transcription

- **Health reports in the Teams Management Pro portal**

  Noted that host names no longer appear in the UI due to a shift to room-level insights, with host names expected to be available via data export by end of August. Reaffirmed that health calculations include offline tickets and that the Active Tickets trend is temporarily unavailable, helping admins interpret report data accurately.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/health-reports

- **Transition to Password-less Teams Shared Space device Resource Accounts**

  Expanded post-transition guidance with a Cleanup Wizard option for eligible accounts, clarified manual password rotation, and documented unsupported scenarios (no hybrid join for Windows, no password removal for hybrid-synced accounts). Added FAQs covering Windows admin mode behavior, device sign-in persistence after password changes, relation to Windows Hello for Business, and token reset implications. Terminology and anchors were aligned to “transition,” improving operational clarity.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/passwordlessentraresourceaccounts

- **Set up common area phones for Microsoft Teams**

  Updated terminology to “Teams Shared Space” licensing and clarified that common area phones use dedicated resource accounts, distinct from Teams Rooms mailboxes. Revised steps and notes to reflect license inclusions and correct account setup, reducing confusion during deployment.

  https://learn.microsoft.com/en-us/microsoftteams/phones/set-up-common-area-phones