# Microsoft Fabric
**Date created:** 2026-08-10 UTC  
**Tags:** Guidance  

## Major Changes

- **Data Factory limitations overview**

  Updated the Data Factory limitations to reflect new capabilities and clearer guidance. Clarified that tumbling window scheduling is partially available via interval-based schedules (time slices supported) with no backfill. Expanded authentication and activity support: connectors now support OAuth and Azure Key Vault; Managed Identity is no longer limited to Azure Blob; Web activity supports service principal; and previously unavailable items (Validation activity, Mapping Data Flow activity, SSIS integration runtime) are now listed as supported. Retained important constraints, including that GetMetadata and Script activities cannot source from Fabric KQL databases and background authentication sync considerations.

  https://learn.microsoft.com/en-us/fabric/data-factory/data-factory-limitations