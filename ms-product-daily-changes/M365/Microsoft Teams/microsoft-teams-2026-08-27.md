# Microsoft Teams
**Date created:** 2026-08-27 UTC  
**Tags:** Analytics, Best Practices, Compliance, Configuration, Deprecation, Guidance, Monitoring, Security, Troubleshooting  

## New Articles

- **Device settings available for remote management**
  
  Introduced a comprehensive reference for all device settings that can be managed remotely in the Teams Rooms Pro management portal. The Windows tab details categories such as Account, Meetings, Device, Coordinated meetings, Peripherals, Theming, and Digital Signage, including key options like Front Row, display configuration, content camera enhancements, and tenant-governed signage. This central guide helps admins standardize configurations, streamline troubleshooting, and apply governance consistently. A placeholder indicates that settings for Teams Android devices are coming soon.
  
  https://learn.microsoft.com/en-us/microsoftteams/rooms/device-settings-available

## Major Changes

- **Managing settings for Teams devices**
  
  Clarified that settings management applies only to signed-in devices and that devices process one command at a time; queued commands expire after three days and can be canceled from the Activity page. The page removes the long “Settings available” details, shifting the focus to how commands are processed and managed operationally. This sets clear expectations for reliability and timing of remote actions and redirects admins to the dedicated settings reference for configuration specifics.
  
  https://learn.microsoft.com/en-us/microsoftteams/rooms/pro-portal-settings

## Moderate Changes

- **Reporting - Voice applications historical reports**
  
  Clarified reporting logic so that redirected calls answered due to Call Overflow are attributed to the original queue. Removed an outdated note about investigated discrepancies and reiterated that callbacks handled by agents aren’t tracked, which can cause differences between Call Queue and Agent Timeline reports. These updates help admins interpret metrics more accurately.
  
  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-report-historical

- **Teams Rooms certified systems and peripherals**
  
  Added a new certified DTEN D7X AI Board 55" for Teams Rooms on Windows and updated AudioTechnica ATND1061 firmware support to 1.4.0 in several Q-SYS solutions. Also added the Q-SYS RoomSuite Modular System with defined components and version requirements. These changes guide procurement and ensure deployments meet compatibility standards.
  
  https://learn.microsoft.com/en-us/microsoftteams/rooms/certified-hardware

- **Teams Rooms on Android certified devices**
  
  Clarified that remote control functionality (IR/RF) isn’t supported on Teams Rooms on Android and advised using a certified touch console for meeting and room interactions. This sets accurate expectations and helps avoid unsupported peripherals.
  
  https://learn.microsoft.com/en-us/microsoftteams/devices/certified-hardware-android

- **Manage devices in Teams**
  
  Streamlined guidance for Android device configuration profiles by removing detailed examples and recommending one profile per configuration set. This simplifies setup and promotes consistent, maintainable configurations at scale.
  
  https://learn.microsoft.com/en-us/microsoftteams/devices/device-management

- **Monitor and troubleshoot Teams meetings and calls from the Teams admin center**
  
  Added guidance that event telemetry is available only for presenters and organizers (if participating), not other attendees. Updated the privacy note to state that EUII is obfuscated for federated and external participants per policy, but not obfuscated for P2P calls to support troubleshooting. These clarifications set correct expectations for data visibility and privacy.
  
  https://learn.microsoft.com/en-us/microsoftteams/monitor-troubleshoot-teams-meetings-calls

- **Microsoft Teams Rooms on Windows and Teams Android device security**
  
  Updated network requirements for the Pro Management Portal to specify access over TCP/UDP 443 and standardized the portal name. This helps admins configure firewalls correctly to ensure device connectivity and management reliability.
  
  https://learn.microsoft.com/en-us/microsoftteams/rooms/security