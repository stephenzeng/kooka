# Microsoft 365 Copilot connectors
**Date created:** 2026-08-27 UTC  
**Tags:** Best Practices, Configuration, Deprecation, Guidance, Identity, Performance, Security, Troubleshooting  

## Major Changes

- **Set up the ServiceNow service for ServiceNow Catalog connector ingestion**

  Introduced the GetAllUserCriteriaV2 scripted REST API resource that evaluates only item-level user criteria and supports evaluating multiple users per request. Added full setup instructions and included this step in prerequisites to streamline configuration. Marked the older GetAllUserCriteria as scheduled for deprecation and clarified selection behavior when both resources exist. These changes reduce API calls and speed up the first full identity crawl.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/servicenow-catalog-admin-setup

- **Set up the ServiceNow service for ServiceNow Knowledge connector ingestion**

  Added a new Advanced flow REST API resource (user_changes) to enable incremental identity synchronization, with complete implementation, parameters, response format, ACLs, and verification steps. Introduced auditing and permission prerequisites, including access to sys_audit and sys_audit_delete and guidance to enable auditing for specific tables/fields. Removed the preview label from the API that evaluates only article-level user criteria. These updates keep identities current between full crawls and improve governance.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/servicenow-knowledge-admin-setup

## Moderate Changes

- **Search and validate indexed connector content**

  Removed support for using ServiceNow knowledge article sys_id as a valid identifier in search validation. The table now lists only Article number and Knowledge base sys_id, and instructions for copying article sys_id were removed to prevent misidentification and improve accuracy.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/indexed-content

- **Deploy the ServiceNow Catalog connector**

  You can now customize the AccessURL for both new and existing connections, eliminating the need to recreate connections. This simplifies URL management and reduces administrative overhead.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/servicenow-catalog-deployment

- **Troubleshoot issues with the ServiceNow Catalog connector**

  Added GCC High IP ranges for USGov regions to the firewall allowlist to ensure connectivity in sovereign clouds. Clarified that AccessURL can be customized for both new and existing connections to streamline URL updates.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/servicenow-catalog-troubleshooting

- **Deploy the ServiceNow Knowledge Copilot connector**

  Clarified permission evaluation: Simple flow may mis-handle advanced script-based user criteria and can overshare, so Advanced flow with the REST API is recommended. Introduced an incremental identity sync crawl for Advanced flow to keep identities updated between full crawls and clarified that standard incremental crawls don’t update identities. Also enabled AccessURL customization on both new and existing connections to ease administration.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/servicenow-knowledge-deployment

- **ServiceNow Knowledge Copilot connector overview**

  Updated capabilities to support incremental identity sync for Advanced flow, keeping users, groups, roles, and user criteria current between full crawls, and noted that only attachments visible to users are indexed. Increased the maximum combined attachment size per article from 20 MB to 64 MB to accommodate richer content.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/servicenow-knowledge-overview

- **Troubleshoot issues with the ServiceNow Knowledge connector**

  Added GCC High IP ranges for USGov regions to the allowlist to improve connectivity in sovereign environments. Clarified that AccessURL customization is supported for both new and existing connections.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/servicenow-knowledge-troubleshooting

- **Deploy the ServiceNow Tickets Copilot connector**

  Enabled AccessURL customization for both new and existing connections to avoid recreating connections for URL changes. Clarified that preview access permissions aren’t enforced until deployment, helping admins plan testing and rollout.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/servicenow-tickets-deployment

- **Troubleshoot issues with the ServiceNow Tickets connector**

  Added GCC High egress IP ranges for USGov regions to the firewall table to support sovereign connectivity. Also confirmed that AccessURL can be customized for existing connections without recreation.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/servicenow-tickets-troubleshooting