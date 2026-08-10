# Microsoft Purview
**Date created:** 2026-07-18 UTC  
**Tags:** Administration, AI, Governance, Monitoring, Security  

## New Articles

- **Configure default protection for classification failures in DLP for Exchange**
  
  Introduced guidance to enable classification failure detection for Exchange Online DLP via the Purview portal and PowerShell (Set-PolicyConfig with DlpErrorHandlingConfig). Explained how attachment conditions behave when detection is enabled, covering timeouts, throttling, and other error scenarios to reduce unintended data leakage. Recommended using DocumentScanFailures with existing conditions using AND to precisely target failure cases. Provided rule-ordering best practices so content detection runs before scan-failure rules, with a prioritized example to avoid false positives. Included links to related DLP articles for deeper implementation detail.
  
  https://learn.microsoft.com/en-us/purview/dlp-exchange-classification-failure-protection

## Major Changes

- **Audit log activities**
  
  Added a new Dragon Copilot Web activities section with dedicated record types (DragonCopilotAccess, DragonCopilotClinicalData, DragonCopilotSession) and detailed event tables spanning access, clinical data, session lifecycle, prompts, and AI-generated content. Expanded Microsoft Fabric audit coverage with Copilot session lifecycle events and message logging, plus new admin connection operations for gateway data sources. These additions broaden visibility into AI- and Fabric-related operations, improving compliance reporting, investigations, and operational monitoring.
  
  https://learn.microsoft.com/en-us/purview/audit-log-activities

## Moderate Changes

- **Audit logs for Copilot and AI applications**
  
  Expanded audit coverage to include Cowork in addition to Copilot and other AI apps. Added DLPEvaluationDeferred and DLPEvaluationDeferredReason properties, and clarified Operation and RecordType descriptions for Copilot, connected, and third‑party AI scenarios. These updates improve clarity and depth of auditing so analysts can better track DLP deferrals and interpret activity types across AI integrations.
  
  https://learn.microsoft.com/en-us/purview/audit-copilot

- **Learn about using Microsoft Purview Data Loss Prevention to protect interactions with Microsoft 365 Copilot and Copilot Chat**
  
  Updated DLP guidance to remove references to prebuilt agents and adjusted availability labels (for example, removing “generally available” where not applicable). Clarified feature scope and preview status to help admins plan policies based on current capabilities and support boundaries.
  
  https://learn.microsoft.com/en-us/purview/dlp-microsoft365-copilot-location-learn-about

- **Learn about DLP file quarantine for SharePoint and OneDrive**
  
  Refreshed Known limitations by removing the public preview label and the prior file name collision constraint. Added a new limit of up to 200,000 items processed per tenant within 24 hours, helping admins anticipate scale boundaries and tune policies accordingly.
  
  https://learn.microsoft.com/en-us/purview/dlp-spo-odb-quarantine-learn

- **Create data quality rules**
  
  Added a prerequisite note for API usage: asset metadata must exist before creating rules. Provided a concise workflow—create asset metadata, verify registration, then create and associate the rule—so users avoid API errors and streamline setup.
  
  https://learn.microsoft.com/en-us/purview/unified-catalog-data-quality-rules