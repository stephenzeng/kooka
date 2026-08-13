# Azure Monitor
**Date created:** 2026-08-13 UTC  
**Tags:** Deprecation, Guidance  

## Major Changes

- **Migrate to Azure Monitor Agent from Azure Diagnostic extensions (WAD/LAD)**

  Added a deprecation notice for the ADX/Fabric preview destination used in the routing step, retiring on September 1, 2026. Updated guidance directs customers to route data to a Log Analytics workspace going forward and use Mirror Azure Monitor in Fabric for analysis. This change ensures continuity of log ingestion and analytics and helps customers avoid disruption as preview capabilities retire.

  https://learn.microsoft.com/en-us/azure/azure-monitor/agents/azure-monitor-agent-migration-wad-lad

- **Send data to Fabric and Azure Data Explorer (Preview)**

  Announced retirement of the preview capability that sends data to Azure Data Explorer and Fabric eventhouse via Azure Monitor Agent Data Collection Rules, effective September 1, 2026. Readers are advised to transition to the Mirror Azure Monitor (preview) feature for Fabric-based analytics. Taking action now helps prevent ingestion pipeline breakage and aligns deployments with supported data paths.

  https://learn.microsoft.com/en-us/azure/azure-monitor/vm/send-fabric-destination

## Moderate Changes

- **Mirror Azure Monitor Data in Microsoft Fabric (Preview)**

  Clarified that the DCR capability “Send data to a Fabric destination” retires on September 1, 2026, and explained that Mirrored Azure Monitor keeps logs within Azure Monitor, unlike the retiring DCR route. This update helps customers plan transitions while maintaining governance and retention in Azure Monitor.

  https://learn.microsoft.com/en-us/azure/azure-monitor/fundamentals/monitor-cross-domain-fabric