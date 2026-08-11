# Microsoft Teams
**Date created:** 2026-08-05 UTC  
**Tags:** Administration, Analytics, Monitoring, Security  

## Major Changes

- **Transitioning Teams Android Device Management from Teams Admin Center to the Teams Rooms Pro Management Portal**

  Expanded transition guidance for Teams Android devices, detailing minimum Admin Agent versions, accelerated and mandatory update behavior, and how non-compliant devices are handled. Clarified enrollment for Teams Phones, ring behavior that may update devices faster than configured schedules, and defaulting of non-compliant phones to the General ring with a nightly window. Revised feature availability timelines across public and government clouds, adding items such as custom backgrounds and Tags as Groups, with adjusted dates for update management, remote actions, and SIP device management. This helps admins plan migrations off TAC, keep devices manageable, and align expectations for rollout timing.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/aboutunifieddevicemanagement-pmp1

- **Manage updates for Teams android devices in Pro Management portal (PMP)**

  Updated update policies to start the maintenance window at 12 AM and clarified that pausing/resuming Android updates requires Global-level permissions (included in Global and Teams admin roles). Introduced minimum Admin Agent version requirements with accelerated, non-pausable updates to ensure manageability, plus an irreversible transition from TAC phases to PMP rings. Added detailed behavior for devices below minimum versions, prerequisites for Teams Phones, and guidance for government clouds and end-of-support devices. These changes tighten governance, reduce fragmentation, and ensure devices remain supported and controllable in PMP.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/androidupdatemanagementinpmp

## Moderate Changes

- **Setup - Automatic Recording for Call Queue**

  Added support for automatic transcription alongside recording and clarified prerequisites, including SharePoint enablement and supported call answering modes. Improved guidance on SharePoint ownership, template immutability, default settings, and announcement wording, and removed the preview limitation. Requires Microsoft Teams PowerShell module 7.8.0 or later to ensure compatibility and manageability.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-setup-call-queue-recording-automatic

- **Release Notes for Teams Android Devices Management Apps**

  Updated release notes with Admin Agent 830 and 856, added version aliases, and clarified cloud availability plans. Government clouds will skip 830 and receive 856, aligning releases and expectations across environments.

  https://learn.microsoft.com/en-us/microsoftteams/devices/certified-device-apps

- **Intelligent media quality classifiers in Call Quality Dashboard (CQD)**

  Refreshed model update dates to reflect the latest model as of August 4, 2026 and streamlined the historical updates list. Removed the prior limitation note to present a clearer, current view of classifier updates.

  https://learn.microsoft.com/en-us/microsoftteams/cqd-intelligent-media-quality-classifiers

- **Use Power BI to analyze CQD data for Microsoft Teams**

  Replaced the legacy Teams Auto Attendant & Call Queue Historical Reports templates with the new consolidated Auto Attendant & Call Queue Historical Report. Guidance now directs admins to download and use the new report for ongoing analysis.

  https://learn.microsoft.com/en-us/microsoftteams/CQD-Power-BI-query-templates

- **Transition to Password-less Teams Shared Space device Resource Accounts**

  Added business benefits for password-less resource accounts, including reduced credential overhead, stronger security with device-bound tokens, and improved sign-in resilience. Provided a clear migration flow, noted that passwords aren’t removed yet in Entra ID (future phase), and refined prerequisites and portal requirements. This helps organizations move to safer, more manageable shared device accounts with predictable behavior and rollback safeguards.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/passwordlessentraresourceaccounts

- **Set as a Resource Accounts for Shared Devices in Teams Rooms Pro Management**

  Streamlined guidance to focus on setting device-dedicated accounts as resources in Entra ID and documented the benefits, including restricted access to personal and shared content and better governance. Added a step-by-step portal procedure and clarified background processing and status, reducing ambiguity for admins.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/set-as-resource-account-for-shared-teams-devices

- **Manage a Microsoft Teams Rooms console settings remotely with an XML configuration file**

  Added an important recommendation to use the Teams Rooms Pro Management Portal for individual and bulk settings instead of XML, noting that new XML settings won’t be published. Points admins to centralized device settings management to simplify configuration and ensure coverage of all current options.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/xml-config-file