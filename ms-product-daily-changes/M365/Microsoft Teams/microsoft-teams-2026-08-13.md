# Microsoft Teams
**Date created:** 2026-08-13 UTC  
**Tags:** Analytics, Configuration, Deprecation, Governance, Guidance, Security, Troubleshooting  

## Major Changes

- **Transitioning Teams Android Device Management from Teams Admin Center to the Teams Rooms Pro Management Portal**

  Added detailed guidance for handling offline devices, devices on older Admin Agent versions, and devices that remain signed out, including the Zero-Day Update path for Admin Agent 794+ and manual OEM firmware updates for earlier versions. Introduced direction for unsupported or end-of-life devices with a comprehensive device list and expectations for getting to a supported Admin Agent version. Reorganized requirements and timelines, separating minimum app versions from feature availability and adding a “Specific feature availability in PMP” section. These updates streamline the transition to PMP and reduce friction in bringing devices into compliant, manageable states.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/aboutunifieddevicemanagement-pmp1

- **Manage updates for Teams android devices in Pro Management portal (PMP)**

  Introduced new sections and FAQs covering offline devices, upgrading from older Admin Agent versions, devices that remain signed out, and handling unsupported or end-of-life hardware. Expanded FAQs explain how to force updates, maintenance window behavior, where to view updates in PMP, TAC manual updates during deprecation, pausing updates (PMP only), ring duration parity, SIP device support, and training resources. Minor text cleanups were made without changing guidance. These additions improve clarity, reduce update failures, and help admins standardize Android device lifecycle management.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/androidupdatemanagementinpmp

## Moderate Changes

- **Reporting - Voice applications historical reports**

  Added shared include content to standardize guidance and reporting details for Teams Phone Agents, Auto Attendants, and Call Queues historical reports. This improves consistency and reuse without changing core reporting behavior.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-report-historical

- **Setup - Automatic Recording template for Call Queue**

  Updated Known issues to call out that SharePoint structure or permission changes can block access or break automatic recordings, and that the Teams admin must also be a SharePoint site admin for template management. This clarifies prerequisites and helps prevent recording failures.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-setup-call-queue-template-recording-automatic

- **Setup - Teams Phone Agent**

  Added an August 12, 2026 “What’s new” entry announcing spam detection routing options and linked to dedicated guidance. Also clarified dates for earlier updates to improve change tracking.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-setup-teams-phone-agent

- **Setup - Automatic recording for Teams Phone Agent**

  Added a Known issues section noting that SharePoint site or permission changes can cause access issues or automatic recording failures. Clarified that assigning or managing templates requires the Teams admin to be a SharePoint site admin, helping avoid onboarding and recording issues.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-setup-teams-phone-agent-template-recording-automatic

- **Release Notes for Teams Android Devices Management Apps**

  Updated release notes for Admin Agent 1.0.0.202607160723 (856) to reflect expanded availability to Public/WW, GCC-H, and DoD (GCC pending), a faster mandatory rollout cadence, and possible backdated publish dates. Clarified that prior version 1.0.0.202606082157 won’t release to Government clouds and noted similar rollout and mandatory update details for public cloud, helping admins plan deployments and compliance windows.

  https://learn.microsoft.com/en-us/microsoftteams/devices/certified-device-apps

- **Teams Rooms certified systems and peripherals**

  Moved the Logitech Tap and Intel Tiger Canyon NUC PC from the Certified list to the End of Service/Life list. Admins should plan lifecycle transitions and avoid new deployments of this hardware.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/certified-hardware

- **Usage reports in the Teams Management Pro portal**

  Updated behavior notes: events are calculated in each device’s local time zone; usage now focuses on room-level metrics with host names removed from the UI (still available in CSV); and utilization reflects both reservations and actual occupancy. The Usage Details trend chart is temporarily removed pending enhancements; People Count now includes Cloud IntelliFrame; and exports ship as compressed files without a metadata header row. These changes align reporting with room-centric insights and streamline exports.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/usage-reports