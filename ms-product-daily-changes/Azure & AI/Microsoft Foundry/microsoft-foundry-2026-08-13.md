# Microsoft Foundry
**Date created:** 2026-08-13 UTC  
**Tags:** Best Practices, Compliance, Configuration, Get Started, Governance, Guidance, Identity, Performance, Security, Troubleshooting  

## New Articles

- **Azure AI Search Preview Terms**

  Introduced a dedicated article outlining the scope and conditions for Azure AI Search preview features, including SLA exclusions, production-use cautions, and change readiness. Describes licensing and data-handling implications under Microsoft Product Terms, DPA, and Azure preview supplemental terms. Explains access/permission timing, CORS considerations for browser-based access, and responsible AI expectations with recommended mitigations. References the 2026-05-01-preview REST API and links to transparency and supplemental terms.

  https://learn.microsoft.com/en-us/azure/search/search-preview-terms

- **Troubleshoot SharePoint Permission Filtering**

  Added a comprehensive troubleshooting guide for query-time permission filtering with SharePoint data in Azure AI Search. Provides a stepwise decision tree to validate identities, configuration, supported group relationships, delegated tokens, and required preview API versions. Offers methods to isolate permission behavior, compare expected vs actual results safely, and capture diagnostics for support.

  https://learn.microsoft.com/en-us/azure/search/troubleshoot-sharepoint-query-permission-filtering

- **Deploy and use MAI-Thinking-1 in Microsoft Foundry**

  Introduced a how-to for deploying and using the MAI-Thinking-1 model for advanced reasoning, agentic coding, and long-context workflows. Explains the model’s scenarios and structured output use, with step-by-step procedures provided via an include. Notes availability across the new and classic experiences where applicable.

  https://learn.microsoft.com/en-us/azure/foundry/foundry-models/how-to/use-foundry-models-mai-thinking

## Major Changes

- **azure.yaml reference for hosted agents**

  Significantly expanded the reference for Foundry project configuration. Adds updated azd behavior and environment variable changes, extension compatibility/versioning guidance, private-networking settings, agent discovery card metadata, Responsible AI policy association, memory store settings, and agent endpoint protocols/authorization. Clarifies environment variables, identity provisioning, deployment options (source code and container images), and lifecycle rules for services, skills, and routines. Provides migration guidance and deeper file-include and schema expectations to reduce misconfiguration and improve governance and security.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/azure-yaml-reference

- **Deployment types for Microsoft Foundry Models**

  Restructured and expanded guidance to compare deployment types in detail and help readers choose appropriately. Adds an introduction, instant models considerations, workload pattern guidance, and clearer comparisons with expanded details. This improves decision-making for teams evaluating trade-offs across deployment options.

  https://learn.microsoft.com/en-us/azure/foundry/foundry-models/concepts/deployment-types

## Moderate Changes

- **Create a SharePoint (Indexed) Knowledge Source**

  Clarified how the SharePoint connection string and TenantId rules are applied and aligned generated objects with the SharePoint indexer’s prerequisites, supported formats, and limits. Added troubleshooting paths for permission-enforced results and guidance for known tenant validation/authentication errors, including reviewing indexer status/history.

  https://learn.microsoft.com/en-us/azure/search/agentic-knowledge-source-how-to-sharepoint-indexed

- **Author azure.yaml for hosted agents**

  Updated prerequisites and minimum versions for azd and required extensions, and renamed the model deployment variable to MICROSOFT_FOUNDRY_MODEL_DEPLOYMENT_NAME. Clarified unified azure.yaml behavior for hosted agents, split-service toolbox connections, and added an advanced capabilities section. Refreshed examples and troubleshooting to align with the new variable and features.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/author-azure-yaml

- **Indexer Errors and Warnings**

  Added guidance for the “Invalid AAD tenant” error when the SharePoint indexer authenticates to the wrong Microsoft Entra tenant. Explains when to specify TenantId, managed identity behavior when TenantId is omitted, expected error messages, and how to validate indexer history in the portal.

  https://learn.microsoft.com/en-us/azure/search/cognitive-search-common-errors-warnings

