# Azure Monitor
**Date created:** 2026-08-15 UTC  
**Tags:** Analytics, Consumption, Deprecation, Guidance, Monitoring, Performance, Security, Troubleshooting  

## New Articles

- **Azure Monitor Logs reference - AGSGrafanaAlertAuthFailure**
  Introduced a new table documenting authentication failures during alert rule evaluation for Azure Managed Grafana. The page details table attributes, billing and API support, and a full column schema to help investigate alert execution issues. This enables faster troubleshooting of failed alerts and improved operational visibility.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/agsgrafanaalertauthfailure

- **Azure Monitor Logs reference - DragonCopilot**
  Added a new audit and activity log table for Microsoft Dragon Copilot across healthcare workflows. The reference includes table capabilities (Basic/Auxiliary/Lake support and DCR transformations) and a comprehensive schema covering access, session, policy, and clinical data fields. This helps organizations track usage, troubleshoot issues, and meet governance requirements.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/dragoncopilot

- **Azure Monitor tables for microsoft.horizondb/clusters**
  Published a new resource-type page that introduces the AzureMetrics table for Microsoft.HorizonDB/clusters. It outlines categories, solution mapping, and Basic Logs support, plus a link to example queries. This helps teams discover metrics coverage and plan HorizonDB monitoring.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/microsoft-horizondb-clusters

- **Supported log categories - Microsoft.HorizonDB/clusters**
  Added a resource logs reference for HorizonDB clusters listing all supported log categories, export considerations, and Basic Logs support. Cross-references to supported metrics and “next steps” help teams onboard logs efficiently. This clarifies the full logging surface for HorizonDB.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-horizondb-clusters-logs

- **Example log table queries for QuantumProviderAccountDeviceOperationLogs**
  Introduced example KQL queries for Azure Quantum device operations. Samples include pass-rate analysis using terminal statuses and average duration by device and operation, focused on accurate outcomes. This accelerates insights into reliability and performance of device operations.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/queries/quantumprovideraccountdeviceoperationlogs

- **Azure Monitor Logs reference - Windows365CheckpointLogs**
  Added a new table for Cloud PC checkpoint events, documenting attributes and schema. The reference enables tracking of checkpoint progress and results across Windows 365 connections. It supports Basic and Auxiliary/Lake plans for cost-optimized retention.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/windows365checkpointlogs

- **Azure Monitor Logs reference - Windows365ConnectionErrorLogs**
  Published a new table for Windows 365 connection error events with documented attributes and schema. The table centralizes error diagnostics to simplify root-cause analysis. Support for cost-optimized plans makes ongoing monitoring economical.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/windows365connectionerrorlogs

- **Azure Monitor Logs reference - Windows365ConnectionLogs**
  Added a connection activity log table for Windows 365, including user, device, gateway, and session details. The schema supports tracing connection flows and correlating issues across services. This strengthens end-to-end observability for Cloud PC scenarios.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/windows365connectionlogs

- **Azure Monitor Logs reference - Windows365NetworkLogs**
  Introduced a network performance telemetry table for Windows 365, covering bandwidth and latency estimates per connection. Attributes and schema are fully documented with support for cost-optimized plans. This enables proactive monitoring of Cloud PC network health.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/windows365networklogs

## Major Changes

- **GCPCloudSQL**
  Expanded coverage to ingest broader Cloud SQL logs, including admin/management audit logs, data-access audit logs (pgAudit DDL/DML), and engine/session logs. Added rich payload columns (ProtoPayload, JsonPayload, Labels, MethodName, TextPayload) and multiple pgAudit fields to improve fidelity. Marked many legacy fields as Deprecated and directed users to retrieve details from ProtoPayload, improving consistency and forward compatibility.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/gcpcloudsql

- **Supported metrics - Microsoft.ContainerService/managedClusters**
  Added a new API Server metric “API Request Concurrency” to monitor flow control execution capacity. Introduced a new Scheduler (PREVIEW) category with “Pod Scheduling Rate” to observe scheduling performance. These metrics enhance visibility into Kubernetes control plane throughput and scheduling efficiency.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-containerservice-managedclusters-metrics

- **Supported metrics - Microsoft.MachineLearningServices/workspaces**
  Removed six toolbox-related metrics for AI Agents, streamlining the supported metrics set. This reduces confusion around deprecated signals and aligns monitoring with current product capabilities. Users should update dashboards and alerts to avoid referencing removed metrics.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-machinelearningservices-workspaces-metrics

