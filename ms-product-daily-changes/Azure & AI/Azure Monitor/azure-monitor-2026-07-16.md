# Azure Monitor
**Date created:** 2026-07-16 UTC  
**Tags:** AI, Analytics, Monitoring, Security  

## New Articles

- **Advanced platform metrics (preview)**
  
  Introduced a new concept article for Advanced platform metrics, a paid, opt-in tier that provides more granular Azure Monitor platform metrics. The article explains how it differs from standard metrics (cost, configuration, granularity, availability), how it is enabled, and expected provisioning latency. It also lists currently supported resource providers and links to provider-specific enablement guidance, with pricing notes and related references.
  
  https://learn.microsoft.com/en-us/azure/azure-monitor/metrics/metrics-advanced-platform

## Moderate Changes

- **Azure Monitor REST API index**
  
  Expanded the index to include a new Search operation group for querying Basic and Auxiliary/Lake table logs via REST, and added a Search job entry describing how to create special search tables. Clarified that the Query entry targets Analytics tables. These updates make it easier to find the right API for each log store and scenario.
  
  https://learn.microsoft.com/en-us/azure/azure-monitor/fundamentals/azure-monitor-rest-api-index

- **Application Insights telemetry data model**
  
  Standardized the generative AI telemetry table identifier from GenAIContent to genAIContent across tables, text, and the migration heading. This aligns the documentation to the actual table name and reduces confusion during migrations.
  
  https://learn.microsoft.com/en-us/azure/azure-monitor/app/data-model-complete

- **Supported metrics - Microsoft.Compute/virtualMachines**
  
  Added an Advanced platform metrics column and description to indicate whether each metric participates in the paid advanced tier (all listed as No). This clarifies premium eligibility without changing metric names, definitions, or dimensions.
  
  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-compute-virtualmachines-metrics

- **Supported metrics - Microsoft.Storage/storageAccounts**
  
  Added an Advanced platform metrics column across Capacity and Transaction tables, indicating Yes/No with links to advanced metrics guidance. This helps readers quickly see which storage metrics support the advanced tier while leaving metric definitions unchanged.
  
  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-storage-storageaccounts-metrics

- **Supported metrics - Microsoft.EventHub/Namespaces**
  
  Introduced an Advanced platform metrics column and definition in headings, marking all listed metrics as not part of the advanced tier. The update improves transparency on premium eligibility without altering existing metrics.
  
  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-eventhub-namespaces-metrics

- **Supported metrics - Microsoft.KeyVault/vaults**
  
  Added an Advanced platform metrics column and explanatory note to indicate premium eligibility (set to No for listed metrics). This enhances categorization and does not change metric semantics.
  
  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-keyvault-vaults-metrics

- **Supported metrics - Microsoft.Network/virtualnetworkgateways**
  
  Introduced an Advanced platform metrics column across Errors, Ipsec, Performance, Routing, Scalability, and Traffic tables, with definitions in headings (all values set to No). This update clarifies advanced tier applicability while preserving existing metric details.
  
  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-network-virtualnetworkgateways-metrics

- **Supported metrics - Microsoft.ContainerService/managedClusters**
  
  Added an Advanced platform metrics column to API Server, ETCD, Nodes, and Pods tables (including preview categories), documenting advanced tier status (set to No). This makes premium eligibility explicit without changing metrics or units.
  
  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-containerservice-managedclusters-metrics

- **Supported metrics - microsoft.insights/components**
  
  Introduced an Advanced platform metrics column across Availability, Browser, Failures, Performance counters, Server, and Usage tables, with updated heading descriptions (all set to No). Readers can now see premium applicability at a glance.
  
  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-insights-components-metrics

- **Supported metrics - Microsoft.Sql/servers/databases**
  
  Added an Advanced platform metrics column to Basic, InstanceAndAppAdvanced, and WorkloadManagement tables and defined the concept in headings (all set to No). The change improves guidance on premium eligibility without altering metric behavior.
  
  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-sql-servers-databases-metrics

- **Supported metrics - Microsoft.CognitiveServices/accounts**
  
  Added an Advanced platform metrics column across numerous tables (for example, Azure OpenAI HTTP Requests, Latency, Usage; Cognitive Services SLI; and others), with a definition in headings (primarily set to No). This standardizes how advanced eligibility is shown across AI service metrics.
  
  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-cognitiveservices-accounts-metrics

- **Supported metrics - Microsoft.Web/sites**
  
  Introduced an Advanced platform metrics column and description, marking all listed metrics as not part of the advanced tier. This clarifies classification while leaving metric definitions intact.
  
  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-web-sites-metrics