# Microsoft Teams
**Date created:** 2026-08-20 UTC  
**Tags:** Compliance, Configuration, Deprecation, Governance, Guidance, Identity, Licensing, Monitoring, Security, Troubleshooting  

## New Articles

- **Create a Support Request for Teams Devices**

  Introduced guidance for creating Microsoft support requests for Teams devices and the Teams Rooms Pro Management Portal. Clarifies supported device types, required admin roles, and prerequisites. Provides step-by-step submission paths via the Pro Management Portal or Microsoft 365 Admin Center and details the diagnostic information to include. Adds device-specific data collection (logs, versions, peripherals) to speed resolution.

  https://learn.microsoft.com/en-us/microsoftteams/devices/how-to-get-support

- **Teams Device Known Issues**

  Added a consolidated catalog of known issues and workarounds across Teams Rooms on Windows/Android, panels, phones, and displays. Highlights sign-in and policy-related behaviors, device limitations, interoperability caveats, and hardware-specific mitigations. Provides targeted fixes for audio/video reliability, USB stability, proxy and update behaviors, and cross-platform meeting joins. Helps admins quickly identify symptoms, map to root causes, and apply tested resolutions.

  https://learn.microsoft.com/en-us/microsoftteams/devices/known-issues

- **Teams Pro Management Portal Alert - Bluetooth Disabled**

  Added troubleshooting for the Bluetooth Disabled alert marked Unhealthy (Warning). Explains that Bluetooth is turned off at the OS level and outlines steps to enable it on Windows or Android-based Teams Rooms devices. Notes that Warning incidents do not impact overall device health.

  https://learn.microsoft.com/en-us/microsoftteams/devices/pmpsignal-bluetooth

- **Teams Pro Management Portal Alert - Camera Unhealthy**

  Documented causes and fixes when room cameras are unavailable or misconfigured. Clarifies differences between room, default, and content camera alerts and how hardware changes affect defaults. Guides admins through power, cabling, firmware, and reset checks to restore video.

  https://learn.microsoft.com/en-us/microsoftteams/devices/pmpsignal-camera-status-unhealthy

- **Teams Pro Management Portal Alert - CPU Performance Limited**

  Explained why CPU performance may be throttled due to Windows power settings and how that triggers a Warning. Describes automatic remediation by Teams Rooms Pro and how to correct conflicting GPO/MDM configurations. Provides command-line, Control Panel, and Intune-based methods to set the maximum processor state to 100%.

  https://learn.microsoft.com/en-us/microsoftteams/devices/pmpsignal-cpu-performance-unhealthy

- **Teams Pro Management Portal Alert - Disk Space Unhealthy**

  Introduced a detailed remediation playbook for low disk space conditions on Teams Rooms devices. Outlines automated cleanup actions performed by Teams Rooms Pro and when manual cleanups are needed. Describes thresholds, timing to avoid disruption, and post-remediation outcomes.

  https://learn.microsoft.com/en-us/microsoftteams/devices/pmpsignal-disk-space

- **Teams Pro Management Portal Alert - Front of Room Display Unhealthy**

  Added guidance to resolve undetected or blank Front of Room displays. Recommends validating HDMI paths (cables, extenders, adapters), power states, and EDID devices, and preferring native HDMI. Provides best practices for display power/CEC behaviors that reduce false alarms without affecting health status.

  https://learn.microsoft.com/en-us/microsoftteams/devices/pmpsignal-front-of-room-display

- **Teams Pro Management Portal Alert - HDMI Ingest Unhealthy**

  Added root-cause analysis and resolution steps for HDMI/USB‑C ingest failures. Covers cable integrity, separate ingest module checks, firmware and Windows updates, and OEM guidance. Helps admins quickly restore in-room content sharing.

  https://learn.microsoft.com/en-us/microsoftteams/devices/pmpsignal-hdmi-ingest

- **Teams Pro Management Portal Alert - Meeting App Unhealthy**

  Documented critical conditions where the Teams Rooms meeting app can’t sign in or run correctly. Provides targeted fixes for auto sign-in, account conflicts, black/gray screens, and multi-version app states. Includes registry settings, remediation flags, and reimage guidance to restore app health.

  https://learn.microsoft.com/en-us/microsoftteams/devices/pmpsignal-meeting-app-status

- **Teams Pro Management Portal Alert - Microphone or Speaker Status Unhealthy**

  Added diagnostics for audio device availability and configuration issues. Explains when fallback applies, how non-viable devices are filtered, and special handling for HDMI display speakers. Outlines power, cabling, firmware, and supported extender checks to restore bidirectional audio.

  https://learn.microsoft.com/en-us/microsoftteams/devices/pmpsignal-microphone-speaker-status

