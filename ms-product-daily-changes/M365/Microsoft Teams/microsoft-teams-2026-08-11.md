# Microsoft Teams
**Date created:** 2026-08-11 UTC  
**Tags:** Compliance, Configuration, Deprecation, Guidance, Security, Troubleshooting  

## New Articles

- **Plan - Spam detections for Teams Phone Agent**

  Introduced planning guidance for detecting and handling spam calls in Teams Phone Agent. Explains default behavior that automatically identifies and disconnects suspected spam and how to use a Spam Detection template to redirect such calls to safer destinations. Covers creating allow and deny lists for numbers that should always be permitted or always treated as spam, plus licensing considerations and links to related planning and setup topics.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-plan-teams-phone-agent-spam-detection

- **Setup - Spam Detection template for Teams Phone Agent**

  Added a step-by-step setup article for configuring Spam Detection templates via PowerShell. Defines template components (enablement, actions, targets, and include/exclude number scopes), notes the Microsoft Teams PowerShell 7.9.1-preview or later requirement, and provides examples for common policies like disconnecting or redirecting spam. Includes instructions to assign a template to a Teams Phone Agent for consistent call handling.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-setup-teams-phone-agent-template-spam-detection

## Major Changes

- **Plan for Operator Connect for India**

  Overhauled planning guidance to clearly separate wireline and wireless scenarios, licensing, and device behavior. Clarifies that the India-specific Teams Phone license must be obtained from an Indian operator and that users must be in TeamsOnly mode, while resource accounts can use Operator Connect for India numbers without that license. Details LBR requirements for wireline numbers, wireless roaming and location handling on clients, and emergency location prerequisites for Teams IP phones and Teams Rooms. Adds location consent steps, device and client limitations, number-type compatibility rules, and notes on OSP deployments to help admins design compliant, reliable deployments.

  https://learn.microsoft.com/en-us/microsoftteams/operator-connect-india-plan

- **Teams Rooms app and Windows versioning support - overview**

  Updated Windows support to add 25H2 as Supported and Recommended with a minimum app version of 5.6.210.0. Adjusted 24H2 to Supported (no longer Recommended) and marked 23H2 as Not Supported. This helps admins plan OS upgrades and app version targets to keep Teams Rooms in a supported state.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/rooms-lifecycle-support

## Moderate Changes

- **Plan - Recording for Teams Phone Agent, Auto Attendant, and Call Queue calls**

  Refreshed the sourced content by switching to new description includes for automatic and compliance recording across Teams Phone Agent and call queues. This improves consistency and clarity in planning guidance for recording scenarios.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-plan-recording

- **Plan - Shared Call History for Call Queue and Auto Attendant**

  Updated the shared call history sections to use new description includes for both call queues and auto attendants. The revisions align terminology and improve the accuracy of planning guidance.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-plan-shared-call-history

- **Plan - Templates and Resources**

  Added a new Spam detection templates section and updated multiple template references to new description includes. This consolidates planning resources and highlights anti-spam controls for more effective call handling.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-plan-templates-resources

- **Setup - Teams Phone Agent**

  Reorganized call flow setup into distinct “Greeting options” and “Call routing options” subsections with anchors for better navigation. The structure clarifies configuration choices and speeds up deployment.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-setup-teams-phone-agent

- **Teams Rooms on Android certified devices**

  Added a new certified room kit and inserted August 10, 2026 firmware listings for multiple Logitech devices, including updated Teams and management component versions. Device admins can validate compatibility and plan firmware rollouts with current baselines.

  https://learn.microsoft.com/en-us/microsoftteams/devices/certified-hardware-android

- **Teams policy packages for government**

  Removed the private preview notice for assigning a policy package to a group, indicating general availability. Government admins can confidently use group-based policy package assignment in production.

  https://learn.microsoft.com/en-us/microsoftteams/policy-packages-gov

- **Release notes for Microsoft Teams Rooms**

  Added the August 2026 release entry with fixes for HDMI sharing issues on Poly devices and a fix for devices entering sleep during Town hall. These updates improve meeting reliability and content sharing.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/rooms-release-note

- **Certified Teams panels**

  Added new firmware entries for TAP Scheduler (VR0028) and DockFlex (VR0035) with aligned Teams client, Intune, Authenticator, and Admin Agent versions dated August 10, 2026. Use these versions to maintain certified configurations and streamline updates.

  https://learn.microsoft.com/en-us/microsoftteams/devices/teams-panels-certified-hardware