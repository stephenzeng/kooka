# Microsoft Defender XDR
**Date created:** 2026-08-12 UTC  
**Tags:** Analytics, Best Practices, Configuration, Governance, Guidance, Identity, Security, Troubleshooting  

## Moderate Changes

- **Activate Microsoft Defender unified role-based access control (URBAC)**
  Expanded the deactivation procedure with step-by-step guidance in the Defender portal and clarified that deactivated workloads appear as Not Active. This improves accuracy and reduces errors when turning off specific workloads.

  https://learn.microsoft.com/en-us/defender-xdr/activate-defender-rbac

- **Use Microsoft Sentinel functions, saved queries, and custom rules**
  Added irreversible-deletion warnings for functions and saved queries, and expanded guidance for adx(), arg(), and workspace() operators for cross-service and cross-workspace scenarios. Updated UI descriptions and retitled sections to emphasize creating analytics and custom detection rules, improving safety and task-oriented workflows.

  https://learn.microsoft.com/en-us/defender-xdr/advanced-hunting-defender-use-custom-rules

- **Hunt for ransomware**
  Introduced context on detecting pre-encryption ransomware behaviors with advanced hunting, including a weighted-indicator query for prioritization. Clarified the relevance of taskkill.exe and cipher.exe detections and reorganized content for better comprehension.

  https://learn.microsoft.com/en-us/defender-xdr/advanced-hunting-find-ransomware

- **Protect AI agents in real time using Microsoft Defender**
  Added coverage details for Foundry agents (Preview), specifying evaluation of user requests, agent responses, tool invocations, and tool responses. Updated Copilot Studio coverage to indicate Preview status and clarified evaluation of tool invocations, helping teams understand protection scope.

  https://learn.microsoft.com/en-us/defender-xdr/security-for-ai/ai-agent-real-time-protection

- **Alert classification for password spray attacks**
  Added an advanced hunting query to detect removal of MFA strong authentication requirements, highlighting potential post-compromise tampering. Clarified the purpose of the existing MFA reset/bypass query to improve alert correlation.

  https://learn.microsoft.com/en-us/defender-xdr/alert-classification-password-spray-attack

- **Create dynamic rules for devices in asset rule management**
  Added a warning that deleting a dynamic rule removes it and can affect tag or device value assignments, recommending Turn off to halt application without removal. This helps prevent unintended changes to device classification.

  https://learn.microsoft.com/en-us/defender-xdr/configure-asset-rules

- **Configure automatic attack disruption in Microsoft Defender XDR**
  Added prerequisites for licensing, permissions, and setup, and expanded Sense Agent details including minimum version for Contain User and verification via PowerShell/registry and MsSense DLL version. Clarified Microsoft 365 connector configuration to select all checkboxes, including Microsoft Entra ID apps, to avoid degraded functionality.

  https://learn.microsoft.com/en-us/defender-xdr/configure-attack-disruption

- **Configure email alert notifications in Microsoft Defender XDR**
  Retitled and clarified the article for Defender XDR email notifications, refined steps, and added anchors for easier navigation. Introduced a warning that deleting a notification rule is permanent and stops future alerts, reducing accidental loss of coverage.

  https://learn.microsoft.com/en-us/defender-xdr/configure-email-notifications

- **Investigate data loss prevention alerts with Microsoft Sentinel**
  Added guidance on using the Defender XDR connector to import, correlate, and investigate DLP alerts, with an emphasis on Sentinel’s security orchestration, automation, and response capabilities. Provided steps preceding the KQL example to find a specific alert by SystemAlertId and correlate it with CloudAppEvents over 30 days.

  https://learn.microsoft.com/en-us/defender-xdr/dlp-investigate-alerts-sentinel

- **Edit, delete, and export roles in Microsoft Defender unified role-based access control (RBAC)**
  Rewrote the introduction to detail editing, deleting, and exporting roles and to list required permissions. Expanded delete steps with a warning that removing a role for an active workload strips assigned user permissions, and refined export guidance including the 2025 default model note, CSV contents, multiple assignment rows, and per-workload activation status.

  https://learn.microsoft.com/en-us/defender-xdr/edit-delete-rbac-roles

- **Manage analytics rule correlation settings in Microsoft Defender XDR**
  Clarified Sentinel Contributor role permissions and explicitly named the Incident correlation default setting. Added concrete guidance to override defaults using description tags: #INC_CORR# to include and #DONT_CORR# to exclude specific rules.

  https://learn.microsoft.com/en-us/defender-xdr/exclude-analytics-rules-correlation

- **Manage incidents in Microsoft Defender**
  Added prerequisites stating that incident management requires Defender portal access with an appropriate role assigned through Defender XDR RBAC, with a link to the RBAC documentation. This ensures administrators understand required authorization before proceeding.

  https://learn.microsoft.com/en-us/defender-xdr/manage-incidents

- **Troubleshoot Microsoft Defender XDR service issues**
  Expanded troubleshooting with a prerequisite check, clearer consent setting instructions, improved anchors, and updated step references. Renamed and anchored the app permission reset option, added a warning about removing existing app configuration, and clarified TenantID capture and consent URL parameters to avoid misconfiguration.

  https://learn.microsoft.com/en-us/defender-xdr/troubleshoot