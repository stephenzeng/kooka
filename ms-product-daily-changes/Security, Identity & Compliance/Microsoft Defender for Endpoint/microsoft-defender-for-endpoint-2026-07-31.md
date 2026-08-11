# Microsoft Defender for Endpoint
**Date created:** 2026-07-31 UTC  
**Tags:** AI, Analytics, Monitoring, Security  

## New Articles

- **Controlled configuration in Microsoft Defender for Endpoint**

  Introduced a new concept that makes cloud-managed policy via Intune or Defender for Endpoint the single source of truth for Microsoft Defender Antivirus, overriding Group Policy, scripts, Configuration Manager, and local changes to prevent configuration drift. The article explains how controlled configuration differs from tamper protection, outlines prerequisites and supported scenarios, and describes enforcement behaviors such as value-based conflict resolution and local admin merge. It provides enablement steps in Intune and Defender for Endpoint, reporting and device-level verification guidance, lifecycle behaviors, and troubleshooting with MpCmdRun.exe. It also adds operational guidance on minimum client versions and rollback, and adjusts the minimum Defender Antivirus platform requirement to 4.18.26060.3004.

  https://learn.microsoft.com/en-us/defender-endpoint/secure-controlled-configuration

## Major Changes

- **Discover local AI agents with Microsoft Defender for Endpoint (Preview)**

  Expanded discovery from Windows-only to include macOS and clarified licensing: discovery requires Microsoft Defender for Endpoint Plan 2, while risk indicators and security recommendations require higher-tier licenses. The inventory experience was significantly enriched with detailed columns, agent detail panes, attack surface visualizations, and prerequisite guidance for Defender Antivirus and onboarding. Advanced hunting content was overhauled with new tables (AgentsInfo, ExposureGraphNodes, ExposureGraphEdges), joins via AgentId/NodeId, and end-to-end KQL examples for inventories, MCP servers, risky configurations, and user/asset exposure analysis.

  https://learn.microsoft.com/en-us/defender-endpoint/discover-local-ai-agents

## Moderate Changes

- **Configure attack surface reduction (ASR) rules and exclusions**

  Added comprehensive guidance on resolving policy conflicts across local settings, Group Policy, MDM (Intune), and Configuration Manager, including explicit precedence rules. Documented how to use the MDMWinsOverGP ControlPolicyConflict setting with its OMA-URI and values, and clarified that controlled configuration enforces Intune or MDE settings over conflicting GPO or local changes; wording and references were updated for consistency.

  https://learn.microsoft.com/en-us/defender-endpoint/attack-surface-reduction-rules-configure

- **Attack surface reduction (ASR) rules overview**

  Clarified that Group Policy takes precedence by default for ASR rules and described how to shift precedence using the MDMWinsOverGP Policy CSP or avoid conflicts with controlled configuration. Removed a conflicting internal note and added references to the conflict-handling guidance.

  https://learn.microsoft.com/en-us/defender-endpoint/attack-surface-reduction-rules-overview

- **Protect security settings with tamper protection**

  Introduced “controlled configuration” as the updated management setting name for tamper protection while confirming no change in core functionality. Clarified that it must be explicitly enabled via Intune or Defender for Endpoint security settings management and added a related link to the controlled configuration article.

  https://learn.microsoft.com/en-us/defender-endpoint/prevent-changes-to-security-settings-with-tamper-protection