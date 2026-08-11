# Microsoft Purview
**Date created:** 2026-07-31 UTC  
**Tags:** Governance, Security  

## Moderate Changes

- **Audit log activities**

  Added a new audit event, Applied AI guardrail (AIGuardrail), to the Agent 365 activities to record when guardrails are applied to AI agent requests or responses. This enables better monitoring, compliance reporting, and investigations for AI safety and policy enforcement.

  https://learn.microsoft.com/en-us/purview/audit-log-activities

- **Permissions in the Microsoft Purview portal**

  Added a Temporary permissions section describing expiring role group assignments with auto-revoke on expiration, configurable per user, minimum and maximum durations, independent evaluation for multiple assignments, and UI updates to set or edit expirations. Noted exceptions for eDiscovery Administrator and eDiscovery Manager, and clarified that My Permissions shows the latest expiration without pre-expiry notifications—helping admins grant time-bound access while reducing standing privileges.

  https://learn.microsoft.com/en-us/purview/purview-permissions