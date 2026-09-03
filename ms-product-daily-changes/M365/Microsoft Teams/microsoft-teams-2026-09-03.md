# Microsoft Teams
**Date created:** 2026-09-03 UTC  
**Tags:** Analytics, Configuration, Guidance, Monitoring, Performance, Security, Troubleshooting  

## New Articles

- **Camera controls in Teams Rooms**

  Introduced comprehensive guidance for manual camera controls in Teams Rooms, including local pan, tilt, and zoom (PTZ) and camera switching on Windows and Android. Clarifies eligibility requirements (IntelliFrame-supported cameras or devices that report framing state) and notes that Enhanced framing and Multiple camera view disable manual PTZ. Provides setup and management details via XML settings (LocalPtzControlsEnabled and interactions with OemCameraControlsEnabled) plus step-by-step usage instructions. Includes troubleshooting scenarios to help admins and users resolve missing or unavailable PTZ controls.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/camera-controls

## Major Changes

- **Release notes for Microsoft Teams Rooms**

  Added the September 2026 release (1449/1.0.96.2026243501) with multiple feature enhancements. Highlights include Interpreter agent support for real-time translation (Pro), a modernized Gallery view with participant prioritization and admin-configurable defaults, and a private Event Group chat for town halls with the option to switch to attendee chat (Pro). Also introduces support for SIP/H.323 dialing when configured through a supported partner, improving interoperability for meeting scenarios.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/rooms-release-note

## Moderate Changes

- **Transitioning Teams Android Device Management from Teams Admin Center to the Teams Rooms Pro Management Portal**

  Expanded migration guidance for importing Teams admin center Tags as Groups in the Pro Management portal, with clear steps and notes on account-based Tags vs. device-based Groups. Updated timelines and statuses (including GCC/DoD shifts, new Bulk actions row, and refined SIP device management dates) and added an FAQ explaining when actions like Remove/Restart are disabled due to IoTHub connectivity requirements.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/aboutunifieddevicemanagement-pmp1

- **Setting up Bookable Desks in Microsoft Teams**

  Enhanced reporting guidance with clearer definitions, date-range controls, and search options, plus a detailed Desk usage details table. Added a drill-down view showing usage summary, peak utilization by business hours, and meeting performance metrics to help admins monitor adoption and optimize desk capacity.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/bookable-desks

- **Release Notes for Teams Android Devices Management Apps**

  Added the September 2026 supported version 6.2607.4685 and summarized improvements. Updates focus on reliability and device health, stronger security protections with reduced sensitive logging, and richer diagnostics to streamline troubleshooting.

  https://learn.microsoft.com/en-us/microsoftteams/devices/certified-device-apps

- **Certified Teams phones**

  Added MP66 W to the certified firmware table with the latest firmware and included app versions, dated September 02, 2026. This helps admins validate compatibility and plan standardized deployments.

  https://learn.microsoft.com/en-us/microsoftteams/devices/teams-phones-certified-hardware

- **New VDI solution for Teams**

  Announced public preview of town hall attendee optimization on Windows endpoints, with minimum client versions for Teams, Windows app, and partner plugins. Updated feature comparison to reflect attendee optimization support and confirmed interactivity features like live captions, DVR, reactions, streaming chat, Q&A, and eCDNs are supported.

  https://learn.microsoft.com/en-us/microsoftteams/vdi-2

- **Manage a Microsoft Teams Rooms console settings remotely with an XML configuration file**

  Documented a new XML setting, LocalPtzControlsEnabled (enabled by default), to allow in-room participants to control PTZ functions on supported cameras from the console. Clarifies how to enable/manage the setting and links to the camera controls guidance for eligibility and behavior details. This helps admins centrally standardize camera control experiences across rooms.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/xml-config-file