# Microsoft Foundry
**Date created:** 2026-09-01 UTC  
**Tags:** Best Practices, Billing, Compliance, Configuration, Consumption, Deprecation, Get Started, Governance, Guidance, Identity, Licensing, Monitoring, Performance, Security, Troubleshooting  

## New Articles

- **Bring your own registry for hosted agents**

  Introduced a how-to for deploying hosted agents from authenticated external or self-hosted registries. It covers setting up registry authentication with a project managed identity, including JFrog Artifactory via OIDC token exchange and Docker Distribution via an authentication adapter. The guide shows how to create a CustomKeys project connection with Azure Developer CLI, wire it into azure.yaml using docker.imagePassthrough and registryConnectionId, and optionally configure private network access with Private Link and private DNS. It concludes with deployment and validation steps using azd plus troubleshooting for token exchange, permissions, adapter compatibility, scoping, and networking/timeouts.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/private-registry-connections

## Major Changes

- **Create an indexed Azure SQL knowledge source (preview)**

  Updated to the 2026-08-01-preview API and added private network ingestion using a new networkAccessMode setting (public/private). Guidance details the private execution environment, required SKUs, shared private links to SQL and protected model endpoints, and managed identity authentication with connection string and identity selection rules. Samples across .NET, Python, and REST now use keyless Microsoft Entra ID authentication and remove API keys from model parameters. Prerequisites and permissions were clarified, and example payloads and terminology were standardized.

  https://learn.microsoft.com/en-us/azure/search/agentic-knowledge-source-how-to-azure-sql

- **Create a blob knowledge source from Azure Blob Storage or ADLS Gen2**

  Migrated to the 2026-08-01-preview API and introduced private network ingestion through networkAccessMode, with requirements for managed identity roles and shared private links to storage and protected model endpoints. Authentication guidance shifts to keyless Microsoft Entra ID across .NET, Python, and REST; API key fields were removed from examples and placeholders standardized. Prerequisites, SDK version guidance, and permission notes were refined for clarity and secure setup.

  https://learn.microsoft.com/en-us/azure/search/agentic-knowledge-source-how-to-blob

- **Create a File Knowledge Source for Agentic Retrieval**

  Upgraded to the 2026-08-01-preview API and significantly expanded capabilities and guidance. Added detailed file support and extraction options, including standard extraction with Content Understanding, image handling, and version-specific limits. Introduced improved upload flows (multipart with metadata), file updates by fileId, richer listing with filters, CORS setup for browser scenarios, and keyless authentication in all samples. New troubleshooting, pricing/billing notes, and references were added, and connectivity guidance now includes Foundry shared private links.

  https://learn.microsoft.com/en-us/azure/search/agentic-knowledge-source-how-to-file

- **Create a Search Index Knowledge Source**

  Updated to the 2026-08-01-preview API and adopted keyless authentication with Microsoft Entra ID for SDKs and REST. Clarified that semanticConfigurationName is optional in recent preview versions and aligned examples accordingly. Added a new section on query hints (preview) with filter and boost options, complete examples, limits, and how they interact with baseFilter and retrieval effort settings.

  https://learn.microsoft.com/en-us/azure/search/agentic-knowledge-source-how-to-search-index

- **Create a SharePoint (Indexed) Knowledge Source**

  Migrated to the 2026-08-01-preview API and introduced networkAccessMode to enable private ingestion with shared private links for dependencies. Prerequisites now cover SKUs, managed identity, and role assignments for private mode. SDK and REST samples were updated to keyless auth, API key fields were removed from model parameters, and examples set networkAccessMode explicitly.

  https://learn.microsoft.com/en-us/azure/search/agentic-knowledge-source-how-to-sharepoint-indexed

- **Create a Web Knowledge Source resource**

  Updated to the 2026-08-01-preview API and moved all samples to keyless authentication using Microsoft Entra ID. SDK prerequisites distinguish preview vs. GA packages, and REST examples use bearer tokens with standardized endpoint placeholders. The changes guide migration away from API keys and align all references to the latest preview.

  https://learn.microsoft.com/en-us/azure/search/agentic-knowledge-source-how-to-web

- **Create a Work IQ Knowledge Source**

  Upgraded to the 2026-08-01-preview API and replaced the legacy access flow with a customer-owned Microsoft Entra app registration and federated credentials. Added steps to configure delegated permissions, set up federated identity for the search service, and include entraAppAuthentication parameters in creation calls. Retrieval now requires a user assertion via a dedicated header with claim validation and updated troubleshooting. Samples adopt keyless auth across SDKs and REST, and governance/compliance guidance was expanded.

  https://learn.microsoft.com/en-us/azure/search/agentic-knowledge-source-how-to-work-iq

