# Microsoft Defender for Endpoint
**Date created:** 2026-09-04 UTC  
**Tags:** Best Practices, Configuration, Guidance, Monitoring, Performance, Security  

## Major Changes

- **Evaluate Microsoft Defender Antivirus with security policies**

  Restructured the evaluation guidance to center on configuring Microsoft Defender Antivirus via endpoint security policies in the Defender portal, with a new prerequisites section. Configuration guidance is now organized into Antivirus settings, ASR rules, and Tamper Protection, with ASR recommendations shifted to Audit first and clear steps to review events and use per‑rule exclusions before enabling Block. Network protection guidance clarifies keeping Datagram Processing disabled by default on Windows Server due to performance considerations. Tamper Protection setup is streamlined using a Windows Security Experience policy, and validation steps now focus on cloud connectivity and checking platform, security intelligence, and engine versions via PowerShell. Older wizard-based steps and Exploit Guard emphasis were removed in favor of higher-level workflows and updated instructions for submitting missed detections.

  https://learn.microsoft.com/en-us/defender-endpoint/evaluate-mda-using-mde-security-settings-management

- **Configure security settings in Microsoft Defender for Endpoint on Linux**

  Introduced a preview “Memory scan” capability with details on behavior, dependencies on Behavior Monitoring and Antivirus enforcement level, configuration key (MemoryScan), values, and portal mappings. Availability is specified for version 101.26071.0005 or later in the Insiders‑slow channel. The Antivirus enforcement level table was also updated to mark “Audit” as Preview, helping admins plan staged rollouts.

  https://learn.microsoft.com/en-us/defender-endpoint/linux-preferences

## Moderate Changes

- **Microsoft Defender Antivirus compatibility with other security products**

  Expanded compatibility guidance to incorporate Smart App Control (SAC) and reordered the table to reflect SAC status before Defender Antivirus state. Documented a new Hybrid mode when SAC is On and the device is not onboarded, clarified Passive and Disabled modes for non‑Microsoft AV scenarios, and updated the SAC note to emphasize it as a Windows 11 feature that blocks malicious or untrusted apps.

  https://learn.microsoft.com/en-us/defender-endpoint/microsoft-defender-antivirus-compatibility

- **Microsoft Defender for Endpoint release notes**

  Added Windows Antivirus August 2026 with details for Platform 4.18.26080.3 / Engine 1.1.26080.3 and related support phases. Highlights include health monitoring for Cisco Umbrella and Network Protection impacts, hardening to prevent credential exposure, fixes for BitLocker state detection, stalled platform updates, excessive disk I/O from cleanup failures with whitespace paths, AMSI path exclusion handling for memory scans, and proper admin prompts for ASR warn unblock.

  https://learn.microsoft.com/en-us/defender-endpoint/microsoft-defender-endpoint-releases

- **Onboard servers through Microsoft Defender for Endpoint's onboarding experience**

  Added guidance recommending onboarding servers via Defender for Servers Plan 2 in Defender for Cloud, outlining benefits such as agentless scanning, FIM, JIT access, regulatory compliance, premium Defender Vulnerability Management, OS configuration assessments, and 500‑MB/day data ingestion. Clarified that Defender for Cloud auto‑onboards the Defender for Endpoint extension to supported Azure VMs and Azure Arc‑enabled machines, reducing per‑machine scripting, with notes on standalone and Defender for Business server options.

  https://learn.microsoft.com/en-us/defender-endpoint/onboard-server

- **New features in Microsoft Defender for Endpoint**

  Added a preview entry for “Memory scan for Linux” with availability in version 101.26071.0005 or later (Insiders‑slow). Updated “Tamper protection in audit mode for Linux” to specify availability in the Insiders‑slow channel.

  https://learn.microsoft.com/en-us/defender-endpoint/whats-new-in-microsoft-defender-endpoint