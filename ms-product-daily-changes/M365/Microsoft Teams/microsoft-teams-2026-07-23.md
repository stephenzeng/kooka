# Microsoft Teams
**Date created:** 2026-07-23 UTC  
**Tags:** Administration, Agent, Monitoring, Security  

## New Articles

- **Encryption in Microsoft Teams**

  Introduced a comprehensive overview of how Teams secures communications with standard encryption and optional end-to-end encryption (E2EE). Outlines compliance drivers, standard encryption practices (TLS 1.2+, data-at-rest encryption, service encryption, Customer Key), and detailed E2EE behavior for 1:1 calls and E2EE-required meetings. Clarifies supported modalities, prerequisites (including Teams Premium for E2EE meetings), and key limitations such as no recording, transcription, or PSTN when E2EE is enabled. Provides guidance to choose between standard encryption and E2EE based on risk and explains implications for eDiscovery, DLP, retention, and Copilot.

  https://learn.microsoft.com/en-us/microsoftteams/teams-encryption

## Major Changes

- **Building and endpoint data**

  Expanded the building data schema to include an optional PublicIP column, increasing the format from 15 to 16 columns to better differentiate locations sharing the same private subnet. Updated examples and important notes to demonstrate when and how to populate PublicIP. Added a new section detailing use cases and input format so admins can more accurately map network locations and improve CQD insights.

  https://learn.microsoft.com/en-us/microsoftteams/CQD-upload-tenant-building-data

## Moderate Changes

- **Setup - Shared Call History for Auto Attendant**

  Clarified a limitation: if the same shared voicemail destination is used, you can’t assign different Shared Call History templates across Business Hours, After Hours, or Holiday flows. This helps admins avoid misconfiguration and ensures consistent call history behavior.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-setup-auto-attendant-shared-history

- **Release Notes for Teams Android Devices Management Apps**

  Removed the July 2026 release entry and the entire section for version 1.0.0.202607020009. The page now reflects June 2026 and earlier releases, reducing confusion by removing content that is no longer applicable.

  https://learn.microsoft.com/en-us/microsoftteams/devices/certified-device-apps

- **What is Call Quality Dashboard (CQD)?**

  Added a July 2026 changelog highlighting new Public IP support in building metadata, First/Second Public IP columns, updated transport protocol logic for broader web coverage, and revised user agent categories (including a new VM screenshare category). Removed older 2025 changelog sections to keep the page current and focused.

  https://learn.microsoft.com/en-us/microsoftteams/CQD-what-is-call-quality-dashboard

- **Dimensions and measurements available in Call Quality Dashboard (CQD)**

  Added two new dimensions: First Public IP and Second Public IP, reflecting the public IPs used by each endpoint when provided in building data. These fields improve correlation of media paths and network performance analysis.

  https://learn.microsoft.com/en-us/microsoftteams/dimensions-and-measures-available-in-call-quality-dashboard

- **Manage Teams recording policies for meetings and events**

  Expanded guidance beyond meetings to include 1:1 calls, webinars, and town halls, mapping each to the appropriate policy type and required roles. Clarified convenience versus compliance recording and updated troubleshooting to verify meeting type and related policy settings first.

  https://learn.microsoft.com/en-us/microsoftteams/meeting-recording

- **Monitor and troubleshoot Teams meetings and calls from the Teams admin center**

  Clarified that real-time and aggregate troubleshooting data is available for all users, and refined the User view to include only meetings a user joined. Updated licensing retention details (including Teams Premium and Teams Rooms Pro) and noted telemetry parameters that may be unavailable on Web, VDI, or PSTN.

  https://learn.microsoft.com/en-us/microsoftteams/monitor-troubleshoot-teams-meetings-calls

- **Teams Unify Integration Model for Voice Agent**

  Added a new “Certified Voice Agent solutions” section showcasing providers integrated through the Unify model. Included a certified badge and an initial listing for Audiocodes with a link to its solution, helping customers identify vetted partner options.

  https://learn.microsoft.com/en-us/microsoftteams/teams-voice-agents