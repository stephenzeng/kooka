# Microsoft Teams
**Date created:** 2026-08-26 UTC  
**Tags:** Best Practices, Compliance, Configuration, Governance, Guidance, Licensing, Monitoring, Security, Troubleshooting

## Major Changes

- **Configure digital signage on Teams Rooms**

  Added support to show digital signage on Teams panels, with updated prerequisites including a minimum panels version. Updated terminology and UI to use devices/device groups, revised assignment flows, and introduced a preference to control whether signage appears on panels (including a panels-only option). Split deactivation timers between front-of-room displays and Teams panels and expanded content design guidance for smaller screens. Monitoring, limitations, and unsupported device notes were updated to include panels and to clarify that Cisco devices aren’t supported for Android and panels.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/digital-signage

- **Limits and specifications for Microsoft Teams**

  Increased breakout room capacity by allowing up to 1,000 eligible attendees in meetings and events, and clarified that turning on breakout rooms automatically limits attendance to 1,000. Noted that breakout rooms aren’t supported in events optimized for very large audiences. Removed the outdated notice about temporary Microsoft 365 live event limit increases.

  https://learn.microsoft.com/en-us/microsoftteams/limits-specifications-teams

- **Meetings and events feature and capacity comparison**

  Updated the comparison to reflect breakout rooms availability in meetings and events up to 1,000 attendees, with a footnote clarifying scope. Clarified that breakout rooms aren’t supported above 1,000 attendees.

  https://learn.microsoft.com/en-us/microsoftteams/meetings-events-feature-comparison

## Moderate Changes

- **Transitioning Teams Android Device Management from Teams Admin Center to the Teams Rooms Pro Management Portal**

  Expanded troubleshooting for device visibility and manageability, including detecting the “Device is not connected to IoT Hub” error, clarifying required URL allowlists and minimum Admin Agent versions, and adding a step to ensure unsupported conditional access policies aren’t assigned. Updated end-of-life guidance by linking to official EOL pages and noting Microsoft will provide an Admin Agent for PMP connectivity even if manageability isn’t fully tested.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/aboutunifieddevicemanagement-pmp1

- **Teams Rooms on Android certified devices**

  Added Jabra Panacast 40 VBS and Jabra Panacast TC to the certified Android devices firmware table. Entries include minimum and latest firmware, bundled Microsoft app versions, and the August 24, 2026 release date to guide compliant deployments.

  https://learn.microsoft.com/en-us/microsoftteams/devices/certified-hardware-android

- **What's new in Microsoft Teams devices**

  Introduced digital signage on idle Teams panels with partner integrations and clarified licensing requirements. Added device settings sync from panels to Teams Rooms Pro Management and enhanced desk hub experiences with auto-reservation for connected users and on-device reservation for visitors.

  https://learn.microsoft.com/en-us/microsoftteams/devices/devices-release-notes

- **Route inbound calls in Microsoft Teams**

  Added guidance for per-user Busy on Busy with Teams PowerShell 8.0.0, including the -BusyOnBusyOption parameter (PlayBusySignal, RedirectAsUnansweredCall, RingUser). Clarified precedence between policy and user settings and provided example commands to configure and review user busy behavior.

  https://learn.microsoft.com/en-us/microsoftteams/inbound-call-routing

- **Manage Teams recording expiration policy**

  Expanded policy scope so expiration applies to meetings, webinars, and town halls. Noted that published webinar and town hall recordings expire after 30 days and can be extended to 90 days.

  https://learn.microsoft.com/en-us/microsoftteams/manage-teams-recording-expiration-policy

- **Transition to Password-less Teams Shared Space device Resource Accounts**

  Clarified that new devices must first use username/password before transitioning to password-less. Added details on secure, device-bound token storage (TPM on Windows, Keystore on Android) and refined FAQ wording for eligibility.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/passwordlessentraresourceaccounts

- **Troubleshooting the new optimization**

  Updated guidance for error 3004 (24035) to recommend restarting Teams, explaining it’s typically transient while the plugin stages the media engine. Clarified how 3004 differs from error 2000 by noting a transport exists but the plugin doesn’t respond with “ClientHello.”

  https://learn.microsoft.com/en-us/microsoftteams/vdi-2-troubleshooting