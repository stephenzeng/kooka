# Microsoft Teams
**Date created:** 2026-09-04 UTC  
**Tags:** Analytics, Configuration, Deprecation, Guidance, Licensing  

## Major Changes

- **Release notes for Microsoft Teams Rooms**

  Removed the September 2026 release entry and its details from the Teams Rooms release notes. This eliminates references to features previously listed for that release, such as Interpreter agent support, modernized Gallery, town hall chat for organizers/presenters, and SIP/H.323 dialing. Admins and stakeholders should update plans and communications to avoid relying on the withdrawn release content.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/rooms-release-note

## Moderate Changes

- **Reference - Voice applications prerequisites and licensing**

  Added guidance for Teams Phone Agent with Microsoft Bookings, including required dependencies. Clarified that Automatic Recording for Teams Phone Agent needs no additional Teams Phone licensing and directed readers to the SharePoint service description; also linked the same reference for Call Queue recording. These updates streamline licensing decisions and ensure admins use the correct service documentation.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-reference-prerequisites-licensing

- **Setting up Bookable Desks in Microsoft Teams**

  Clarified that summary and desk usage metrics reflect activity only from 8:00 AM to 5:00 PM on weekdays. Updated utilization definitions to align with this measurement window. This ensures reporting and capacity planning are interpreted consistently.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/bookable-desks

- **Microsoft Teams Public preview**

  Added an IMPORTANT note stating device policies do not apply in Teams on the web, and “On for users in Current Channel (Preview)” is treated as Off in the web client. This clarifies how update policies behave for web users so admins can set expectations accurately.

  https://learn.microsoft.com/en-us/microsoftteams/public-preview-doc-updates

- **Teams settings and policies reference**

  Updated the default for the Meeting policy setting StreamingAttendeeMode from Enabled to Disabled. Admins should review meeting policies to ensure the new default aligns with their streaming attendee experience.

  https://learn.microsoft.com/en-us/microsoftteams/settings-policies-reference

- **Install Teams for Virtualized Desktop Infrastructure (VDI)**

  Expanded the deprecation notice for Windows endpoints with specific Omnissa milestones: End of Support on July 1, 2027 and End of Availability on October 1, 2027 (MC post 1465766). Clarified that the new optimization becomes the default and described fallback behavior if optimization fails. This helps VDI administrators plan migrations and validate client behavior.

  https://learn.microsoft.com/en-us/microsoftteams/teams-client-vdi-requirements-deploy

- **Features currently unavailable in Teams for Web**

  Removed the “Early Access | Public Preview” row from the web feature table to reflect current preview behavior. This reduces confusion about preview availability for web users and aligns the table with current policy.

  https://learn.microsoft.com/en-us/microsoftteams/teams-desktop-client-features

- **Teams view-only meeting experience**

  Simplified enablement guidance by removing dependencies on the SkypeForBusiness module and specific module version requirements. Admins are now instructed to use Set-CsTeamsMeetingPolicy directly, reducing setup friction.

  https://learn.microsoft.com/en-us/microsoftteams/view-only-meeting-experience