- **Azure Content Understanding skill**

  Consolidated the preview disclaimer and explicitly marked preview features and parameters, including semantic chunking, modelName/modelDeployment, and unit=tokens. Updated examples and tables to reflect preview scope without altering functionality, improving clarity around responsibilities and limits.

  https://learn.microsoft.com/en-us/azure/search/cognitive-search-skill-content-understanding

- **Connect a Foundry IQ knowledge base to Foundry Agent Service**

  Clarified RBAC requirements for assigning roles, specifying that users need Owner or User Access Administrator (or equivalent) on both resources. Retained guidance for key-based authentication as a fallback where role assignment isn’t feasible.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/foundry-iq-connect

- **Foundry Agent Service limits, quotas, and regional support**

  Expanded the region availability table, adding several new regions and updating tool availability flags. Adjusted existing entries to reflect current support, helping teams plan deployments and tool usage by region.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/limits-quotas-regions

- **Use model router for Microsoft Foundry**

  Updated agentic request guidance to state that the router can select eligible OpenAI, OSS, and Anthropic models based on tool compatibility. Added references to region/model tool support and clarified how routing works across supported options.

  https://learn.microsoft.com/en-us/azure/foundry/openai/how-to/model-router

- **Use model router with Foundry agents**

  Simplified supported tool types guidance and clarified eligibility across OpenAI, OSS, and Anthropic models with a link to the compatibility matrix. Noted that routing to Claude requires separate deployments in the router pool and updated the example to include gpt-5.6-sol for Quality mode.

  https://learn.microsoft.com/en-us/azure/foundry/openai/how-to/model-router-agents

- **Document-Level Access Control**

  Streamlined SharePoint ACLs content by summarizing the approach and pointing to a dedicated article for details on supported content, principals, synchronization, and permissions. Removed duplicative steps and cross-references to centralize authoritative guidance.

  https://learn.microsoft.com/en-us/azure/search/search-document-level-access-overview

- **Index content from SharePoint in Microsoft 365 (preview)**

  Consolidated ACL-related scenarios into a single permissions matrix entry pointing to a dedicated article. Clarified group relationship support, managed identity setup, TenantId requirements—including cross-tenant cases—and updated examples. Added troubleshooting links for tenant mismatches and clarified indexer and skill input limits.

  https://learn.microsoft.com/en-us/azure/search/search-how-to-index-sharepoint-online

- **Indexer Execution on Serverless and S3 HD**

  Clarified API version requirements, noting S3 HD indexers now require the 2025-11-01-preview REST API and distinguishing between Serverless and S3 HD. Specified that only indexer-backed knowledge sources are supported and reminded readers that service quotas don’t override individual skill and external service limits.

  https://learn.microsoft.com/en-us/azure/search/search-indexer-high-density-serverless-overview

- **Use a SharePoint indexer to ingest permission metadata and filter search results based on user access rights (preview)**

  Added a supported group relationships section covering direct assignments, Entra group nesting, SharePoint group assignments, and unsupported Entra-in-SharePoint nesting. Included troubleshooting references for unexpected permission-filtering results.

  https://learn.microsoft.com/en-us/azure/search/search-indexer-sharepoint-access-control-lists

- **Service limits in Azure AI Search**

  Restructured indexer limits to highlight object/throughput constraints and introduced a dedicated section for blob-like source-file limits across major data sources. Clarified per-skill AI enrichment character limits and recommended using Text Split for larger inputs.

  https://learn.microsoft.com/en-us/azure/search/search-limits-quotas-capacity

- **Query-Time ACL and RBAC Enforcement**

  Clarified that Entra groups nested within SharePoint groups aren’t expanded and linked to supported relationships. Added troubleshooting references for SharePoint permission filtering and specified the query token as a Microsoft Entra access token for the querying user.

  https://learn.microsoft.com/en-us/azure/search/search-query-access-control-rbac-enforcement

- **Model router for Microsoft Foundry**

  Added a supported regions section explaining router availability for Global Standard and Data Zone Standard, with a full region list. Clarified that routing is limited to models available in each region and made minor formatting improvements for readability.

  https://learn.microsoft.com/en-us/azure/foundry/openai/concepts/model-router