# Microsoft Defender for Endpoint
**Date created:** 2026-08-23 UTC  
**Tags:** Best Practices, Configuration, Guidance, Performance, Security  

## Major Changes

- **Configure Microsoft Defender Antivirus using Microsoft Intune**

  Comprehensive rewrite that aligns configuration with the Endpoint Security Antivirus workflow in Intune, with clearer steps for policy type, platform, profiles, scope, and assignments. Clarified supported platforms (Windows enrolled in Intune and Windows Server via Defender for Endpoint security settings management), added Windows 10 end-of-support and licensing notes, and corrected CSP names and default values across key settings. Expanded guidance covers cloud-delivered protection, quarantine retention (now 90 days by default), update channels, network protection options, randomization behaviors, and telemetry controls, helping admins deploy consistent and secure baselines. Performance recommendations were streamlined, including a tip to use Performance analyzer for tuning.

  https://learn.microsoft.com/en-us/defender-endpoint/use-intune-config-manager-microsoft-defender-antivirus

## Moderate Changes

- **Manage Microsoft Defender Antivirus updates and scans for endpoints that are out of date**

  Clarified PowerShell guidance for catch-up scans: both full and quick catch-up scans are disabled by default, and admins should set the related parameters to $false to enable catch-up behavior. This prevents misconfiguration and ensures missed scans run as intended.

  https://learn.microsoft.com/en-us/defender-endpoint/manage-outdated-endpoints-microsoft-defender-antivirus

- **Microsoft Defender Antivirus compatibility with other security products**

  Updated policy guidance to recommend enabling “Turn on catch-up quick scan,” which runs a catch-up quick scan (every 30 days by default) when scheduled scans are missed. Notes about Windows Task Scheduler behavior remain unchanged to avoid conflicts.

  https://learn.microsoft.com/en-us/defender-endpoint/microsoft-defender-antivirus-compatibility

- **Schedule antivirus scans using Microsoft Intune**

  Expanded and reorganized the scan scheduling guidance with step-by-step configuration, valid parameter ranges, and concrete time/day examples for daily and weekly scans. Added recommendations on signature checks before scans, randomization windows, CPU load settings, and catch-up defaults, emphasizing quick scans with real-time and cloud protection for balanced performance.

  https://learn.microsoft.com/en-us/defender-endpoint/schedule-antivirus-scans-intune

- **Schedule antivirus scans using PowerShell**

  Updated the default for DisableCatchupQuickScan to $true, indicating missed quick scans do not run by default. Guidance clarifies how to flip the setting to ensure catch-up behavior when needed.

  https://learn.microsoft.com/en-us/defender-endpoint/schedule-antivirus-scans-powershell