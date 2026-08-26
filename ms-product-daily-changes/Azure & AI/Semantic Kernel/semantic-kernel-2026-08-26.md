# Semantic Kernel
**Date created:** 2026-08-26 UTC  
**Tags:** Configuration, Guidance  

## Major Changes

- **Using the Semantic Kernel Azure DocumentDB (with MongoDB compatibility) Vector Store connector (Preview)**

  Retargeted the connector from Azure Cosmos DB MongoDB (vCore) to Azure DocumentDB (with MongoDB compatibility) and aligned terminology across headings and content. Updated warnings and limitations to make clear it does not apply to Cosmos DB MongoDB (RU). Revised feature mapping so a collection corresponds to an Azure DocumentDB Collection + Index. Updated setup guidance, including changing the NuGet package to CommunityToolkit.VectorData.AzureDocumentDB and the DI extension to AddDocumentDBVectorStore, helping developers migrate dependencies and avoid misconfiguration.

  https://learn.microsoft.com/en-us/semantic-kernel/concepts/vector-store-connectors/out-of-the-box-connectors/azure-cosmosdb-mongodb-connector

- **Using the Azure CosmosDB NoSQL Vector Store connector (Preview)**

  Renamed packages, APIs, and types from CosmosNoSql to Azure Cosmos DB to standardize naming and improve clarity. Updated the NuGet package, DI extensions, types, options, and keys (e.g., CosmosKey) and refreshed code samples to match the new surface area. Refined wording to consistently reference Azure Cosmos DB and removed the C# language pivot warning while retaining the Python note, streamlining guidance and easing migration.

  https://learn.microsoft.com/en-us/semantic-kernel/concepts/vector-store-connectors/out-of-the-box-connectors/azure-cosmosdb-nosql-connector

## Moderate Changes

- **What are Semantic Kernel Vector Stores? (Preview)**

  Reworked the overview to clarify platform differences: Python uses Semantic Kernel abstractions, while .NET relies on a .NET Foundation abstraction with provider and community implementations. Consolidated the description of common capabilities and removed prior claims about connector independence and the “connector” naming, providing clearer architecture and terminology.

  https://learn.microsoft.com/en-us/semantic-kernel/concepts/vector-store-connectors/