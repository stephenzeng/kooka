# Microsoft Defender for Endpoint
**Date created:** 2026-09-02 UTC  
**Tags:** Configuration, Get Started, Guidance, Monitoring, Security, Troubleshooting  

## New Articles

- **Tamper protection in audit mode for Microsoft Defender for Endpoint on Linux (Preview)**
  
  Introduced preview documentation for tamper protection in audit mode on Linux, detailing what activities are monitored and how alerts surface in the portal and Advanced Hunting. Outlines prerequisites, supported kernels and distributions, and connectivity requirements, including eBPF/BTF considerations and an Ubuntu kernel exception. Explains default enablement during preview, staged rollout behavior, and how to verify and troubleshoot status with mdatp health and configuration checks. Provides sample Kusto queries, a safe test scenario to generate alerts, and guidance to tune noise from legitimate activity.
  
  https://learn.microsoft.com/en-us/defender-endpoint/linux-tamper-protection-audit-mode

## Major Changes

- **Configure block at first sight in Microsoft Defender Antivirus**
  
  Expanded and reorganized guidance to cover end-to-end configuration across Intune, Microsoft Defender portal, Configuration Manager, Group Policy, PowerShell, and the Windows Security app. Clarifies prerequisites and how the feature works, adds verification steps, and highlights risks of reduced protection when disabled. Improves admin tips, section structure, and references for customizing user messaging to streamline deployments.
  
  https://learn.microsoft.com/en-us/defender-endpoint/configure-block-at-first-sight-microsoft-defender-antivirus

- **Configure Microsoft Defender Antivirus always-on protection**
  
  Broadened configuration paths to include the Microsoft Defender portal and Configuration Manager, alongside refined Intune guidance. Details specific settings to enable real-time monitoring, on-access protection, bi-directional scanning, and behavior monitoring, plus PowerShell examples to set and verify policies. Adds Windows Security app steps and notes Configuration Manager prerequisites to reduce setup friction and ensure consistent protection.
  
  https://learn.microsoft.com/en-us/defender-endpoint/configure-real-time-protection-microsoft-defender-antivirus

- **Configure remediation for Microsoft Defender Antivirus detections**
  
  Substantially reworked remediation guidance with clearer policy scoping and step-by-step settings across Intune and the Microsoft Defender portal. Enhances Configuration Manager instructions for Default Actions and Threat Overrides, including cautions when allowing items. Refocuses automation on PowerShell with practical examples for default actions, threat-specific overrides, retention settings, and restore point creation to standardize response workflows.
  
  https://learn.microsoft.com/en-us/defender-endpoint/configure-remediation-microsoft-defender-antivirus

- **Microsoft Defender for Endpoint plug-in for Windows Subsystem for Linux (WSL)**
  
  Added support information for WSL containers (WSLc) in Public Preview, including enrollment steps and WSLc-specific prerequisites. Clarifies installer differences between WSL 2 and WSLc, adds guidance for installing WSL preview builds, and updates health checks to validate active WSLc VMs and Defender status. Notes parity in investigation and Advanced Hunting while calling out distro-specific detection nuances and providing WSLc troubleshooting references.
  
  https://learn.microsoft.com/en-us/defender-endpoint/mde-plugin-wsl

## Moderate Changes

- **Configure the Microsoft Defender Antivirus cloud block time-out period**
  
  Added Configuration Manager as a supported path for setting the cloud block time-out on Windows Server and documented the steps to enable extended cloud checks. Streamlined Intune and Defender portal guidance by consolidating policy creation/editing and clarifying where to configure value ranges for the Cloud Extended Timeout setting.
  
  https://learn.microsoft.com/en-us/defender-endpoint/configure-cloud-block-time-out-period-microsoft-defender-antivirus

- **Configure local overrides for Microsoft Defender Antivirus settings**
  
  Clarifies that Group Policy is the supported method for defining local overrides and adds a dedicated procedure. Expands instructions for merging or disabling local/global lists via Intune and the Defender portal, and specifies supported local change methods, with refined steps and anchors for easier navigation.
  
  https://learn.microsoft.com/en-us/defender-endpoint/configure-local-policy-overrides-microsoft-defender-antivirus

- **Configure controlled folder access (CFA)**
  
  Improves setup guidance for Intune and the Defender portal, specifying exact policy locations, platform/profile selections, and where to configure CFA options. Refines instructions for managing protected folders and allowed apps, including CSV formatting tips, and reiterates assignment constraints for devices managed via security settings management.
  
  https://learn.microsoft.com/en-us/defender-endpoint/controlled-folder-access-configure

- **New features in Microsoft Defender for Endpoint**
  
  Updated the What's New page with two preview entries: tamper protection in audit mode for Linux and the Defender plug-in’s support for WSL containers (WSLc). Highlights new visibility across alerts, device timeline, and Advanced Hunting, and provides version availability and public preview enrollment details.
  
  https://learn.microsoft.com/en-us/defender-endpoint/whats-new-in-microsoft-defender-endpoint