# Microsoft Defender for Endpoint
**Date created:** 2026-07-18 UTC  
**Tags:** Administration, Security  

## New Articles

- **Configure automation folder exclusions**

  Introduced step-by-step guidance to configure automation folder exclusions that affect automated investigation and remediation while leaving antivirus scans unaffected. Clarifies wildcard support, what elements define an exclusion, and where to manage exclusions in the Defender portal. Explains impact on automated actions and live response, scope across onboarded devices, and required permissions via Defender XDR Unified RBAC, legacy RBAC, and Microsoft Entra roles. Provides procedures to add, edit, and remove exclusions, and notes the feature isn’t available for Microsoft Defender for Business.

  https://learn.microsoft.com/en-us/defender-endpoint/automation-folder-exclusions-configure

- **Exclusions to avoid in Microsoft Defender Antivirus and Defender for Endpoint**

  Added a best-practice guide outlining high-risk exclusions to avoid across Windows, macOS, and Linux to prevent attacker abuse. Advises against name-only file exclusions, using a single list across different server workloads, and relying on environment variables that resolve differently under LocalSystem. Includes practical exceptions, workload-specific recommendations, and links to related configuration and validation guidance.

  https://learn.microsoft.com/en-us/defender-endpoint/defender-endpoint-exclusions-common-mistakes

- **Exclusions reference for Microsoft Defender for Endpoint**

  Introduces a comprehensive reference mapping each exclusion type (AV, ASR, CFA, automation folders, per-rule ASR, server role auto-exclusions) to the tools that support configuring them. Highlights support across Intune, Microsoft Defender portal, Configuration Manager, Policy CSP, Group Policy, PowerShell, WMI, and the Windows Security app, including limitations and gaps. Provides direct links to configuration procedures and pointers to Linux and macOS guidance.

  https://learn.microsoft.com/en-us/defender-endpoint/defender-endpoint-exclusions-configuration-reference

- **Overview of exclusions and indicators in Microsoft Defender for Endpoint**

  Provides strategic guidance on when to use exclusions versus allow indicators and how they interact with other protections. Explains cross-platform and Windows-only exclusion types, evaluation order and conflict handling, and how automated investigation and remediation works alongside indicators. Recommends safer alternatives before creating exclusions and links to detailed configuration and troubleshooting resources.

  https://learn.microsoft.com/en-us/defender-endpoint/defender-endpoint-exclusions-overview

- **Manage endpoint security policies in Microsoft Defender for Endpoint**

  Enables creating and managing endpoint security policies directly in the Defender portal, reducing the need to switch to Intune for common scenarios. Details supported policy types per platform, permission models, and step-by-step procedures to create, assign, and edit policies. Covers rollout verification, accelerating deployment via Policy sync, scope tag considerations, and where to view applied policies during investigations.

  https://learn.microsoft.com/en-us/defender-endpoint/endpoint-security-policies-configure

- **Configure custom exclusions for Microsoft Defender Antivirus**

  Adds comprehensive how-to guidance for configuring file/folder, extension, and process exclusions across all major management methods. Includes detailed steps for Intune and the Defender portal, CSP OMA-URI paths, Configuration Manager settings, Group Policy procedures, PowerShell and WMI commands, and Windows Security app limitations. Provides verification and validation tips (MpCmdRun checks and EICAR), and clarifies wildcards, contextual exclusions, and tamper protection behavior.

  https://learn.microsoft.com/en-us/defender-endpoint/microsoft-defender-antivirus-exclusions-configure

- **Exclusions in Microsoft Defender Antivirus**

  Introduces concepts for when to use AV exclusions, their security impact, and how they interact with IOCs, ASR, and network protection. Details built-in and custom exclusion types, contextual exclusions and syntax, wildcard behavior and constraints, and environment variable resolution under LocalSystem. Offers guidance on auditing, precedence and merging of local vs. managed exclusions, and safer alternatives to exclusions.

  https://learn.microsoft.com/en-us/defender-endpoint/microsoft-defender-antivirus-exclusions-overview