- **What is a Knowledge Source?**

  Aligned references to the 2026-08-01-preview API and clarified when indexed knowledge sources provide service-generated citation URLs versus remote sources. Added guidance on private ingestion for blob, indexed SharePoint, and indexed Azure SQL using shared private links, and noted that indexed OneLake does not support private synchronization. Removed an explicit prerequisites section and refined terminology around query types.

  https://learn.microsoft.com/en-us/azure/search/agentic-knowledge-source-overview

- **Create a Knowledge Base**

  Updated to the 2026-08-01-preview API and prioritized keyless Microsoft Entra ID authentication across SDKs and REST, relegating API keys to an alternative path. Expanded model support to include new gpt-5.5 and gpt-5.6 variants, consolidating GPT-4 deprecation guidance. Samples were modernized (DefaultAzureCredential, Authorization headers), AOAI keys removed from parameters, and configuration examples simplified. Introduced preview retrieveDefaults to set knowledge base-level defaults with precedence rules and examples.

  https://learn.microsoft.com/en-us/azure/search/agentic-retrieval-how-to-create-knowledge-base

- **Set the Retrieval Reasoning Effort**

  Added an “auto” reasoning effort mode and clarified defaults and behavior. Enhanced prerequisites and usage support, moved samples and references to the 2026-08-01-preview API, and adopted keyless auth for SDKs and REST. Provided comprehensive language-specific examples for configuring effort at the knowledge base level and overriding per request, including model requirements and scenario guidance.

  https://learn.microsoft.com/en-us/azure/search/agentic-retrieval-how-to-set-retrieval-reasoning-effort

- **Monitor generative AI applications (preview)**

  Substantially restructured the monitoring guide for managed online endpoints, focusing on scheduled evaluation with trends and alerts. Clarified prerequisites (workspace, evaluator deployment, user-assigned identity and roles, workspace connection) and added steps to enable inference data collection and required outputs. Streamlined monitor creation, configuration, and analysis guidance, updated links, and aligned to 2026-08-01-preview. References to model retirements and migration options were refreshed.

  https://learn.microsoft.com/en-us/azure/machine-learning/prompt-flow/how-to-monitor-generative-ai-applications?view=azureml-api-2

- **Page through Azure AI Search list results (preview)**

  Rewrote pagination guidance to use cursor-based pagination in 2026-08-01-preview with @odata.nextLink and $skiptoken. Added supported list operations and updated .NET, Python, and REST examples using pageSize, prefix filtering, and keyless authentication. Included best practices for handling continuation URLs, detecting terminal pages, and constraints when parameters change between calls.

  https://learn.microsoft.com/en-us/azure/search/search-how-to-page-list-results

- **What's New**

  Added an August 2026 section and updated to the 2026-08-01-preview API. Highlights include private ingestion for indexed sources, expanded file knowledge source features (including Serverless support and higher limits), Work IQ Entra app authentication, broader model support (gpt-5.5/gpt-5.6), auto retrieval reasoning effort, query hints, runtime and token budget defaults, per-source reranking, SSE streaming for retrieve, citation URLs for indexed sources, and cursor-based pagination across list APIs. Minor editorial updates to prior months were also included.

  https://learn.microsoft.com/en-us/azure/search/whats-new

## Moderate Changes

- **Create a Fabric Data Agent Knowledge Source**

  Updated to the 2026-08-01-preview API and marked Azure portal support as available. Shifted authentication guidance to keyless Microsoft Entra ID for .NET, Python, and REST, replacing API keys and updating samples and references.

  https://learn.microsoft.com/en-us/azure/search/agentic-knowledge-source-how-to-fabric-data-agent

- **Create a Fabric Ontology Knowledge Source**

  Migrated to the 2026-08-01-preview API with the usage table indicating Azure portal support. Added keyless authentication guidance and updated .NET, Python, and REST samples to use DefaultAzureCredential and bearer tokens, noting admin API key as an alternative.

  https://learn.microsoft.com/en-us/azure/search/agentic-knowledge-source-how-to-fabric-ontology