- **Supported metrics - Microsoft.ManagedNetworkFabric/networkDevices**
  Added four port-channel metrics to aggregate member interface telemetry and a new SLI category with device connectivity and operational health metrics. Guidance recommends Maximum aggregation to interpret health states over time. These additions improve insight into link aggregation performance and device health for fabric operations.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-managednetworkfabric-networkdevices-metrics

- **Example log table queries for PGSQLServerLogs**
  Expanded troubleshooting content with multiple new KQL examples for errors, deadlocks, restarts, connections, authentication failures, lock contention, autovacuum, and audit events. Each section includes alerting guidance to operationalize detection. This accelerates incident triage and improves operational readiness for PostgreSQL workloads.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/queries/pgsqlserverlogs

- **Azure Monitor Logs table feature support reference**
  Updated the support matrix to remove ADGSyslogEvent, add AGSGrafanaAlertAuthFailure and DragonCopilot, and enable Basic Logs for QuantumProviderAccountDeviceOperationLogs. Added four Windows 365 tables with Basic and Auxiliary/Lake support. These changes clarify feature availability and help plan cost and governance for new tables.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables-features

- **Azure Monitor Resource log / log analytics tables by resource group**
  Expanded the index to include QuantumProviderAccountDeviceOperationLogs and a new HorizonDB section with AzureMetrics. Added four Windows 365 log tables and removed ADGSyslogEvent. This makes discovery of new logs easier and keeps the index aligned with current resource coverage.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables-index

## Moderate Changes

- **CrowdStrikeAlerts**
  Added a CrowdStrikeDomain column to record the configured CrowdStrike host/domain on each record. This enables multi-tenant or multi-domain differentiation in queries and dashboards.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/crowdstrikealerts

- **CrowdStrikeAuditEvents**
  Introduced the CrowdStrikeDomain column to capture the source host/domain for each event. This supports clearer segmentation and correlation across multiple CrowdStrike connections.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/crowdstrikeauditevents

- **CrowdStrikeCases**
  Added the CrowdStrikeDomain column to identify the configured CrowdStrike host/domain per case. This improves filtering and reporting across distinct CrowdStrike environments.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/crowdstrikecases

- **CrowdStrikeHosts**
  Included a CrowdStrikeDomain field to tag each record with the source host/domain. This helps distinguish hosts when aggregating data from multiple connections.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/crowdstrikehosts

- **CrowdStrikeIncidents**
  Added a CrowdStrikeDomain column to track the configured host/domain for every incident. This enhances multi-environment incident analysis and reporting.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/crowdstrikeincidents

- **CrowdStrikeVulnerabilities**
  Introduced a CrowdStrikeDomain column to differentiate hosts/domains across vulnerability data. This improves scoping and correlation in vulnerability investigations.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/crowdstrikevulnerabilities

- **Supported Resource log categories for Azure Monitor**
  Updated the Microsoft.HorizonDB entry to list supported logs for clusters and added a link to the new HorizonDB logs page. This clarifies logging coverage for HorizonDB resources.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/logs-index

- **Azure Monitor supported metrics by resource type**
  Added Microsoft.HorizonDB with metrics and logs for clusters and aligned its listing with new log support. This ensures consistent discovery of HorizonDB telemetry across logs and metrics.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/metrics-index

- **Supported log categories - Microsoft.Dashboard/grafana**
  Added a “Grafana Alert Authentication Failure Events” category with cost and support details. This enables targeted export and monitoring of authentication failures in alert evaluation.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-dashboard-grafana-logs

- **Supported metrics - Microsoft.DocumentDB/DatabaseAccounts**
  Removed the IsLeakedPartition dimension from the Index Usage metric. Update any filters or groupings that rely on this dimension to avoid broken charts or alerts.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-documentdb-databaseaccounts-metrics

- **Log Analytics tables for microsoft.intune/operations**
  Added four Windows 365 tables covering checkpoint events, connection errors, connection lifecycle, and network performance for Cloud PC. This expands observability for Windows 365 and supports cost-optimized plans.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/microsoft-intune-operations

- **Supported metrics - microsoft.kubernetes/connectedClusters**
  Introduced the Cluster Connectivity Status metric to indicate whether Arc-enabled Kubernetes clusters are connected. Use it to alert on connectivity losses that affect management operations.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-kubernetes-connectedclusters-metrics

