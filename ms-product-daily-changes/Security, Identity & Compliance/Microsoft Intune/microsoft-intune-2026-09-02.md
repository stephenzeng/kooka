# Microsoft Intune
**Date created:** 2026-09-02 UTC  
**Tags:** Analytics, Automation, Best Practices, Compliance, Configuration, Guidance, Identity, Licensing, Monitoring, Performance, Security, Troubleshooting  

## Major Changes

- **In development - Microsoft Intune**

  Announced upcoming capabilities across app management, device configuration, enrollment, management, security, and monitoring. Highlights include enforcing Managed Home Screen authentication on shared Android devices, declarative VPP app downloads on iOS/iPadOS, and new Apple settings plus Enforce Routes support in VPN profiles. Device and policy rollout improves with Deployment plans (rings, scheduling, MAA integration), a new default device page, bulk eSIM actions for Android 15+, and expanded Advanced Analytics. Windows Autopatch adds Quality Update approvals and Quick Machine Recovery policies, while Remote Help expands to GCCH and certificate connector health signals improve admin visibility.

  https://learn.microsoft.com/en-us/intune/whats-new/in-development

- **Software update point installation and configuration**

  Completely reworked guidance to clarify prerequisites, applicability, and installation tracking for software update points. Added end-to-end diagrams, richer log examples (SMSProv, SiteComp, bootstrap, SUP), and practical SQL queries to inspect component properties and subscribed products/classifications. Documented WSUS configuration flows and state values, plus database monitor notifications for deeper troubleshooting insights. The content now focuses on installation/configuration mechanics and monitoring, removing older proxy and WSUS connection account how-to steps.

  https://learn.microsoft.com/en-us/troubleshoot/mem/configmgr/update-management/software-update-point-installation-configuration

- **Track software update synchronization**

  Expanded and reorganized content to explain how ConfigMgr synchronizes update metadata at top-level and child sites. Provides step-by-step flows with log samples, sample SQL, and references to key components and status messages to speed root-cause analysis. Adds prescriptive guidance for WSUS maintenance and clarifies how ConfigMgr handles expired update cleanup in the database with timing, eligibility criteria, and verification hints. Diagram references further illustrate synchronization paths and policy signaling.

  https://learn.microsoft.com/en-us/troubleshoot/mem/configmgr/update-management/track-software-update-synchronization

## Moderate Changes

- **Remediations**

  Added performance recommendations to minimize device impact: target only necessary script packages, avoid resource-heavy scripts, and use less frequent schedules (for example, every 7 days). Guidance also emphasizes writing detection scripts that return stable, actionable results rather than volatile values.

  https://learn.microsoft.com/en-us/intune/device-management/tools/deploy-remediations

- **Planning for Remote Help with Microsoft Intune**

  Clarified licensing for Android Dedicated (COSU) scenarios on supported Zebra and Samsung devices: no Sharer license is needed because no user is signed in. Only the Helper requires a Remote Help license, simplifying cost and planning.

  https://learn.microsoft.com/en-us/intune/remote-help/plan

- **Troubleshoot software update synchronization**

  Reorganized troubleshooting steps with clearer prerequisites and prescriptive WSUS Update Source guidance. Improved directions for authentication, proxy, and connectivity issues with standardized examples, log references (WCM, WSyncMgr, WSUSCtrl), and updated links to current tools and support resources.

  https://learn.microsoft.com/en-us/troubleshoot/mem/configmgr/update-management/troubleshoot-software-update-synchronization