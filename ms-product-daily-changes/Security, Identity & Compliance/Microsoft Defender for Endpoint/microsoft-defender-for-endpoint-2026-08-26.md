# Microsoft Defender for Endpoint
**Date created:** 2026-08-26 UTC  
**Tags:** Automation, Best Practices, Configuration, Guidance, Monitoring, Security, Troubleshooting  

## Major Changes

- **Onboard Windows devices to Microsoft Defender for Endpoint by using Microsoft Intune**

  Overhauled and expanded guidance to cover both onboarding and offboarding for Windows 10 and Windows 11, with clearer end-to-end steps via the Intune–Defender integration workflow. Strengthened prerequisites, including Intune enrollment, required roles for EDR policies, and licensing notes clarifying Intune is a separate subscription. Updated CSP references and clarified OMA-URI support; noted the Intune EDR setting for diagnostic data reporting frequency is deprecated and that onboarding enables Endpoint DLP. Rewrote offboarding with precise Defender portal navigation, improved package handling, and two Intune deployment options (custom OMA-URI and EDR policy), plus an important note on data flow impact, retention up to 180 days, and device inventory behavior.

  https://learn.microsoft.com/en-us/defender-endpoint/configure-endpoints-mdm

## Moderate Changes

- **Enable and configure Microsoft Defender Antivirus always-on protection**

  Streamlined Windows guidance by consolidating Intune steps with explicit real-time, on-access, bi-directional scan, behavior monitoring, and heuristics settings, and by revising Group Policy instructions to use centralized GPMC with required policies and a dedicated heuristics section. Clarified tamper protection usage—troubleshooting mode for temporary changes, policy for permanent—and removed macOS-specific Intune creation steps to reduce confusion.

  https://learn.microsoft.com/en-us/defender-endpoint/configure-real-time-protection-microsoft-defender-antivirus

- **Evaluate Microsoft Defender Antivirus**

  Removed the downloadable PDF and associated note, directing readers to use the PowerShell script to automatically enable evaluation settings. This simplifies the evaluation path and keeps the procedure up to date.

  https://learn.microsoft.com/en-us/defender-endpoint/evaluate-microsoft-defender-antivirus

- **Configure security settings in Microsoft Defender for Endpoint on Linux**

  Replaced the prior antivirusEngine table with a single enforcementLevel string and added a new Audit mode to evaluate protection without enforcement. Updated verification to use antivirus_enforcement_level and clarified defaults, version availability for Audit mode, and the recommendation to run a full scan before enabling real-time protection.

  https://learn.microsoft.com/en-us/defender-endpoint/linux-preferences

- **Microsoft Defender for Endpoint release notes**

  Added a new Android release (platform 1.0.9212.0102, Aug 20, 2026) with details and improvements. The Malware Protection card now shows the most recent scan time, helping admins quickly verify device protection status.

  https://learn.microsoft.com/en-us/defender-endpoint/microsoft-defender-endpoint-releases

- **New features in Microsoft Defender for Endpoint**

  Added two Linux updates: Antivirus audit mode (Preview) for real-time detection and alerting without enforcement, and Offboarding API support (GA) to automate device lifecycle management. Both features are available on Microsoft Defender for Endpoint on Linux version 101.26062.0007 or later.

  https://learn.microsoft.com/en-us/defender-endpoint/whats-new-in-microsoft-defender-endpoint