- **Teams Pro Management Portal Alert - Default Credentials in use**

  Introduced security guidance when devices retain OEM default local admin passwords. Recommends changing the admin password and using Windows LAPS for rotation. Provides governance practices for administrative access and account alternatives.

  https://learn.microsoft.com/en-us/microsoftteams/devices/pmpsignal-mtrw-default-credentials

- **Teams Pro Management Portal Alert - OS Edition Unhealthy**

  Clarified that unsupported Windows editions prevent Teams Rooms from operating properly. Guides admins to verify certified hardware and reimage to Windows IoT Enterprise or Windows Enterprise (GA channel). Notes certified systems ship with the correct OS edition.

  https://learn.microsoft.com/en-us/microsoftteams/devices/pmpsignal-os-edition

- **Teams Pro Management Portal Alert - Teams Sign-in Errors**

  Added a complete diagnostic path for resource account sign-in failures. Combines automated Remote Connectivity Analyzer tests with manual checks for MFA/CA policies, credentials, licensing, and mailbox presence. Maps common AADSTS codes to actionable remediation steps.

  https://learn.microsoft.com/en-us/microsoftteams/devices/pmpsignal-resource-account-sign-in

- **Teams Pro Management Portal Alert - Sleep Timer**

  Explained how nonzero “Sleep after” settings trigger a Warning and can disrupt device availability. Details automatic remediation and how to align GPO/MDM policies. Provides command-line, Control Panel, and Intune script methods to set the value to 0.

  https://learn.microsoft.com/en-us/microsoftteams/devices/pmpsignal-sleep-timer

- **Teams Pro Management Portal Alert - Unmonitored or Offline Health Status**

  Added end-to-end diagnostics for devices that appear Unmonitored or Offline. Covers agent health, TPM, scheduled tasks, portal/device presence, proxy and endpoint connectivity (including WebSockets), and OS events indicating shutdowns or startup failures. Provides log locations and collection steps to expedite support engagement.

  https://learn.microsoft.com/en-us/microsoftteams/devices/pmpsignal-unmonitored-offline

- **Teams Pro Management Portal Alert - USB Peripheral Power Drain**

  Documented USB device resets caused by Windows power behavior after display off/sleep. Describes automatic remediation by the Pro agent and provides registry, PowerShell, and Intune options to disable the behavior. Reduces post-wake peripheral failures.

  https://learn.microsoft.com/en-us/microsoftteams/devices/pmpsignal-usb-peripherial-power-drain

- **Teams Pro Management Portal Alert - USB Selective Suspend**

  Explained how USB selective suspend can leave peripherals unresponsive after sleep and why the signal shows Warning. Notes automated remediation and offers powercfg, Control Panel, and Intune methods to disable selective suspend when plugged in. Improves stability for room peripherals.

  https://learn.microsoft.com/en-us/microsoftteams/devices/pmpsignal-usb-selective-suspend

- **Teams Pro Management Portal Alert - Windows Update Unhealthy**

  Added a troubleshooting guide to restore Windows Update health and security compliance. Covers disk cleanup, policy conflicts, proxy/multipart download requirements, and targeted fixes for prevalent error codes using CBS.log and DISM. Includes steps to verify Teams Rooms app version compatibility.

  https://learn.microsoft.com/en-us/microsoftteams/devices/pmpsignal-windows-update

- **Collect Teams Device Logs**

  Introduced methods to collect diagnostic logs via the Teams Rooms Pro Management Portal and locally on Teams Rooms on Windows. Provides a PowerShell-based collection workflow and guidance for Android devices using OEM tools. Streamlines evidence gathering for support cases.

  https://learn.microsoft.com/en-us/microsoftteams/devices/troubleshooting-collect-device-logs

- **Teams Rooms app doesn't start automatically after a Windows update**

  Added remediation for cases where the Teams Rooms app fails to start after Windows updates. Guides admins to confirm OS version support, collect logs, and use the recovery tool to return to a supported state. Recommends adjusting update policies to prevent recurrence.

  https://learn.microsoft.com/en-us/microsoftteams/devices/troubleshooting-mtrw-app-launch-after-updates