- **Create an indexed OneLake knowledge source**

  Updated to the 2026-08-01-preview API and moved examples to keyless authentication across SDKs and REST. Added a limitations note that private synchronization isn’t supported and to keep networkAccessMode public; examples reflect this and clarify SDK package guidance.

  https://learn.microsoft.com/en-us/azure/search/agentic-knowledge-source-how-to-onelake

- **Create a remote SharePoint knowledge source (preview)**

  Updated to the 2026-08-01-preview API and emphasized keyless Microsoft Entra ID authentication for SDKs and REST. Prerequisites and samples were revised to use DefaultAzureCredential, with API keys documented as an alternative path.

  https://learn.microsoft.com/en-us/azure/search/agentic-knowledge-source-how-to-sharepoint-remote

- **Use answer synthesis for citation-backed responses in Azure AI Search (preview)**

  Updated to the 2026-08-01-preview API with a new usage support matrix and standardized placeholders. Strengthened prerequisites for keyless authentication and updated REST and reference links to bearer tokens and the new preview version.

  https://learn.microsoft.com/en-us/azure/search/agentic-retrieval-how-to-answer-synthesis

- **Configure freshness-aware retrieval in Azure AI Search (preview)**

  Added a usage support matrix and moved to the 2026-08-01-preview API. Guidance now favors keyless authentication with Microsoft Entra ID across SDKs and REST, with API keys positioned as an alternative.

  https://learn.microsoft.com/en-us/azure/search/agentic-retrieval-how-to-configure-freshness

- **Create an index for agentic retrieval in Azure AI Search**

  Improved examples and corrected semantic configuration JSON structure. Removed apiKey from Azure OpenAI vectorizer examples to align with secure configuration practices and clarified example language.

  https://learn.microsoft.com/en-us/azure/search/agentic-retrieval-how-to-create-index

- **Tutorial: Build an end-to-end agentic retrieval solution using Azure AI Search**

  Aligned the tutorial to the 2026-08-01-preview API across instructions and example code, including the MCP endpoint. Ensures consistency with the latest preview version for all steps.

  https://learn.microsoft.com/en-us/azure/search/agentic-retrieval-how-to-create-pipeline

- **Surface document-embedded images in agentic retrieval (preview)**

  Updated to the 2026-08-01-preview API and added a usage support matrix. Clarified authentication nomenclature for tokens and API keys and refined permission wording in examples and tables.

  https://learn.microsoft.com/en-us/azure/search/agentic-retrieval-how-to-image-serving

- **Agentic retrieval in Azure AI Search**

  Updated the important notice to the 2026-08-01-preview API and clarified support for managed and custom solutions. Guidance now highlights building custom solutions via portal, REST, or SDKs and refines the intro description.

  https://learn.microsoft.com/en-us/azure/search/agentic-retrieval-overview

- **Vector stores in Azure Machine Learning (preview)**

  Added a note clarifying Azure AI Search vector search GA vs. AML vector index in prompt flow remaining in preview. Expanded RAG overview on chunking and embeddings and updated guidance to reflect vector generation/loading capabilities.

  https://learn.microsoft.com/en-us/azure/machine-learning/concept-vector-stores?view=azureml-api-2

- **Connect a Foundry IQ knowledge base to Foundry Agent Service**

  Updated all REST references, code samples, and troubleshooting to 2026-08-01-preview. Adjusted MCP endpoint parameters and example URLs to align with the new version across setup and tool configuration.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/foundry-iq-connect

- **Validate end-to-end private agentic retrieval**

  Migrated all references and REST endpoint examples to 2026-08-01-preview, including MCP target/server URLs and troubleshooting guidance. Ensures consistent versioning for knowledge source/base and MCP configuration steps.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/foundry-iq-tutorial-private-retrieval

- **Deploy models as standard deployments**

  Updated the end-to-end example to use the Bria-2.3-Fast model and revised endpoint naming and subscription examples. Replaced a Python listing call with the current client.serverless_endpoints.list() API to reflect best practices.

  https://learn.microsoft.com/en-us/azure/machine-learning/how-to-deploy-models-serverless?view=azureml-api-2

- **Manage notebook and terminal sessions**

  Reorganized guidance to clarify session persistence and performance impact. Added a “Manage active sessions” workflow and emphasized closing unused sessions via the management pane for better responsiveness.

  https://learn.microsoft.com/en-us/azure/machine-learning/how-to-manage-compute-sessions?view=azureml-api-2

