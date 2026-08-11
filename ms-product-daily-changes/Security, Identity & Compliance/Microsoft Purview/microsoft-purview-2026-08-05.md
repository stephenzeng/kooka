# Microsoft Purview
**Date created:** 2026-08-05 UTC  
**Tags:** Administration, Agent, Governance, Monitoring, Security  

## Major Changes

- **Use Microsoft Purview to manage data security & compliance for Anthropic Claude (Enterprise)**
  
  Expanded capability coverage for Claude Enterprise by marking Data classification as supported and enabling support for Insider Risk Management, Communication Compliance, eDiscovery, Data Lifecycle Management, and Compliance Manager. This update broadens governance and compliance controls available for Claude Enterprise workloads. Organizations can now classify data, manage lifecycle and risk, and run compliance assessments through Purview-integrated features, strengthening overall security and audit readiness.
  
  https://learn.microsoft.com/en-us/purview/ai-claude-enterprise

## Moderate Changes

- **Audit log activities**
  
  Added a section detailing Purview permission activities captured in the Microsoft 365 audit log, including create, update, and delete operations for RBAC role groups and user assignments. This improves visibility into administrative changes and supports investigations and compliance reporting.
  
  https://learn.microsoft.com/en-us/purview/audit-log-activities

- **Data loss prevention policy tip reference for Outlook for Microsoft 365**
  
  Clarified that Outlook Classic requires either Microsoft 365 E5 or a license with the Information Protection for Office 365 – Premium service plan to enable DLP Policy Tips. This helps admins ensure the right licensing is in place so policy tips function as expected.
  
  https://learn.microsoft.com/en-us/purview/dlp-ol365-win32-policy-tips

- **Monitoring agents in Insider Risk Management**
  
  Noted a limitation that admin units aren’t supported for agent alerts, preventing scoped analysts from viewing agent-related alerts. This sets expectations for access scoping and helps plan monitoring workflows accordingly.
  
  https://learn.microsoft.com/en-us/purview/insider-risk-management-monitoring-agents

- **Overview of data quality in Microsoft Purview Unified Catalog**
  
  Clarified that Data Quality is supported only when the Purview account and data sources are in Purview-supported regions and located in the same Azure region. This guidance helps ensure compliant deployments and avoids unsupported configurations.
  
  https://learn.microsoft.com/en-us/purview/unified-catalog-data-quality