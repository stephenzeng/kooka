# Microsoft 365 Copilot connectors
**Date created:** 2026-08-22 UTC  
**Tags:** Configuration, Get Started, Governance, Guidance, Identity, Security, Troubleshooting  

## New Articles

- **Set up the Azure DevOps service for Azure DevOps Wiki connector ingestion**
  Introduced a dedicated admin setup guide for preparing Azure DevOps to ingest Wiki content with the Microsoft 365 Copilot connector. It provides a setup checklist, prerequisites, and recommended authentication (Federated Credential) alongside Microsoft Entra ID OAuth as an alternative. The article details required Azure DevOps permissions and the crawl account role, helping admins configure access correctly before deployment. A next-step link directs readers to the deployment guide for rollout.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/azure-devops-wiki-admin-setup

- **Deploy the Azure DevOps Wiki connector**
  Added a step-by-step deployment guide covering scope (project and code wikis), prerequisites, and configuration in the Microsoft 365 admin center. It explains both Federated Credential (service principal) and Microsoft Entra ID OAuth setups, including permissions, redirect URI, and secret management. Guidance includes rollout to targeted users, default settings, and customization options for access, identity mapping, project selection, schema, crawl cadence, and search result presentation. Related links connect readers to overview and troubleshooting content for end-to-end enablement.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/azure-devops-wiki-deployment

- **Azure DevOps Wiki connector overview**
  Introduced an overview describing the connector’s purpose, benefits, and key use cases, including how it can power agent experiences. The article outlines capabilities (indexing project and code wikis, natural language and semantic search) and limits (Azure DevOps Services only, one organization per connection). It documents available filters, default indexed properties, and the permissions model with Microsoft Entra identity mapping. A next-step path points to the deployment guide to get started.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/azure-devops-wiki-overview

- **Azure DevOps Wiki connector troubleshooting**
  Published a troubleshooting reference that maps common setup and crawl errors to clear resolutions. It covers authentication and permission issues (disabled OAuth, incorrect scopes, wrong app ID or secret), data access denials, expired credentials, and insufficient access levels affecting crawl. The article links to setup verification and related docs to streamline diagnosis and recovery.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/azure-devops-wiki-troubleshooting

## Major Changes

- **Federated connectors overview**
  Added Cowork to supported experiences and consolidated ISV publishing guidance, emphasizing a single connector manifest and pipeline across connector types. Updated admin controls to use Allowed agent types in Agent 365 instead of a tenant-wide PowerShell toggle; prior cmdlet settings no longer apply and must be reconfigured in the UI. Centralized management now allows admins to manage synchronized, federated, and supported Cowork plugins in one place, including from the Agent tab, and bulk disable guidance now references Allowed agent types. FAQs clarify that Allowed plugins settings apply to future federated connectors and reiterate the single-manifest ISV publishing model, reducing operational confusion.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/federated-connectors-overview

- **Deploy the Jira Data Center connector**
  Expanded guidance adds supported custom fields with recommended schema attributes and earliest compatible GCA versions, improving predictable indexing and query behavior. The update clarifies indexing for default and custom fields, shows how selected properties affect search and filtering, and provides a UI walkthrough for adding custom properties. It also documents governance rules for custom properties (naming, data types, reserved prefixes, and limits) and references the Jira REST API to discover available fields, helping admins configure robust, compliant deployments.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/jira-data-center-deployment

## Moderate Changes

- **Deploy the Jira Cloud connector**
  Added a reference list of supported Jira custom fields with recommended attributes for query, retrieval, and refinement. Included a step-by-step process to add custom properties in the connector configuration, with screenshots, plus a minor clarification to format NULL as code. These updates help admins map fields accurately and streamline configuration.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/jira-cloud-deployment