# Microsoft Defender for Endpoint
**Date created:** 2026-08-14 UTC  
**Tags:** Configuration, Guidance, Monitoring, Performance, Security  

## Moderate Changes

- **Configure Microsoft Defender Antivirus scanning options**
  
  Updated Group Policy guidance with a clearer, step-by-step workflow in GPMC and tips for using Local Group Policy Editor. Clarifies legacy policy path naming without changing available options or defaults.
  
  https://learn.microsoft.com/en-us/defender-endpoint/configure-advanced-scan-types-microsoft-defender-antivirus

- **Configure the cloud block time out period**
  
  Expanded instructions for configuring the extended cloud check in GPMC, including precise navigation and valid values (1–50 seconds) added to the default 10-second delay. Notes legacy path naming and includes local configuration tips.
  
  https://learn.microsoft.com/en-us/defender-endpoint/configure-cloud-block-time-out-period-microsoft-defender-antivirus

- **Configure Microsoft Defender Antivirus notifications that appear on endpoints**
  
  Revised Group Policy procedures to clearly locate and configure notification policies in GPMC, with explicit effects for disabling enhanced or all notifications and hiding reboot prompts. Adds legacy path notes and local editor tips for consistent configuration.
  
  https://learn.microsoft.com/en-us/defender-endpoint/configure-notifications-microsoft-defender-antivirus

- **Configure remediation for Microsoft Defender Antivirus detections**
  
  Restructured remediation guidance with detailed GPMC navigation and a refined policy table that adds subfolder context and clarifies default behaviors, including threat-level actions. Improves accuracy and setup flow, with notes on legacy naming and local configuration options.
  
  https://learn.microsoft.com/en-us/defender-endpoint/configure-remediation-microsoft-defender-antivirus

- **Detect and block potentially unwanted applications**
  
  Clarified Group Policy steps for enabling PUA protection, including where to find the policy, when to update Administrative Templates, and how to choose Block vs Audit. Adds legacy path notes and local device configuration guidance.
  
  https://learn.microsoft.com/en-us/defender-endpoint/detect-block-potentially-unwanted-apps-microsoft-defender-antivirus

- **Endpoint detection and response in block mode**
  
  Expanded GPMC-based procedure to enable EDR in block mode with precise navigation and multiple ways to open and set the policy. Includes a local Group Policy path for device-level configuration.
  
  https://learn.microsoft.com/en-us/defender-endpoint/edr-in-block-mode

- **Turn on cloud protection in Microsoft Defender Antivirus**
  
  Reworked guidance for enabling MAPS (cloud-delivered protection) in GPMC with separate, detailed steps for joining MAPS and configuring sample submission. PowerShell guidance now uses a single Set-MpPreference command and explains consent values and their protection impact, including Block at First Sight.
  
  https://learn.microsoft.com/en-us/defender-endpoint/enable-cloud-protection-microsoft-defender-antivirus

- **Enable exploit protection**
  
  Clarified how to configure exploit protection via GPMC, including detailed navigation and enabling the common settings policy with XML source options (local, UNC, or URL). Adds legacy path context and local configuration tips.
  
  https://learn.microsoft.com/en-us/defender-endpoint/enable-exploit-protection

- **Manage Microsoft Defender Antivirus updates and scans for endpoints that are out of date**
  
  Expanded procedures for catch-up protection and scans with step-by-step GPMC navigation, clearer behavior descriptions, and separated guidance for spyware vs. virus definition age settings. Clarifies forced catch-up scan behavior, metered connection policy effects, and adds local editor tips.
  
  https://learn.microsoft.com/en-us/defender-endpoint/manage-outdated-endpoints-microsoft-defender-antivirus

- **Schedule Microsoft Defender Antivirus protection updates**
  
  Reorganized Group Policy steps into clear subsections for scheduling day, interval, and time, with defaults explained and time set as minutes after midnight. Adds legacy path notes and tips for local configuration.
  
  https://learn.microsoft.com/en-us/defender-endpoint/manage-protection-update-schedule-microsoft-defender-antivirus

- **Manage the sources for Microsoft Defender Antivirus protection updates**
  
  Rewrote GPMC guidance to configure update source order and file shares, listing valid values and delimiter usage with UNC examples. Clarifies legacy naming differences and provides local editor tips to avoid misconfiguration.
  
  https://learn.microsoft.com/en-us/defender-endpoint/manage-protection-updates-microsoft-defender-antivirus

- **Manage updates for mobile devices and virtual machines (VMs)**
  
  Clarified how to opt in to Microsoft Update and control updates on battery power with explicit GPMC steps and policy actions. Adds legacy path notes and local editor guidance for consistent results on mobile and VM scenarios.
  
  https://learn.microsoft.com/en-us/defender-endpoint/manage-updates-mobile-devices-vms-microsoft-defender-antivirus

- **Configure custom exclusions for Microsoft Defender Antivirus**
  
  Expanded Group Policy setup steps to locate and edit exclusion settings in GPMC with a note on legacy path naming. No changes to exclusion options or behavior.
  
  https://learn.microsoft.com/en-us/defender-endpoint/microsoft-defender-antivirus-exclusions-configure

- **Microsoft Defender Antivirus exclusions on Windows Server**
  
  Clarified the GPMC procedure to disable automatic exclusions by detailing how to find and edit the target GPO. Notes legacy naming differences to avoid path confusion on older Windows versions.
  
  https://learn.microsoft.com/en-us/defender-endpoint/microsoft-defender-antivirus-exclusions-windows-server

- **Microsoft Defender for Endpoint release notes**
  
  Added August 2026 release entries for Android and iOS with performance improvements and bug fixes, and updated Linux from 101.26062.0005 to 101.26062.0007. The Linux section also includes a new note on reliability and quality improvements.
  
  https://learn.microsoft.com/en-us/defender-endpoint/microsoft-defender-endpoint-releases

- **Use network protection to help prevent connections to malicious or suspicious sites**
  
  Improved Group Policy procedures for network protection with exact navigation, methods to open settings, and clearer steps for enabling options like converting warn to block and asynchronous inspection. Emphasizes performance-related configuration choices and includes local editor guidance.
  
  https://learn.microsoft.com/en-us/defender-endpoint/network-protection

- **Specify the cloud protection level**
  
  Refined GPMC instructions to enable and choose a cloud blocking level with updated descriptions of tradeoffs for protection, performance, and false positives. Clarifies RSOP caveats for value 0 and suggests registry or GPResult checks, with local configuration tips.
  
  https://learn.microsoft.com/en-us/defender-endpoint/specify-cloud-protection-level-microsoft-defender-antivirus

- **Use Group Policy settings to configure and manage Microsoft Defender Antivirus**
  
  Expanded configuration steps with precise GPMC navigation and multiple ways to open and edit settings, plus notes on legacy path naming. Adds local editor tips to streamline device-level configuration.
  
  https://learn.microsoft.com/en-us/defender-endpoint/use-group-policy-microsoft-defender-antivirus