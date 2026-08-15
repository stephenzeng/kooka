# Microsoft Defender for Endpoint
**Date created:** 2026-08-15 UTC  
**Tags:** Configuration, Guidance, Identity, Performance, Security, Troubleshooting  

## Major Changes

- **Migrate servers to Microsoft Defender for Endpoint by using Configuration Manager**

  Overhauled guidance to provide a step-by-step migration path from the MMA-based solution to the unified Microsoft Defender for Endpoint on Windows Server 2012 R2 and 2016 using Configuration Manager. Clarifies version-specific steps (manual for ConfigMgr earlier than 2207, automated options for newer versions) and expands prerequisites and preparation, including required files and scripts. Reworks the application deployment into a Script Installer with parameters to remove MMA and onboard, updates detection using the Sense service registry key, and details deployment workflows. Adds comprehensive verification and troubleshooting instructions, including logs, portal checks, and detection testing.

  https://learn.microsoft.com/en-us/defender-endpoint/application-deployment-via-mecm

- **Behavior monitoring in Microsoft Defender Antivirus**

  Expanded and clarified how behavior monitoring works, its dependent features, and how to configure it across management tools with precedence considerations. Adds concrete PowerShell commands to enable/disable and query status, plus improved Advanced Hunting guidance. Significantly strengthens performance troubleshooting with Performance Analyzer commands, controlled testing using troubleshooting mode, rollback options, cautions on exclusions, and use of the Client Analyzer for escalations.

  https://learn.microsoft.com/en-us/defender-endpoint/behavior-monitor

- **Create a custom gradual rollout process for Microsoft Defender updates**

  Restructures and expands the update rollout guidance with clear prerequisites, supported OS, and minimum platform version requirements. Clarifies management authority best practices and Group Policy settings, including channel options and when to remove conflicting GPOs. Enhances Intune coverage with Settings Catalog options and detailed OMA-URI paths, adds supported PowerShell parameters with examples, and provides verification steps using Get-MpPreference and registry keys. This helps organizations stage platform, engine, and security intelligence updates with greater control and transparency.

  https://learn.microsoft.com/en-us/defender-endpoint/configure-updates

## Moderate Changes

- **Assign Microsoft Defender for Endpoint basic permissions**

  Refocused guidance on assigning basic portal access using Microsoft Graph PowerShell, with clear prerequisites and role/permission requirements. Notes that unified RBAC is required for new customers starting Feb 16, 2025, and maps access levels to Microsoft Entra roles (Security Administrator and Security Reader). Streamlines role assignment with updated cmdlets and recommends using the unified role-assignment API where applicable.

  https://learn.microsoft.com/en-us/defender-endpoint/basic-permissions

- **Set up AI agent runtime protection with Microsoft Defender for Endpoint (Preview)**

  Marks the feature as Preview with expanded prerequisites and clearer enablement guidance, including when to use Audit vs Block and how to disable. Improves Intune deployment instructions using PowerShell scripts in system context, explains script execution behavior, and outlines steps to redeploy updates. Clarifies alert visibility, SOC investigation context, and end-user notification behavior to support phased testing and rollout.

  https://learn.microsoft.com/en-us/defender-endpoint/configure-ai-agent-runtime-protection