# Azure Monitor
**Date created:** 2026-08-28 UTC  
**Tags:** Analytics, Compliance, Deprecation, Guidance, Monitoring, Performance, Security  

## New Articles

- **Azure Monitor Logs reference - QuantumProviderAccountMessageAuditLogs**

  Introduced a new reference page documenting the QuantumProviderAccountMessageAuditLogs table for Azure Quantum Provider Accounts. The article details the table’s purpose (auditing provider message operations), supported resource types and categories, and end-to-end column schema such as message metadata, requester identifiers, scheduled windows, and result codes. It also links to sample queries to help teams start analyzing activity quickly and establish governance.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/quantumprovideraccountmessageauditlogs

## Major Changes

- **Supported metrics - Microsoft.Network/dnsResolvers**

  Deprecated the existing Queries Per Second (QPS) metric and introduced a new QPS metric (QPSMdm) with the EndpointArmResourceId dimension. The new metric supports only Sum aggregation and offers 1-minute granularity to improve accuracy and consistency. Customers should migrate alerts, dashboards, and exports to QPSMdm to ensure continuity and align with the updated dimension model.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-network-dnsresolvers-metrics

## Moderate Changes

- **AADNonInteractiveUserSignInLogs**

  Added the RootActorID column to capture the root actor virtual ID for non-interactive sign-ins. This improves attribution and investigation workflows by linking activity to the initiating actor.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/aadnoninteractiveusersigninlogs

- **AGWAccessLogs**

  Added AdvancedRoutingConditionSetName, AdvancedRoutingMapName, and AdvancedRoutingRulePriority columns. These fields enable deeper troubleshooting and analytics for advanced routing decisions on Application Gateway.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/agwaccesslogs

- **Functions in Azure Monitor log queries**

  Updated guidance to match the current workspace experience, including discovering functions via categories/search and running them directly with the Run action. Clarified editing flows (switching to KQL mode, loading to editor, using Save as function) and IntelliSense behavior to streamline authoring and reuse.

  https://learn.microsoft.com/en-us/azure/azure-monitor/logs/functions

- **Supported metrics - Microsoft.CognitiveServices/accounts**

  Added ServiceTierRequest and ServiceTierResponse dimensions across several Azure OpenAI latency and usage metrics. This enables filtering and segmentation by service tier to analyze performance and consumption patterns.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-cognitiveservices-accounts-metrics

- **Supported metrics - Microsoft.CognitiveServices/accounts/projects**

  Introduced six preview Toolbox metrics (ToolboxCallToolCalls, ToolboxToolsDeferred, ToolboxToolSearchCalls, ToolboxToolSearchEnabled, ToolboxToolSearchResults, ToolboxToolsVisible). These provide visibility into tool discovery, usage, and deferrals for targeted optimization.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-cognitiveservices-accounts-projects-metrics

- **Supported metrics - Microsoft.DocumentDB/DatabaseAccounts**

  Added Throttled Request Percentage (ThrottledRequestPercentage) to measure the share of requests limited by provisioned throughput. This helps detect RU pressure, tune capacity, and set alerts to protect workload performance.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-documentdb-databaseaccounts-metrics

- **Supported metrics - Microsoft.Network/expressRouteCircuits**

  Added MulticloudInterconnectBitsInPerSecond and MulticloudInterconnectBitsOutPerSecond metrics. These track interconnect bandwidth at 1-minute granularity to improve capacity planning and network monitoring.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-network-expressroutecircuits-metrics

- **Supported metrics - microsoft.network/virtualnetworkgateways**

  Expanded time granularity to 1-minute across error, routing, and traffic metrics. Finer intervals enable near real-time monitoring, faster incident detection, and tighter alert thresholds.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-network-virtualnetworkgateways-metrics

- **Supported metrics - microsoft.network/vpngateways**

  Enabled 1-minute time granularity across multiple VPN Gateway metrics spanning errors, routing, and traffic. This improves operational visibility and shortens detection and response times for network issues.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-network-vpngateways-metrics

- **Log Analytics tables for microsoft.quantum/provideraccounts**

  Added the QuantumProviderAccountMessageAuditLogs table entry with description and reference link. This makes auditing provider message management operations discoverable in the table catalog.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/microsoft-quantum-provideraccounts

- **Supported log categories - Microsoft.StorageMover/storageMovers**

  Introduced the AuditLog category mapped to StorageMoverAuditLogs with cost and basic logs support indicators. This enables governance and auditing for Storage Mover resources.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-storagemover-storagemovers-logs

- **Azure Monitor log analytics queries by tables**

  Added a QuantumProviderAccountMessageAuditLogs section with sample queries for operations over 24 hours, failed operations over 7 days, and upcoming scheduled windows. These examples accelerate analysis and operational triage.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/queries-by-table

- **SigninLogs**

  Added ClientSessionId and RootActorID fields to enrich sign-in records. These additions improve correlation across client sessions and enhance actor attribution for investigations.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/signinlogs

- **Azure Monitor Logs table feature support reference**

  Added QuantumProviderAccountMessageAuditLogs to the table feature matrix. This increases discoverability and clarifies feature support for the new table.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables-features