- **Blank screen on a Teams Rooms on Windows device**

  Added diagnostics for black/blank screen conditions and unresponsive consoles. Details checks for device health in the portal, process and event log review, and when to power cycle or reimage. Explains expected behavior during OEM firmware updates and how to distinguish display vs. touchscreen issues.

  https://learn.microsoft.com/en-us/microsoftteams/devices/troubleshooting-mtrw-blank-screen

- **On-screen keyboard size is reduced on some Teams Rooms on Windows devices**

  Documented a Windows 11 behavior that reduces on‑screen keyboard height on certain consoles. Provides a configuration workaround to adjust keyboard size and apply it to the Skype account. Includes steps to restart and validate the change.

  https://learn.microsoft.com/en-us/microsoftteams/devices/troubleshooting-mtrw-onscreen-keyboard-size

- **Troubleshoot Conditional Access-related issues for Teams Android devices**

  Added guidance for Android devices affected by Conditional Access and Intune compliance policies. Explains how to detect failing policies using connectivity tests and Entra sign-in logs and how to exclude devices using filters. Recommends supported policy configurations to avoid sign-in loops and instability.

  https://learn.microsoft.com/en-us/microsoftteams/devices/troubleshooting-teams-android-device-conditional-access

- **Teams Android Devices get signed out**

  Introduced a troubleshooting path for Android devices that automatically sign out. Shows how to identify affected devices in Entra sign-in logs and run targeted Remote Connectivity Analyzer tests. Provides recovery steps per device type, prerequisites, and cleanup guidance for directory objects when resetting.

  https://learn.microsoft.com/en-us/microsoftteams/devices/troubleshooting-teams-android-signed-out

## Major Changes

- **Teams Rooms and Devices feature comparison**

  Updated comparison tables by removing Teams Admin Center feature rows and reflecting expanded Pro Management Portal capabilities. Device Settings Management, Update Management, and Log Collection are now shown as Available across compared platforms. This clarifies where admins should manage devices and reduces confusion about feature parity after recent portal enhancements.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/teams-devices-feature-comparison

## Moderate Changes

- **Planning - Authorized users for voice applications**

  Added a Known issues section specific to Authorized Users to surface current limitations and workarounds. This helps admins anticipate behavior and plan deployments more confidently.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-plan-authorized-users

- **Planning - Call priorities for Call Queues**

  Introduced a Known issues section for call queue priorities, consolidating current limitations. This enables more informed configuration and expectation setting.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-plan-call-queue-priorities

- **Planning - Recording voice applications calls**

  Added Known issues for automatic and compliance recording scenarios via dedicated includes. This clarifies constraints and guides admins toward supported recording configurations.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-plan-recording

- **Planning - Shared Call History for voice applications**

  Added a Known issues section for Shared Call History in call queues. Admins can now review limitations upfront and adjust rollout plans accordingly.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-plan-shared-call-history

- **Reference - Supported Configurations**

  Added a Templates and resources section that documents key limits and allowances, including phone number lists and tag limits. This provides clearer boundaries for scalable, compliant deployments.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-reference-limits-supported-configurations

- **Setup - Call Queue**

  Expanded Known issues with an organized, feature-based list and added a “What’s new” section summarizing recent updates. This improves troubleshooting efficiency and keeps implementers current.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-setup-call-queue

- **Setup - Call Priorities for Call Queues**

  Replaced “None” with a dynamic Known issues include and added a clear “What’s new” header. This makes it easier to discover current issues and recent changes affecting call priorities.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-setup-call-queue-priorities

- **Setup - Compliance Recording for Call Queues template**

  Updated Known issues using a dedicated include and reorganized recent updates under a new “What’s new” section. This improves accuracy and discoverability for compliance recording guidance.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-setup-call-queue-template-recording-compliance

- **Setup - Shared Call History template for Call Queue**

  Replaced placeholder Known issues with a live include and broadened “What’s new” from the feature level to call queues overall. These changes keep the page current and reduce maintenance overhead.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-setup-call-queue-template-shared-history

- **Teams Rooms app and Windows versioning support - overview**

  Updated update channels to reflect delivery via the Pro Management Portal, clarified release support policy, and streamlined Windows feature update guidance. Pruned outdated Windows 10 entries and added a “Supported device lifecycle” section with links to certified device end-of-service. Simplified Surface Hub guidance and removed legacy related topics to focus on actionable lifecycle management.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/rooms-lifecycle-support

- **Health signals**

  Refreshed the health signal catalog: removed obsolete signals, added OS edition, and standardized names. Renamed “Offline” to “Unmonitored” and expanded panel signal coverage. These updates improve clarity and alignment with current monitoring behaviors.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/signals