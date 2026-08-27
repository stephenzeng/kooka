# Microsoft Purview
**Date created:** 2026-08-27 UTC  
**Tags:** Compliance, Configuration, Governance, Guidance, Monitoring, Security  

## Moderate Changes

- **Audit logs for Copilot and AI applications**

  Updated guidance on how audit logs capture model attribution for Microsoft Copilot and Copilot Chat, including when provider and model names are recorded for explicit selections (with examples). Clarified that Auto selection and some internal models may not expose provider/model details, and that Cowork currently omits provider information. This helps administrators interpret model-related signals and understand gaps in audit records.

  https://learn.microsoft.com/en-us/purview/audit-copilot

- **Audit log activities**

  Added two Microsoft Fabric audit activities for OneLake soft delete: reading settings (GetFileSoftDelete) and modifying settings/retention (ModifiedOneLakeFileSoftDeleteSettings, 1–365 days). This expands visibility and governance over data retention controls in OneLake.

  https://learn.microsoft.com/en-us/purview/audit-log-activities

- **Microsoft Purview Endpoint DLP changes in macOS 27 overview (preview)**

  Clarified the macOS 27 shift from Accessibility to Device Control and Data Access permissions and the impact of reduced browser/URL context on protections; requires Endpoint DLP client version 101.26072 or later. Updated behavior details, configuration mapping with explicit setting names and keys, sample snippets (including notifications), and monitoring guidance for device status in the Purview portal. A streamlined readiness checklist helps admins plan and validate their rollout.

  https://learn.microsoft.com/en-us/purview/endpoint-dlp-macos-27-changes