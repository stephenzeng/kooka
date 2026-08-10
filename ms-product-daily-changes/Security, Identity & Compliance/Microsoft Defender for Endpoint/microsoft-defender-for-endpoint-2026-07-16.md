# Microsoft Defender for Endpoint
**Date created:** 2026-07-16 UTC  
**Tags:** Administration, Security  

## Moderate Changes

- **Allow Microsoft Defender for Endpoint scripts with WDAC script enforcement**
  Added a planning/prerequisites reference and clarified supported platforms and components required for configuration. Introduced a security warning advising against broad path-based allow rules, user-writable locations, and wide wildcards to help prevent weakened security posture.
  https://learn.microsoft.com/en-us/defender-endpoint/configure-wdac-script-enforcement-mde

- **Attack surface reduction (ASR) rule demonstrations**
  Expanded step-by-step testing guidance, added clear prerequisites, and refined instructions for switching between Block, Audit, and Disabled modes during demos. Clarified Controlled Folder Access considerations, detailed scenario walkthroughs (including USB blocking and ransomware behavior), and improved cleanup steps to restore original settings reliably.
  https://learn.microsoft.com/en-us/defender-endpoint/defender-endpoint-demonstration-attack-surface-reduction-rules

- **Evaluate Microsoft Defender Antivirus and Exploit Guard with Endpoint security policies**
  Expanded scope to include Microsoft Defender Exploit Guard and added prerequisites for supported Windows versions and onboarding. Emphasized the value of cloud-delivered protection for faster threat response, clarified handling of ASR rule blocks, and added guidance on MAPS, connectivity checks, and submitting missed detections.
  https://learn.microsoft.com/en-us/defender-endpoint/evaluate-mda-using-mde-security-settings-management

- **Evaluate Microsoft Defender Antivirus using Group Policy**
  Clarified and streamlined evaluation guidance, including Administrative Templates setup and when to use a Central Store. Enhanced explanations for MAPS, scan and update settings, default remediation behavior, network protection (including Windows Server steps), ASR rules, Controlled Folder Access, tamper protection, connectivity validation, and version checks.
  https://learn.microsoft.com/en-us/defender-endpoint/evaluate-mdav-using-gp

- **Manage Microsoft Defender Antivirus updates and scans for endpoints that are out of date**
  Expanded guidance on configuring catch-up protection updates, reporting thresholds, and catch-up scans, and standardized “Use <tool> to <action>” navigation. Clarified Configuration Manager fallback behavior, detailed PowerShell/WMI parameters (for example, SignatureUpdateCatchupInterval), noted that catch-up scans are enabled by default with instructions to disable, and added an important prerequisite to schedule at least one scan.
  https://learn.microsoft.com/en-us/defender-endpoint/manage-outdated-endpoints-microsoft-defender-antivirus