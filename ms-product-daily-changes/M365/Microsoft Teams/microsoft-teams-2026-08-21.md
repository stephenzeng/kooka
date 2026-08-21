# Microsoft Teams
**Date created:** 2026-08-21 UTC  
**Tags:** Compliance, Configuration, Guidance, Identity, Licensing, Security, Troubleshooting  

## Moderate Changes

- **Setup - Direct dial Copilot Studio Voice Agents**

  Updated planning guidance by removing links to Teams Phone Agent-specific pages and adding a link to managing Teams resource accounts. Revised licensing guidance to remove Teams Phone Agent–specific requirements and preview gating details for Copilot Studio integration. These changes streamline prerequisites and reduce confusion.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-direct-mcs

- **Planning - Authorized users for voice applications**

  Reorganized Known issues to separate content for auto attendants and call queues, improving clarity by pulling from distinct include files. Added a dedicated Known issues subsection for Teams Phone Agent authorized users. This separation helps admins quickly locate issue details by feature area.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-plan-authorized-users

- **Planning - Overview of voice applications**

  Added “What’s new” sections for Teams Phone Agent, Auto Attendant, and Call Queue that surface updates from the last six months via includes. This highlights recent changes in one place to simplify release tracking.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-plan-overview

- **Planning - Recording voice applications calls**

  Refined Known issues includes for Call Queue to reference specific Automatic Recording and Compliance Recording files. Added a new “Automatic Recording for Teams Phone Agent” section with known issues. These updates improve precision and expand coverage for recording scenarios.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-plan-recording

- **Planning - Shared Call History for voice applications**

  Expanded Known issues with new subsections for Teams Phone Agents and auto attendants, each using targeted includes. Updated the call queue include reference to the new filename. This makes troubleshooting paths clearer across features.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-plan-shared-call-history

- **Planning - Agents and Queues for Teams Phone Agent**

  Introduced a centralized Known issues section via an include. This brings visibility to current limitations and aids troubleshooting.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-plan-teams-phone-agent-agents-queues

- **Planning - Spam detection for Teams Phone Agent**

  Added a new Known issues section via a shared include to document current limitations. This helps admins quickly assess impact and mitigations.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-plan-teams-phone-agent-spam-detection

- **Planning - Appointment tools for Teams Phone Agent**

  Added a Known issues section using a shared include to surface documented limitations. This improves discoverability of troubleshooting guidance.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-plan-teams-phone-agent-tools-appointments

- **Planning - Questions and Answers tools for Teams Phone Agent**

  Added a Known issues section via a shared include to provide troubleshooting-related details. This ensures issue tracking remains up to date.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-plan-teams-phone-agent-tools-questions-answers

- **Setup - Auto Attendant**

  Expanded Known issues from a placeholder to a structured, collapsible list, noting no known issues in the core service while surfacing feature-specific items via includes. Added a “What’s new for auto attendants in the past six months” section to highlight recent updates. This improves transparency and keeps release information front and center.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-setup-auto-attendant

- **Setup - Shared Call History template for Auto Attendant**

  Replaced the placeholder Known issues with an include that lists specific shared call history issues. Added a “What’s new in Auto Attendant (last six months)” section to track recent changes.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-setup-auto-attendant-template-shared-history

- **Setup - Call Queue via PowerShell**

  Added a “What’s new in Call Queues (last six months)” section via an include. No changes to setup steps or PowerShell examples, keeping procedural guidance stable while surfacing updates.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-setup-call-queue-cmdlets

- **Setup - Teams Phone Agent**

  Replaced a single “None” entry with a comprehensive Known issues section, adding per-feature collapsible items (Agents and queues, Appointments, Authorized Users, Automatic recording, Q&A, Shared call history, Spam) via includes. Added a “What’s new in Teams Phone Agent (last six months)” heading to organize release updates. This centralizes issue tracking and recent changes for faster admin review.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-setup-teams-phone-agent

- **Setup - Teams Phone Agent - Agents and Queues**

  Replaced “None” with an include that surfaces centralized Known issues. Added a “What’s new in Teams Phone Agent (last six months)” heading to frame recent updates.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-setup-teams-phone-agent-agents-queues

- **Setup - Teams Phone Agent Spam Detection**

  Replaced the Known issues placeholder with an include listing current issues for spam detection. Added a “What’s new in Teams Phone Agent (last six months)” section to surface recent changes.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-setup-teams-phone-agent-template-spam-detection

- **Setup - Teams Phone Agent Appointment tools**

  Replaced “None” with an include that lists current Known issues and added a “What’s new in Teams Phone Agent (last six months)” header. No procedural changes; updates focus on discoverability of issues and release notes.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-setup-teams-phone-agent-tools-appointments

- **Setup - Teams Phone Agent Questions and Answers tools**

  Updated Known issues to pull current content via an include and added a “What’s new in Teams Phone Agent (last six months)” section. This keeps troubleshooting and updates easily accessible.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-setup-teams-phone-agent-tools-questions-answers

- **Manage Microsoft Copilot in Teams calls**

  Added an Important note clarifying that when a one-to-one call is escalated to a group call, recording, transcript, Recap, and Copilot artifacts remain tied to the original one-to-one chat. Participants added during escalation cannot access those artifacts, regardless of when recording or transcription started. This sets expectations for compliance and access control.

  https://learn.microsoft.com/en-us/microsoftteams/copilot-teams-calling-transcription

- **Transition to Password-less Teams Shared Space device Resource Accounts**

  Updated administrative role guidance and split permissions between transitioning devices (Teams Administrator) and running the Cleanup Password wizard (User Administrator or Global Administrator). Renamed Step 1 and added notes clarifying required roles and password reset permissions, with pointers to possible RBAC or administrative unit scoping. This clarifies who can perform each action and reduces setup friction.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/passwordlessentraresourceaccounts