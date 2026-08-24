# Microsoft Foundry
**Date created:** 2026-08-24 UTC  
**Tags:** Compliance, Configuration, Get Started, Governance, Guidance, Identity, Monitoring, Performance, Security, Troubleshooting  

## New Articles

- **Region support for Azure Translator in Foundry Tools**

  Introduced a comprehensive guide to region support, endpoints, and data processing locations for Translator across Text, Document, and Custom Translator in Foundry Tools. Explains differences between standard NMT and LLM-based translation, including global/geography/resource-specific routing and LLM deployment types. Provides region behavior for Document Translation and Custom Translator, with guidance on managed identity, data handling, and VNet requirements. Includes data residency considerations, sovereign cloud notes, and business continuity recommendations with links to related resources.

  https://learn.microsoft.com/en-us/azure/ai-services/translator/region-support

## Major Changes

- **Surface document-embedded images in agentic retrieval (preview)**

  Overhauled guidance for enabling and using image serving, including updated prerequisites, role assignments, and clearer managed identity usage with Foundry endpoints. Introduces and clarifies limitations (image serving via retrieve API only for answer synthesis and not supported with ingestionPermissionOptions), and revises retrieval responses and activity reporting. Refines indexing and retrieval behavior for standard content extraction, figure verbalization, and metrics such as verbalizationUsed, imagesRetrieved, imagesSentToModel, and totalImageSizeBytes. Updates configuration and examples to bearer auth, ResourceId storage connections, and restructured model settings, plus end-to-end C#/Python samples, cleanup steps, and focused troubleshooting.

  https://learn.microsoft.com/en-us/azure/search/agentic-retrieval-how-to-image-serving

## Moderate Changes

- **Create a Blob Knowledge Source for Agentic Retrieval**

  Added prerequisites for standard content extraction using a Microsoft Foundry resource and endpoint, including deployment of embedding and multimodal chat models and managed identity role requirements. Updated SDK namespaces and REST examples to use bearer authentication, ResourceId-based storage connections, and removed inline apiKey fields. Clarified that image serving isn’t supported when ingestionPermissionOptions is configured and removed obsolete error notes.

  https://learn.microsoft.com/en-us/azure/search/agentic-knowledge-source-how-to-blob

- **Create an indexed OneLake knowledge source**

  Added Foundry-based prerequisites for standard content extraction, including region support and deploying embedding and multimodal chat models. Updated REST guidance to use bearer tokens and removed apiKey fields, and documented that image serving isn’t supported when ingestionPermissionOptions is configured. Included minor query guidance refinements and removed outdated “Known errors” content.

  https://learn.microsoft.com/en-us/azure/search/agentic-knowledge-source-how-to-onelake

- **Create an indexed SharePoint knowledge source (preview)**

  Introduced prerequisites for standard content extraction with Foundry endpoints and required models, and switched the example to bearer authentication and a federated SharePoint connection string. Removed explicit model apiKey fields and noted that image serving isn’t supported with ingestionPermissionOptions. Cleaned up a troubleshooting note tied to Content Understanding defaults.

  https://learn.microsoft.com/en-us/azure/search/agentic-knowledge-source-how-to-sharepoint-indexed

- **What is a knowledge source?**

  Clarified configuration guidance: don’t configure assetStore and ingestionPermissionOptions together on the same knowledge source. Noted that enabling ingestionPermissionOptions disables image serving (preview), helping teams choose the right approach for retrieval scenarios.

  https://learn.microsoft.com/en-us/azure/search/agentic-knowledge-source-overview

- **Query a knowledge base using the retrieve action or MCP endpoint**

  Renamed the images subsection and clarified that document-embedded images from blob, indexed OneLake, and indexed SharePoint are supplied to the answer-synthesis model, not returned as fields in the retrieve response. Added a limitation for ingestionPermissionOptions and expanded metrics guidance, explicitly detailing verbalizationUsed, imagesRetrieved, imagesSentToModel, and totalImageSizeBytes.

  https://learn.microsoft.com/en-us/azure/search/agentic-retrieval-how-to-retrieve

