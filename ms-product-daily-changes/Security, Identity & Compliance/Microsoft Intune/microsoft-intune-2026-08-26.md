# Microsoft Intune
**Date created:** 2026-08-26 UTC  
**Tags:** Configuration, Deprecation, Governance, Guidance, Licensing, Monitoring, Security, Troubleshooting  

## Major Changes

- **What's new in previous months in the Microsoft Intune**

  Added the February 9, 2026 (Service release 2601) archive entry highlighting broad updates across advanced capabilities, app management, device configuration, device management, security, reporting, and tenant administration. Notable improvements include user-based EPM on AVD single-session VMs, new protected apps, and expanded Windows settings (Edge v143 policies, firewall audit mode, Windows AI agent, Chrome ADMX updates). Android gained OEMConfig apps and management-mode filtering; Apple catalogs and terminology were updated. Admin experiences improved with granular assignment filter values, Zimperium iOS certificate inventory sync, Windows 11 25H2 feature update reporting, and GA of consolidated Admin tasks.

  https://learn.microsoft.com/en-us/intune/whats-new/archive

- **Deploy Remote Help with Microsoft Intune**

  Updated deployment guidance to support Windows unattended assistance, including new prerequisites, RBAC requirements, and clear separation from attended workflows. Introduced step-by-step Win32 app packaging and dependency setup for the AVD agent and bootloader, plus configuration to enable Remote Desktop via settings catalog. Clarified that built-in Help Desk Operator lacks the permission for Windows unattended remote sign-in and that a custom role is required. Reorganized content to make attended vs. unattended deployment paths and ongoing update behaviors easier to follow.

  https://learn.microsoft.com/en-us/intune/remote-help/deploy

- **What's new in Microsoft Intune**

  Added the Week of August 25, 2026 (Service release 2608) updates, including unattended Remote Help for Windows, Apple DDM support for required VPP apps, expanded Android and Apple settings, new Windows catalog items, enhanced enrollment controls, improved device management and inventory, and security additions for Linux Defender AV and a Windows 365 for Agents baseline. Streamlined device operations with a new single device page (default), GA for operatingSystemVersion in filters, improved eSIM actions, and broader Android inventory support. Also removed the older February 9, 2026 (2601) block and consolidated related Remote Help guidance clarifications around unattended control, RBAC, Conditional Access applicability, and attended-only chat.

  https://learn.microsoft.com/en-us/intune/whats-new/

- **Plan for Remote Help with Microsoft Intune**

  Expanded planning guidance to govern unattended access, including dedicated custom roles, device scoping, and stricter Conditional Access for helpers. Clarified capabilities by separating attended vs. unattended modes and noting that Windows experiences use separate apps. Overhauled RBAC with renamed permissions (“Remote Help app - …”) and new permissions for Android unattended and Windows unattended remote sign-in, with updated built-in role mappings. Refreshed Windows requirements for unattended sessions (corporate, Intune-managed, IME, Remote Desktop enabled, powered/online) and consolidated cross-platform requirements and operational guidance.

  https://learn.microsoft.com/en-us/intune/remote-help/plan

- **Using Remote Help on Windows to Assist Authenticated Users**

  Introduced a comprehensive attended vs. unattended model for Windows sessions launched from Intune, including permissions, prerequisites, session limits, notifications, and reclaim/lock behaviors. Added an end-user note explaining unattended requests and the 30-second auto-start with the ability to reclaim the device. Reorganized Windows content into a dedicated Intune-launched flow, updated Windows native app guidance (including unenrolled device help), and reinforced AVD targeting with security codes. Streamlined macOS flows, clarified first-time sign-in, updated UI labels, and added unenrolled macOS assistance steps.

  https://learn.microsoft.com/en-us/intune/remote-help/start-session

## Moderate Changes

- **In development - Microsoft Intune**

  Removed the “Audit mode for the Microsoft Defender Antivirus template for Linux” section that previously described upcoming behavior for Audit enforcement. The page no longer lists that future change for Intune-managed or MDE-attached Linux devices.

  https://learn.microsoft.com/en-us/intune/whats-new/in-development

- **Assignment filter properties and operators reference**

  Updated the reference to reflect GA for operatingSystemVersion and removed prior public preview notes. Clarified that osVersion is deprecated for creating new filters, while existing filters that use it continue to function.

  https://learn.microsoft.com/en-us/intune/fundamentals/filters/ref-device-properties

- **Vulnerability Remediation Agent in Microsoft Intune**

  Clarified licensing: the agentic user must be licensed unless “Allow admins without an Intune license” is enabled in Tenant administration > Roles > Settings. This helps avoid setup failures and ensures compliant access.

  https://learn.microsoft.com/en-us/intune/copilot/agents/vulnerability-remediation-agent