- **Supported log categories - Microsoft.ManagedNetworkFabric/networkDevices**
  Added an “Interface General Events” category. This broadens visibility into interface-level events for fabric devices.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-managednetworkfabric-networkdevices-logs

- **Supported metrics - Microsoft.Network/connections**
  Added per-device ingress and egress throughput metrics for Multicloud Interconnect. These signals enable granular traffic monitoring and capacity planning.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-network-connections-metrics

- **Supported metrics - Microsoft.Network/expressRouteCircuits**
  Added QoS drop-rate metrics for Multicloud Interconnect at various time grains with DS Export. These help quantify packet drops and validate QoS behavior across circuits.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-network-expressroutecircuits-metrics

- **Log Analytics tables for microsoft.network/networkvirtualappliances**
  Removed the ADGSyslogEvent table from the applicable tables list. Update any documentation or expectations that referenced this table for this resource type.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/microsoft-network-networkvirtualappliances

- **Log Analytics tables for microsoft.quantum/provideraccounts**
  Added the QuantumProviderAccountDeviceOperationLogs table with operational telemetry details and Basic Logs support. This enables monitoring and analysis of device operations, including correlation via shared IDs.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/microsoft-quantum-provideraccounts

- **Supported metrics - Microsoft.Search/searchServices**
  Clarified the “Compute units used” metric units (micro-CU-hours), added guidance to convert to CU-hours, and noted deprecation of the Status filter. Added a new ResourceKind dimension to improve segmentation.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-search-searchservices-metrics

- **Example log table queries for PGSQLAutovacuumStats**
  Added example queries for bloat ratio, vacuum statistics, and analyze statistics with recommended time binning. These help tune maintenance and assess table health over time.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/queries/pgsqlautovacuumstats

- **Example log table queries for PGSQLPgStatActivitySessions**
  Added queries for longest sessions, longest transactions, and sessions with long queries, with filters to exclude system contexts. Use these to identify resource-intensive sessions and address performance bottlenecks.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/queries/pgsqlpgstatactivitysessions

- **Example log table queries for PGSQLQueryStoreRuntime**
  Added queries to find queries exceeding execution thresholds, top slow queries, and execution count trends. Notes clarify Query Store aggregation and plan availability to ensure accurate analysis.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/queries/pgsqlquerystoreruntime

- **Example log table queries for PGSQLQueryStoreWaits**
  Added wait event trends and top wait events queries with recommended binning and labeling. These examples help pinpoint dominant waits impacting performance.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/queries/pgsqlquerystorewaits

- **QuantumProviderAccountDeviceOperationLogs**
  Updated table attributes to specify resource type, enable Basic Logs support, and add sample queries. This improves discoverability and lowers cost for telemetry retention.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/quantumprovideraccountdeviceoperationlogs

- **Azure Monitor log analytics queries by tables**
  Removed the ADGSyslogEvent section and added QuantumProviderAccountDeviceOperationLogs with pass-rate and duration queries. Also introduced duplicate bullets in several PostgreSQL sections; review content to avoid confusion.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/queries-by-table

- **SalesforceAuditTrail**
  Added a SalesforceDomain column to identify the configured Salesforce host/domain per record. This supports multi-domain analysis and clearer correlation.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/salesforceaudittrail

- **SalesforceLoginHistory**
  Introduced the SalesforceDomain column to tag records with the source Salesforce host/domain. This enables precise filtering and reporting across tenants or domains.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/salesforceloginhistory

- **StorageBlobLogs**
  Expanded schema with CopyDestinationArmId, EncryptionKeyTypeOfBlob, RequestRegion, and TrafficClassification. These fields improve traceability of copy operations, encryption context, request origin, and traffic source classification.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/storagebloblogs

- **Azure Monitor Log Analytics log tables organized by category**
  Updated the index to add PreAuthenticationDiscoveryLogs, QuantumProviderAccountDeviceOperationLogs, and four Windows 365 tables; removed ADGSyslogEvent. This keeps category navigation aligned with newly supported tables.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables-category

- **What's new in Azure Monitor documentation**
  Added an August 2026 entry highlighting enhancements to Auxiliary/Lake table plans, including expanded table support, plan switching, and sovereign cloud availability. Linked to feature comparisons, configuration guidance, and a detailed announcement.

  https://learn.microsoft.com/en-us/azure/azure-monitor/fundamentals/whats-new