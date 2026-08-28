# Microsoft Intune
**Date created:** 2026-08-28 UTC  
**Tags:** Configuration, Guidance, Monitoring, Security, Troubleshooting  

## New Articles

- **Security update for the SMS Provider and administration service**

  Introduced a new hotfix article (KB 38982839) for Configuration Manager current branch 2603 and versions 2509/2503 to address security issues in the SMS Provider and administration service. Provides installation guidance via Updates and Servicing, notes on restarts/site reset, and steps to update secondary sites, including a SQL query to verify status. Highlights a defense-in-depth recommendation related to CVE-2026-26128 and advises installing the relevant Windows security update. Includes file lists, release history (initial August 2026), and references to related servicing documentation.

  https://learn.microsoft.com/en-us/intune/configmgr/hotfix/2603/38982839

- **Device action: Enhanced logging**

  Added a how-to article for the Enhanced log collection device action on supervised Apple platforms, supporting macOS and iOS/iPadOS 27+. Explains required permissions, AppleCare token usage, and steps to start or cancel enhanced log collection from Intune. Describes monitoring via the DDM status channel and clarifies that logs upload directly to Apple and are not downloaded from Intune. Provides links to related Intune docs and Apple’s command reference.

  https://learn.microsoft.com/en-us/intune/device-management/actions/apple-enhanced-logging

- **Settings list for the Windows 365 for Agents security baseline in Intune**

  Published a new reference for the Windows 365 for Agents security baseline (version 24H1) detailing default settings across security, Defender, ASR, firewall, Device Guard, credential protections, browser/network controls, and more. Helps admins understand enforced defaults for Cloud PCs running agentic workloads, with links to relevant CSP documentation. Includes notes on baseline versioning behavior to support planning and governance.

  https://learn.microsoft.com/en-us/intune/device-security/security-baselines/ref-windows-365-agents-settings

## Moderate Changes

- **Security update for Microsoft Configuration Manager versions 2409, 2503**

  Clarified that for version 2503 this update is superseded by KB 38982839, while the article remains applicable to version 2409. Updated the release history with an August 2026 entry so admins deploy the correct update moving forward.

  https://learn.microsoft.com/en-us/intune/configmgr/hotfix/2503/37447175

- **How to Manage iOS and macOS Apps Purchased Through Apple Business Manager with Microsoft Intune**

  Added a new Management type setting to choose MDM (default) or DDM for managing VPP apps, with guidance on DDM benefits for iOS/iPadOS 18+ (faster delivery, real-time status, richer attributes). Noted that DDM currently doesn’t support available assignments (only Required or Uninstall), helping admins plan deployment strategies; minor formatting updates included.

  https://learn.microsoft.com/en-us/intune/app-management/deployment/manage-vpp-apple

- **Use security baselines to help secure Windows devices you manage with Microsoft Intune**

  Added the Windows 365 for Agents security baseline (version 24H1) to the available baselines and the Create profile list, with a link to its settings reference. This enables organizations to apply a preconfigured security posture for agentic Cloud PC workloads.

  https://learn.microsoft.com/en-us/intune/device-security/security-baselines/overview

- **Microsoft Intune Protected Apps**

  Expanded the protected partner apps list with new options including Ben for Intune, Calven, Heijmans, Notability, Notion, SDP - On Premises | Intune, and Superhuman Mail. The additions give admins more choice when applying app protection policies, with app details and store links for Android and iOS.

  https://learn.microsoft.com/en-us/intune/app-management/ref-protected-apps

- **Set up enrollment of Android Enterprise personally owned work profile devices**

  Updated web-based enrollment requirements to include the Samsung browser alongside Chrome and Edge. Removed outdated guidance about MFA phone call issues and workarounds, streamlining enrollment expectations and reducing confusion.

  https://learn.microsoft.com/en-us/intune/device-enrollment/android/setup-personal-work-profile