- **Troubleshooting common indexer errors and warnings in Azure AI Search**

  Expanded authentication troubleshooting for managed identities, including enabling system or user-assigned identities and assigning roles at the correct scope. Added a concrete example for granting Storage Blob Data Reader at the storage-account scope for Azure Blob data sources.

  https://learn.microsoft.com/en-us/azure/search/cognitive-search-common-errors-warnings

- **Enable Custom Translator through Azure Virtual Network**

  Replaced the inline billing region code list with guidance to use the resource’s billing region code and a link to centralized region support. Clarified the usage wording for the Create a workspace API call to reduce configuration errors.

  https://learn.microsoft.com/en-us/azure/ai-services/translator/custom-translator/how-to/enable-vnet-service-endpoint

- **What is Azure Translator document translation?**

  Consolidated data residency and endpoint guidance to reference a centralized Region support page and removed redundant regional tables and notes. Clarified processing location behavior, custom endpoint requirements, and managed identity considerations.

  https://learn.microsoft.com/en-us/azure/ai-services/translator/document-translation/overview

- **Azure Translator in Foundry Tools v3.0**

  Simplified Base URLs by removing lengthy global/regional endpoint lists and examples. Points readers to a centralized Region support page for endpoint URLs and processing location details.

  https://learn.microsoft.com/en-us/azure/ai-services/translator/text-translation/reference/v3/reference

- **.NET Samples**

  Added a new image-serving sample for agentic retrieval (preview), with guidance for managed ingestion, A/B retrieval testing, and querying/downloading image references from Azure Blob Storage. Removed the outdated AzureSearch_JFK_Files demo entry.

  https://learn.microsoft.com/en-us/azure/search/samples-dotnet

- **Python Samples**

  Added an image-serving sample entry that demonstrates extracting and serving document-embedded images during answer synthesis, plus querying and downloading image references from Azure Blob Storage.

  https://learn.microsoft.com/en-us/azure/search/samples-python

- **Document-level access control in Azure AI Search**

  Added a note that combining ingestionPermissionOptions with assetStore isn’t supported for indexed knowledge sources. This configuration disables image serving (preview), guiding teams to align security with retrieval capabilities.

  https://learn.microsoft.com/en-us/azure/search/search-document-level-access-overview

- **Use an ADLS Gen2 indexer to ingest permission metadata and filter search results based on user access rights (preview)**

  Clarified that Knowledge store includes the asset store required for image serving (preview) and that image serving isn’t supported when ingesting ACLs or RBAC scopes. Helps teams plan for image-enriched retrieval while enforcing document-level permissions.

  https://learn.microsoft.com/en-us/azure/search/search-indexer-access-control-lists-and-role-based-access

- **Use an Azure AI Search indexer to ingest Microsoft Purview sensitivity labels and enforce document-level security (preview)**

  Updated Knowledge store guidance to include the asset store dependency for image serving (preview) and noted that image serving isn’t supported when ingesting sensitivity labels. Ensures expectations are set for image availability in secured scenarios.

  https://learn.microsoft.com/en-us/azure/search/search-indexer-sensitivity-labels

- **Use a SharePoint indexer to ingest permission metadata and filter search results based on user access rights (preview)**

  Clarified that the asset store is required for image serving (preview) and stated that image serving isn’t supported for knowledge sources ingesting SharePoint ACLs. Aligns image-serving expectations with permission ingestion configurations.

  https://learn.microsoft.com/en-us/azure/search/search-indexer-sharepoint-access-control-lists

- **What is Azure Translator text translation?**

  Replaced detailed endpoint tables with a Region support reference and clarified that NMT endpoints and Foundry LLM deployments follow different processing boundaries. Removed Switzerland-specific endpoint guidance and adjusted headings for clarity.

  https://learn.microsoft.com/en-us/azure/ai-services/translator/text-translation/2026-06-06/overview