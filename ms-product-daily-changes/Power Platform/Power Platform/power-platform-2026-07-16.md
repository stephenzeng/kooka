# Power Platform
**Date created:** 2026-07-16 UTC  
**Tags:** Administration, Governance, Monitoring, Other  

## New Articles

- **Integrate Outlook and SAP with Power Apps**

  Introduced a reference architecture showing how to extend Outlook with a Power Apps canvas app to interact with SAP CRM and SAP S/4HANA via a custom connector fronted by SAP API Management. The guidance details security and identity patterns, responsibility boundaries, throttling, and premium licensing requirements. It also covers reliability, performance, user experience, ALM best practices, observability, and data loss prevention policies. Key design decisions clarify no direct on-premises connectivity, SAP API Management as the boundary, and Office.js for context handoff.

  https://learn.microsoft.com/en-us/power-platform/architecture/reference-architectures/outlook-canvas-app

## Moderate Changes

- **View Microsoft Dataverse and model-driven app activity logs in Microsoft Purview**

  Updated examples to focus on the sequence of messages when converting a lead to an opportunity, removing the prior read-Account example. This streamlines guidance and helps readers better understand end-to-end log interpretation for a common business process.

  https://learn.microsoft.com/en-us/power-platform/admin/activity-logging-auditing/activity-logs-dataverse-model-driven-apps

- **Business continuity and disaster recovery**

  Removed the prerequisite that self-service disaster recovery requires a managed environment linked to a pay-as-you-go billing plan. This broadens eligibility and simplifies setup for organizations implementing self-service disaster recovery.

  https://learn.microsoft.com/en-us/power-platform/admin/business-continuity-disaster-recovery

- **Overview of Power Platform and Copilot Studio reference architectures**

  Added a new entry for integrating Outlook and SAP with Power Apps, expanding the library of vetted solution patterns. This helps architects quickly find implementation guidance for Outlook extensibility with SAP back ends.

  https://learn.microsoft.com/en-us/power-platform/architecture/reference-architectures/

- **OrgDBOrgSettings for server-side synchronization**

  Added the PreserveEmailSenderRecipientParties setting to keep original sender and recipient activity parties on existing emails even if names or addresses change later. This improves auditability and message traceability; it applies only to changes made after the setting is enabled.

  https://learn.microsoft.com/en-us/power-platform/admin/OrgDbOrgSettings

- **Set up virtual network support for Power Platform**

  Noted that initial VNet setup can cause disruptions, including up to 30 minutes of unavailability while connections initialize for the delegated subnet. This helps admins plan maintenance windows and minimize user impact during setup.

  https://learn.microsoft.com/en-us/power-platform/admin/vnet-support-setup-configure