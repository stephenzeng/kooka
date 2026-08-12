# Microsoft Foundry
**Date created:** 2026-08-12 UTC  
**Tags:** Best Practices, Configuration, Deprecation, Guidance, Security, Troubleshooting  

## New Articles

- **Tutorial: Configure Multiple Blob Indexers for One Search Index**

  Introduced an end-to-end tutorial showing how to configure three folder-scoped Azure Blob indexers (DOCX, JSON, CSV) to feed a single Azure AI Search index with a nullable union schema. Covers prerequisites (managed identity, Azure Storage, Microsoft Foundry resource, embedding deployment, RBAC) and detailed setup, including a union-schema index with vector search and an Azure OpenAI vectorizer via Foundry. Provides step-by-step pipelines: DOCX with Content Understanding semantic chunking and embeddings, JSON with direct mappings, and CSV with embeddings mapped to a vector field. Includes run/monitor guidance, comprehensive query examples (full-text, vector, filtered vector, hybrid), operational practices (scheduling, reconciliation, deletion detection), and a troubleshooting table. Notes use of the 2026-05-01-preview API and associated preview considerations.

  https://learn.microsoft.com/en-us/azure/search/search-how-to-multiple-indexers-one-index

## Moderate Changes

- **Document Intelligence v4.0 migration**

  Added a deprecation notice announcing end of support for Document Intelligence REST preview API versions (2024-07-31-preview, 2024-02-29-preview, 2023-10-31-preview) on June 30, 2026. This update clarifies the timeline so teams can plan migrations to supported versions and avoid disruption.

  https://learn.microsoft.com/en-us/azure/ai-services/document-intelligence/versioning/migration-guide-overview?view=doc-intel-4.0.0

- **Index content from SharePoint in Microsoft 365 (preview)**

  Retired outdated troubleshooting guidance for failures when indexing encrypted SharePoint files, including the eTag mismatch with irmEncryptFailedToFindProtector example. This streamlines the article and helps readers rely on current encryption and discovery practices when diagnosing indexing issues.

  https://learn.microsoft.com/en-us/azure/search/search-how-to-index-sharepoint-online