- **Configure Microsoft Defender Antivirus on Windows Server**

  Provides end-to-end configuration guidance for Windows Server 2016+ and Azure Stack HCI OS 23H2+. Covers enabling or reinstalling Defender AV, verifying service status, and configuring security intelligence updates. Explains active vs. passive mode when onboarded to Defender for Endpoint, tamper protection considerations, and steps to reactivate Defender AV after removing third-party AV.

  https://learn.microsoft.com/en-us/defender-endpoint/microsoft-defender-antivirus-windows-server-configure

- **Network isolation exclusions in Microsoft Defender for Endpoint**

  Adds guidance to define global network isolation exclusions and apply selective isolation on devices. Details required permissions, supported OS, rule parameters (process path, service name, PFN, direction, remote IP formats/limits), and evaluation logic. Notes API usage for selective isolation and that changes apply to new isolation sessions, with deprecation notes for previously embedded app exclusions.

  https://learn.microsoft.com/en-us/defender-endpoint/network-isolation-exclusions

## Major Changes

- **Take response actions on a device in Microsoft Defender for Endpoint**

  Added a new section covering automatic device isolation within automatic attack disruption, including how to review actions, safeguards, and selective isolation/exclusions. Expanded and clarified procedures for antivirus scans, app restriction, and device isolation, with standardized user notification descriptions and clearer Action center terminology. Updated references for isolation exclusions and improved image accessibility with standardized components.

  https://learn.microsoft.com/en-us/defender-endpoint/respond-machine-alerts

## Moderate Changes

- **Configure attack surface reduction (ASR) rules and exclusions**

  Expanded guidance to configure ASR rules and exclusions directly in the Defender portal using endpoint security policies, mirroring Intune profiles. Clarified assignment group limitations for devices managed via security settings management and aligned recommendations away from Intune-only guidance.

  https://learn.microsoft.com/en-us/defender-endpoint/attack-surface-reduction-rules-configure

- **Attack surface reduction (ASR) rules overview**

  Added the Defender portal as a supported method for configuring ASR rules and per-rule exclusions. Consolidated references for AV exclusions, wildcard usage, and environment variables to a single exclusions overview for consistency.

  https://learn.microsoft.com/en-us/defender-endpoint/attack-surface-reduction-rules-overview

- **Configure controlled folder access (CFA)**

  Introduced Defender portal steps to configure CFA via endpoint security policies, aligning with Intune profile settings. Included notes about assignment group limitations for devices managed through security settings management.

  https://learn.microsoft.com/en-us/defender-endpoint/controlled-folder-access-configure

- **Protect folders from ransomware with controlled folder access**

  Documented configuration and management via the Defender portal with parity to Intune and updated supported modes terminology from “MDM CSP” to “Policy CSP.” Expanded the deployment methods table to include Defender portal configuration.

  https://learn.microsoft.com/en-us/defender-endpoint/controlled-folder-access-overview

- **Microsoft Defender for Endpoint release notes**

  Added Linux July 2026 release details, including versions and feature enhancements like a new antivirus_enforcement_level field and improved connectivity tests. Updated June 2026 Linux release entries to reflect revised engine and signature versions, and noted a fix for installations on FIPS-enabled RHEL 8/9.

  https://learn.microsoft.com/en-us/defender-endpoint/microsoft-defender-endpoint-releases

- **Microsoft Defender Antivirus in the Windows Security app**

  Reworked exclusion instructions with a streamlined flow and explicit option choices. Clarified that process exclusions affect files opened by the process and advised using file or folder exclusions when the process itself must be excluded, with links to a consolidated exclusions overview.

  https://learn.microsoft.com/en-us/defender-endpoint/microsoft-defender-security-center-antivirus

- **Troubleshoot ASR rules**

  Expanded troubleshooting to address false positives/negatives and clarified how to interpret PowerShell output for rule IDs and actions. Advised managing modes via the same deployment channel and provided concrete data collection steps using MDE Client Analyzer or MpCmdRun in verbose mode before opening support cases.

  https://learn.microsoft.com/en-us/defender-endpoint/troubleshoot-asr