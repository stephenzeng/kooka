# Microsoft 365 Copilot connectors
**Date created:** 2026-07-24 UTC  
**Tags:** Administration, Agent, AI, Analytics, Programming, Security  

## New Articles

- **Deploy the Azure Data Lake Storage Gen2 connector**

  Introduced a step-by-step deployment guide covering setup in the Microsoft 365 admin center, including naming, connection string entry, and authentication via AccountKey or service principal with required roles. Documented optional queue-based notifications, connection testing prerequisites, staged rollout, and default indexing behavior for users, scope, and sync cadence. Added guidance for configuring permissions (Everyone vs ACL-trimmed for ADLS Gen2), identity mapping to Microsoft Entra ID, schema/property management, and adjustable incremental/full crawl intervals. Linked to related overview, troubleshooting, and general deployment guidance to streamline admin onboarding.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/azure-data-lake-storage-gen2-deployment

- **Azure Data Lake Storage Gen2 connector overview**

  New overview explains how the connector indexes content from Azure Blob Storage and ADLS Gen2 for use in Copilot and Microsoft Search, with benefits, use cases, and example prompt scenarios. It outlines key capabilities (natural language queries, supported file types, ACL-based trimming for ADLS Gen2, scheduling, and optional queue notifications) and important limitations (file sizes, unsupported binaries, reconfiguration constraints, ACL requirements, and image-only Office files). The article clarifies permission models—ACL-trimmed results for ADLS Gen2 and organization-wide visibility for Blob Storage—and lists the types of data indexed across Office, PDF, text, and HTML. A “next steps” link directs admins to deployment guidance.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/azure-data-lake-storage-gen2-overview

## Major Changes

- **Set up the ServiceNow service for ServiceNow Knowledge connector ingestion**

  Added a preview integration for the GetAllUserCriteriaV2 REST API that evaluates only article user criteria and supports batching multiple users per request, reducing API calls and first full identity crawl time. The setup now includes ACL creation, scripted REST API configuration, a POST /user_criteria_v2 resource with full JavaScript handler code, authentication/ACL requirements, endpoint verification, and request schema details. The deployment checklist was updated to reference the new V2 flow, and the prior GetAllUserCriteria API is marked for planned deprecation with guidance to adopt V2 where applicable.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/servicenow-knowledge-admin-setup

## Moderate Changes

- **Troubleshoot issues with the Azure Data Lake Storage Gen2 connector**

  Renamed the troubleshooting article for clarity and added guidance for Test Connection failures. Admins are advised to ensure the storage account has at least one container with at least one file to prevent connection errors.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/azure-data-lake-storage-gen2-troubleshooting

- **Microsoft Graph connector agent**

  Updated prerequisites to require .NET Desktop Runtime 10.0 (x64). Revised network requirements by removing Service Bus endpoints and updating allowlist domains/URLs for Microsoft 365 Enterprise, GCC, and GCCH environments.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/connector-agent

- **Release history for Microsoft Graph connector agent**

  Added release notes for Version 4.0.0.0 introducing .NET 10 support, GCA statistics, and performance improvements for Confluence user info processing and the Intranet connector. The update improves delete detection reliability, fixes DOCX parsing with embedded Visio, surfaces actionable access-denied error E1037, and includes security, bug, and reliability enhancements.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/connector-agent-releases

- **GitHub Cloud Issues connector overview**

  Documented a limitation that access granted exclusively via GitHub secret teams isn’t supported. To ensure visibility of issues in Copilot and Microsoft Search, grant access through a visible team or add users as explicit collaborators.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/github-cloud-issues-overview

- **GitHub Cloud Knowledge connector overview**

  Added a limitation clarifying that secret teams aren’t supported for access evaluation. Use visible teams or explicit collaborator assignments so users can see relevant content in Copilot and search.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/github-cloud-knowledge-overview

- **GitHub Cloud Pull Requests connector overview**

  Noted that access granted only via secret teams isn’t supported. Ensure users are members of visible teams or are explicit collaborators so pull requests appear in Copilot and search results.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/github-cloud-pull-requests-overview

- **GitHub Server Issues connector overview**

  Clarified that secret teams aren’t supported for access checks. Use visible teams or explicit collaborator assignments to make issues discoverable in Copilot and Microsoft Search.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/github-server-issues-overview

- **GitHub Server Knowledge connector overview**

  Added a permissions limitation indicating secret teams aren’t supported. Grant access via visible teams or explicit collaborators to ensure content is available in Copilot and search.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/github-server-knowledge-overview

- **GitHub Server Pull Requests connector overview**

  Documented that secret teams aren’t supported for access evaluation. Use visible teams or explicit collaborator assignments so pull requests appear in Copilot and search.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/github-server-pull-requests-overview

- **Deploy the PagerDuty Incidents connector**

  Added a new prerequisite permission for Custom Fields – Read Access and introduced instructions for adding custom properties. During setup, admins can discover incident-type custom fields and include selected fields in the connector schema under Manage properties.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/pagerduty-incidents-deployment

- **Set up the Salesforce service for Salesforce CRM connector ingestion**

  Expanded guidance on enabling API access, including choosing between the System Administrator profile and a custom profile. Added detailed steps for required Administrative and Standard Object permissions, and clarified supported objects (Accounts, Cases, Contacts, Leads, Opportunities) with necessary Read and View All permissions.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/salesforce-crm-admin-setup