- **Get started with RAG using a prompt flow sample**

  Added a prompt flow retirement notice and updated prerequisites to use an AML workspace and Microsoft Foundry Models for Azure OpenAI access. Streamlined enablement instructions and retitled the closing section to Related content.

  https://learn.microsoft.com/en-us/azure/machine-learning/how-to-use-retrieval-augmented-generation?view=azureml-api-2

- **Host LangGraph agents as Foundry hosted agents**

  Expanded to include Deep Agents hosting with ResponsesHostServer and InvocationsHostServer and added no-code hosting for existing agents using langchain_azure_ai.agents.hosting.run. Provided CLI usage, multi-graph handling, and an azure.yaml example; raised the minimum langchain-azure-ai version to 1.2.9.

  https://learn.microsoft.com/en-us/azure/foundry/how-to/develop/langchain-hosted-agents

- **Upgrade to the latest REST API in Azure AI Search**

  Updated to the 2026-08-01-preview API and added migration guidance for breaking changes in agentic retrieval and list operations. Introduced cursor-based pagination and clarified unchanged behavior for other APIs when upgrading.

  https://learn.microsoft.com/en-us/azure/search/search-api-migration

- **Use a blob indexer or knowledge source to ingest RBAC scopes metadata**

  Updated the Important notice and example requests to use the 2026-08-01-preview API. No structural changes, ensuring examples and references are current.

  https://learn.microsoft.com/en-us/azure/search/search-blob-indexer-role-based-access

- **Index content from SharePoint in Microsoft 365 (preview)**

  Switched all REST references and samples to 2026-08-01-preview and updated links accordingly. Made a minor wording tweak while retaining preview scope for container settings.

  https://learn.microsoft.com/en-us/azure/search/search-how-to-index-sharepoint-online

- **Tutorial: Configure multiple blob indexers for one search index**

  Updated the tutorial and troubleshooting references to 2026-08-01-preview across all REST operations and links. No procedural or conceptual changes beyond version alignment.

  https://learn.microsoft.com/en-us/azure/search/search-how-to-multiple-indexers-one-index

- **Use an ADLS Gen2 indexer to ingest permission metadata and filter search results based on user access rights (preview)**

  Updated the Important note and API examples to the 2026-08-01-preview version, including resetdocs and resync endpoints. Content otherwise unchanged.

  https://learn.microsoft.com/en-us/azure/search/search-indexer-access-control-lists-and-role-based-access

- **Indexer execution on Serverless and Standard 3 High Density (S3 HD)**

  Removed the note that file knowledge sources aren’t supported on Serverless, indicating feature parity. Updated REST example versions to 2026-08-01-preview.

  https://learn.microsoft.com/en-us/azure/search/search-indexer-high-density-serverless-overview

- **Use an Azure AI Search indexer to ingest Microsoft Purview sensitivity labels and enforce document-level security (preview)**

  Updated prerequisites, configuration guidance, and REST examples to 2026-08-01-preview and clarified Elevated Read requires 2026-05-01-preview or later. Links and version labels were aligned.

  https://learn.microsoft.com/en-us/azure/search/search-indexer-sensitivity-labels

- **Service limits in Azure AI Search**

  Clarified that starting with 2026-05-01-preview and later, all retrieval reasoning efforts share the same knowledge source limits. Updated the limits table label to reflect applicability.

  https://learn.microsoft.com/en-us/azure/search/search-limits-quotas-capacity

- **Configure customer-managed keys across different tenants**

  Updated preview API references to 2026-08-01-preview in federated identity guidance and example requests. Note text was adjusted to match the new version.

  https://learn.microsoft.com/en-us/azure/search/search-security-managed-encryption-cross-tenant

- **Choose a pricing model and service tier in Azure AI Search**

  Removed the statement that File Knowledge Source is not supported on the Serverless Developer tier, reflecting current support. No other changes.

  https://learn.microsoft.com/en-us/azure/search/search-sku-tier

- **Configure semantic ranker and return captions in search results**

  Replaced a lengthy explanation with a concise tip that agentic retrieval flows don’t require a semantic configuration starting with 2026-05-01-preview. Updated examples and links to the 2026-08-01-preview API and refined wording.

  https://learn.microsoft.com/en-us/azure/search/semantic-how-to-configure

- **Tutorial: Extract, chunk, and embed multimodal content with the Document Layout skill**

  Updated all REST requests, responses, and Location/@odata.nextLink examples to 2026-08-01-preview across data sources, indexers, and queries. No conceptual changes to the tutorial.

  https://learn.microsoft.com/en-us/azure/search/tutorial-multimodal