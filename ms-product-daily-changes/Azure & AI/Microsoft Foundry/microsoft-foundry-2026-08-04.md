# Microsoft Foundry
**Date created:** 2026-08-04 UTC  
**Tags:** Administration, Agent, AI, Automation, Programming, Security  

## New Articles

- **What is the Foundry Agent Canvas?**

  Introduced a concept article for the Foundry Agent Canvas, a GitHub Copilot App extension that helps you design, configure, test, and deploy Microsoft Foundry hosted agents from a side panel. It scaffolds and edits agent code based on project selections, supports browsing and adding models, toolboxes, skills, and guardrails, and enables local testing with Agent Inspector before deploying to Foundry Agent Service. The article walks through installation options and an end-to-end workflow, noting that Inspect Locally and Deploy actions run azd commands, and links to related quickstarts and how-to guides.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/foundry-canvas

- **Content provenance**

  Added a new article that defines content provenance and clarifies it provides origin signals rather than guarantees of truthfulness. It explains two signals—C2PA manifests (cryptographically signed metadata) and invisible watermarks (verifiable via Microsoft’s detection)—and when they apply. A multimodal support section lists image model families and specific models that include invisible watermarks and C2PA credentials to help teams evaluate provenance features.

  https://learn.microsoft.com/en-us/azure/foundry/responsible-ai/content-understanding/provenance-disclosure

## Major Changes

- **Use a SharePoint indexer to ingest permission metadata and filter search results based on user access rights (preview)**

  Expanded guidance for SharePoint ACL ingestion with Azure AI Search, including a comprehensive Limitations section and a detailed explanation of how hierarchical permissions are evaluated. Added a section on finding the correct Microsoft Entra identifiers with a mapping table and step-by-step instructions for obtaining the FederatedCredentialApplicationId for system- and user-assigned managed identities. Standardized metadata naming from metadata_sharepoint_site_url to metadata_spo_site_url across field mappings, projections, tables, examples, and troubleshooting. Troubleshooting was broadened to cover site URL population, 401/403 errors, and correct use of federated credentials, and content was reorganized for clarity to reduce configuration errors.

  https://learn.microsoft.com/en-us/azure/search/search-indexer-sharepoint-access-control-lists

## Moderate Changes

- **Create a file knowledge source (preview)**

  Added an explicit limit of up to 100 files per file knowledge source and recommended using a blob knowledge source for larger sets, scheduled ingestion, lifecycle management, or existing content in Azure Storage. Clarified that re-uploading the same filename does not replace the file; replacement requires deleting the prior version by fileId before uploading. Also refined notes about where uploaded content is stored to set expectations for governance and operations.

  https://learn.microsoft.com/en-us/azure/search/agentic-knowledge-source-how-to-file

- **Microsoft Foundry SDKs and Endpoints**

  Updated the C# example to use the Azure.AI.Extensions.OpenAI namespace, introduce a deploymentName constant, and switch to ProjectResponsesClient with updated response creation and output access patterns. These changes align the sample with current SDK structures to help developers initialize clients and read responses correctly.

  https://learn.microsoft.com/en-us/azure/foundry/how-to/develop/sdk-overview

- **Define an index projection for parent-child indexing**

  Clarified permission metadata inheritance by updating examples to use metadata_spo_site_url instead of metadata_sharepoint_site_url. Reinforced that each chunk must inherit ACL-related fields (such as metadata_user_ids, metadata_group_ids, and metadata_spo_site_url) so query-time permission filters work reliably.

  https://learn.microsoft.com/en-us/azure/search/search-how-to-define-index-projections

- **Index content from SharePoint in Microsoft 365 (preview)**

  Expanded guidance for federated credentials, clearly distinguishing ApplicationId (ingestion app) from FederatedCredentialApplicationId (managed identity client ID) and how to set them in connection strings. Added configuration examples for system-assigned and user-assigned managed identities, including cross-tenant scenarios, with notes on when to include the identity block and differing TenantId requirements. Introduced a required metadata field, metadata_spo_site_url, to support SharePoint site group resolution.

  https://learn.microsoft.com/en-us/azure/search/search-how-to-index-sharepoint-online

- **Use an ADLS Gen2 indexer to ingest permission metadata and filter search results based on user access rights (preview)**

  Removed references to the GenAI Prompt skill and guidance about disableImageVerbalization, reflecting that this skill is not supported for ADLS Gen2 permission inheritance. This avoids misconfiguration and streamlines the recommended setup.

  https://learn.microsoft.com/en-us/azure/search/search-indexer-access-control-lists-and-role-based-access

- **Use an Azure AI Search indexer to ingest Microsoft Purview sensitivity labels and enforce document-level security (preview)**

  Removed the GenAI Prompt skill from the list of supported items for this feature. This clarifies current capabilities and prevents reliance on unsupported skills in security-sensitive pipelines.

  https://learn.microsoft.com/en-us/azure/search/search-indexer-sensitivity-labels

- **Service limits in Azure AI Search**

  Added a troubleshooting section to diagnose quota, capacity, and limit failures, including a table that maps common errors to likely causes and first actions. Guidance includes verifying subscription quotas, regional capacity constraints, dependent service throttling, and provisioning states, plus what information to provide when opening an Azure support request.

  https://learn.microsoft.com/en-us/azure/search/search-limits-quotas-capacity