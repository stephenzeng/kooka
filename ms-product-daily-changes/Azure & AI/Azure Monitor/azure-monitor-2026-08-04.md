# Azure Monitor
**Date created:** 2026-08-04 UTC  
**Tags:** Analytics, Monitoring, Security  

## New Articles

- **Azure Monitor Logs reference - DevOpsOperationsAudit**
  
  Introduced a new Azure Monitor Logs table that captures Azure SQL audit operations with extensive context on actions, principals, sessions, database scope, execution metrics, and sensitivity details. The schema and feature flags are documented, along with links to sample queries. This enables auditing and compliance teams to query a dedicated dataset for DevOps-related SQL activity.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/devopsoperationsaudit

- **Supported log categories - Microsoft.HardwareSecurityModules/paymentHsmClusters**
  
  Added a new reference for resource logs on Payment HSM clusters, including the Hsm Hardware Operations category. The page clarifies export costs and that basic logs and ingestion-time transformations aren’t supported. This helps administrators configure diagnostics and route HSM logs appropriately.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-hardwaresecuritymodules-paymenthsmclusters-logs

- **Supported log categories - Microsoft.Logic/automationProjects/applications**
  
  Published supported logs for Logic automation project applications, listing Workflow runtime diagnostic events with export details. It specifies unsupported features like basic logs and ingestion transformations. This helps teams enable diagnostics for app-level automation workflows.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-logic-automationprojects-applications-logs

- **Supported metrics - Microsoft.Logic/automationProjects/applications**
  
  Added a metrics reference for Logic automation project applications, documenting two billing metrics and their properties (unit, aggregation, time grain, and export). This enables cost tracking and alerting for application-level automation usage and retention.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-logic-automationprojects-applications-metrics

- **Supported log categories - Microsoft.Logic/automationProjects**
  
  Introduced the logs reference for Logic automation projects, listing Workflow runtime diagnostic events and export behavior. Guidance links help teams set up and use these logs for troubleshooting and governance.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-logic-automationprojects-logs

- **Supported metrics - Microsoft.Logic/automationProjects**
  
  Published metrics for Logic automation projects, including billing and resource consumption (vCPU and memory) with 1‑minute granularity and export support. These metrics support usage analysis, budget controls, and operational alerting.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-logic-automationprojects-metrics

- **Supported metrics - Microsoft.ResourceBuilder/workspaces**
  
  Added metrics for Resource Builder workspaces covering job and pipeline execution counts and latency, with dimensions for state and names. This helps operators monitor pipeline reliability and performance trends.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-resourcebuilder-workspaces-metrics

- **Supported log categories - Oracle.Database/exascaleDbStorageVaults**
  
  Introduced resource log categories for Oracle Exascale DB Storage Vaults (Creation, Delete, Update). Export support and limitations are documented, enabling teams to capture lifecycle events for governance and auditing.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/oracle-database-exascaledbstoragevaults-logs

- **Azure Monitor Logs reference - QuantumProviderAccountDeviceOperationLogs**
  
  Added a new operational telemetry table for Azure Quantum Provider Account devices, tracking operation lifecycle events tied by CorrelationId. The schema covers identifiers, versions, durations, results, and billing-related fields and supports Auxiliary/Lake. This enables detailed troubleshooting and analysis of device operations.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/quantumprovideraccountdeviceoperationlogs

## Major Changes

- **ASimAgentEventLogs**
  
  Expanded the schema with new entity key columns for actors, applications, devices, sources, and targets. These additions improve entity mapping and correlation across agent event data, enabling more accurate investigations and detections.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/asimagenteventlogs

- **ASimAuthenticationEventLogs**
  
  Added multiple columns to capture acting/target applications and systems, device keys, and additional user identifiers. This enriches authentication events with consistent entity keys, improving cross-table correlation and threat hunting.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/asimauthenticationeventlogs

- **ASimFileEventLogs**
  
  Introduced entity keys for applications, users, devices, files, processes, and systems, plus support for additional user IDs. The richer schema strengthens linkage between file operations and related entities to aid forensic analysis.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/asimfileeventlogs

- **ASimNetworkSessionLogs**
  
  Added source and destination application/system/user entity keys and additional identifier fields, plus a general AdditionalEntities column. This enables full-path session correlation across users, devices, and applications for network investigations.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/asimnetworksessionlogs

- **ASimProcessEventLogs**
  
  Expanded the schema with acting/target process keys, parent process, device key, and additional user identifiers. These changes improve lineage and entity correlation for process events, supporting advanced detection and triage.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/asimprocesseventlogs

- **AzureMonitorPipelineLogErrors**
  
  Enabled Auxiliary/Lake support and added ComponentName and EventName columns. This broadens analytics options and improves filtering and attribution for pipeline error diagnostics.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/azuremonitorpipelinelogerrors

- **CloudAuditEvents**
  
  Revised the schema to add multi-cloud identifiers and context (Account, AuditSource, AwsResourceName, AzureResourceId, GcpFullResourceName), standardized ISP casing, and removed CloudResourceId. The update provides clearer resource attribution across clouds for audit analytics.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/cloudauditevents

- **CloudStorageAggregatedEvents**
  
  Renamed IpAddress to IPAddress and added Md5Hashes for accessed resources. The change standardizes naming and enables hash-based analysis of content access.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/cloudstorageaggregatedevents

- **DisruptionAndResponseEvents**
  
  Renamed DataSources to DataSource and added MachineGroup and ReportId. These changes improve RBAC scoping and event traceability for disruption reports.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/disruptionandresponseevents

- **SentinelBehaviorEntities**
  
  Changed the ApplicationId column type from string to int. This breaking-type adjustment enhances data consistency and performance for queries relying on numeric operations.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/sentinelbehaviorentities

- **Supported metrics for Microsoft.Cache/redisEnterprise**
  
  Overhauled Redis Enterprise metrics: converted key counters to rates/sec, adjusted aggregations to emphasize averages, updated units, and refined latency semantics. Added preview shard-level metrics with rich dimensions for deeper cache insight. These updates improve accuracy of performance monitoring and enable granular shard diagnostics.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-cache-redisenterprise-metrics

## Moderate Changes

- **AgentsInfo**
  
  Enabled Basic table support. This lowers cost options for retaining and querying agent metadata.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/agentsinfo

- **AlertEvidence**
  
  Added AzureResourceId, AzureResourceType, and AzureSubscriptionId fields. These enrich alerts with cloud resource context, improving triage and automation.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/alertevidence

- **ASimAlertEventLogs**
  
  Added entity-focused columns including AdditionalEntities and keys for device, file, process, and user. This enhances correlation across alert events and related entities.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/asimalerteventlogs

- **ASimAuditEventLogs**
  
  Added entity keys for acting/target applications and systems, device keys, and additional user identifiers. The changes strengthen correlation and context in audit investigations.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/asimauditeventlogs

- **ASimDhcpEventLogs**
  
  Added AdditionalEntities plus keys for device, source system, and source user identifiers. This improves tracking DHCP activity across entities for network troubleshooting.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/asimdhcpeventlogs

- **ASimDnsActivityLogs**
  
  Added entity keys for device, systems, and source process, plus additional user IDs. This supports more precise DNS activity correlation and attribution.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/asimdnsactivitylogs

- **ASimRegistryEventLogs**
  
  Added keys for acting/parent processes, device, and additional actor user IDs. This improves lineage and actor attribution in registry change analysis.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/asimregistryeventlogs

- **ASimUserManagementActivityLogs**
  
  Added keys for acting applications, devices, source systems, and target/actor user identifiers. These updates enhance traceability of user lifecycle operations.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/asimusermanagementactivitylogs

- **ASimWebSessionLogs**
  
  Added source/destination application, system, user, and device keys, plus AdditionalEntities. This enables multi-entity correlation for web session investigations.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/asimwebsessionlogs

- **CloudHsmHardwareOperationAuditLogs**
  
  Enabled Basic table support and marked availability in LogManagement. This broadens cost-effective retention and simplifies discovery.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/cloudhsmhardwareoperationauditlogs

- **CloudProcessEvents**
  
  Added ReportId to uniquely identify each event. This improves deduplication and cross-system tracking.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/cloudprocessevents

- **DeviceInfo**
  
  Added ConnectivityType to indicate how a device connects. This helps segment devices by network path for monitoring and policy.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/deviceinfo

- **DynamicEventCollection**
  
  Added initiating process and parent creation time fields. This provides temporal context for process-driven collections.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/dynamiceventcollection

- **EmailUrlInfo**
  
  Added UrlChainId and UrlChainPosition to model URL chains. This supports better tracking of multi-hop links in messages.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/emailurlinfo

- **Use Dashboards with Grafana for Azure Virtual Machines**
  
  Added an at-scale OpenTelemetry VM dashboard option and guidance for monitoring multiple VMs in a workspace. Instructions clarify prerequisites and include a new screenshot to accelerate setup.

  https://learn.microsoft.com/en-us/azure/azure-monitor/visualize/grafana-azure-virtual-machines

- **IdentityAccountInfo**
  
  Added SourceProviderRiskLevelDetails for richer risk context from the source. This enables more granular security scoring and filtering.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/identityaccountinfo

- **Supported Resource log categories for Azure Monitor**
  
  Expanded supported categories and resources, including paymentHsmClusters, Logic automationProjects/apps, ResourceBuilder workspaces, and Oracle exascale DB storage vaults. This helps teams discover new telemetry surfaces for monitoring.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/logs-index

- **MessageEvents**
  
  Added fields for message and thread classification, and renamed ThreadSubtype to ThreadSubType. This improves consistency and supports more precise filtering.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/messageevents

- **Azure Monitor supported metrics by resource type**
  
  Added entries for Hardware Security Modules, Logic automation projects, ResourceBuilder workspaces, and Oracle exascale storage vaults. This update clarifies what metrics are available across new resource types.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/metrics-index

- **Metrics experience for virtual machines in Azure Monitor**
  
  Clarified multi-VM capabilities for the OpenTelemetry-based experience, highlighting an at-scale default-metrics Grafana dashboard. Guidance distinguishes when to use logs-based VM insights for broader multi-VM analytics and consolidates limitations.

  https://learn.microsoft.com/en-us/azure/azure-monitor/vm/metrics-opentelemetry-guest

- **Supported metrics for Microsoft.App/sessionpools**
  
  Added Session API request count and average response time metrics with dimensions and export support. This enables monitoring API volume and latency for session pools.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-app-sessionpools-metrics

- **Log Analytics tables for microsoft.azurestackhci/clusters**
  
  Perf now supports the Basic Logs plan. This reduces cost for performance data retention on Azure Stack HCI clusters.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/microsoft-azurestackhci-clusters

- **Supported metrics for Microsoft.Batch/batchaccounts**
  
  Expanded aggregations for numerous resource allocation metrics to include Average, Minimum, and Maximum. This enables richer analysis beyond totals, improving capacity planning.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-batch-batchaccounts-metrics

- **Log Analytics tables for microsoft.compute/virtualmachines**
  
  Updated Perf entry to supported/available (Yes). This broadens options for collecting VM performance data.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/microsoft-compute-virtualmachines

- **Log Analytics tables for microsoft.compute/virtualmachinescalesets**
  
  Enabled Perf table support for VM Scale Sets. This allows performance monitoring at scale with cost flexibility.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/microsoft-compute-virtualmachinescalesets

- **Log Analytics tables for microsoft.conenctedvmwarevsphere/virtualmachines**
  
  Marked Perf as supported in the related tables list. This facilitates performance insights for connected VMware VMs.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/microsoft-conenctedvmwarevsphere-virtualmachines

- **Log Analytics tables for microsoft.containerservice/managedclusters**
  
  Enabled data collection for Perf under managedClusters. This supports performance visibility for AKS clusters.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/microsoft-containerservice-managedclusters

- **Supported metrics for Microsoft.ContainerService/managedClusters**
  
  Added the partition dimension to three ETCD metrics. This improves granularity for diagnosing control-plane load.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-containerservice-managedclusters-metrics

- **Supported metrics for Microsoft.DocumentDB/cassandraClusters**
  
  Standardized aggregations across many metrics, largely removing Count and aligning on Average/Minimum/Maximum. This makes trend analysis more consistent across categories.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-documentdb-cassandraclusters-metrics

- **Supported metrics for Microsoft.DocumentDB/DatabaseAccounts**
  
  Expanded or tightened time grain support across many Cosmos DB metrics, adding longer intervals where applicable and constraining certain high-frequency metrics to PT1M. This improves reporting flexibility and performance.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-documentdb-databaseaccounts-metrics

- **Supported metrics for Microsoft.ElasticSan/elasticSans**
  
  Clarified capacity metric definitions, including baseline and provisioned capacity semantics and how snapshots factor into totals. This helps avoid misinterpretation in capacity planning.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-elasticsan-elasticsans-metrics

- **Supported metrics for Microsoft.EventHub/Namespaces**
  
  Expanded aggregations for CaptureBacklog and connection metrics to include Sum, Average, Minimum, and Maximum. This provides more comprehensive operational insights.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-eventhub-namespaces-metrics

- **Log Analytics tables for microsoft.hardwaresecuritymodules/cloudhsmclusters**
  
  Marked CloudHsmHardwareOperationAuditLogs as available in LogManagement. This simplifies discovery and routing for HSM audit data.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/microsoft-hardwaresecuritymodules-cloudhsmclusters

- **Supported log categories - Microsoft.HardwareSecurityModules/cloudHsmClusters**
  
  Added Hsm Hardware Operations to the supported logs table with export and plan details. This enables consistent configuration across HSM offerings.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-hardwaresecuritymodules-cloudhsmclusters-logs

- **Log Analytics tables for microsoft.hybridcontainerservice/provisionedclusters**
  
  Updated Perf capability to Yes. This enables performance monitoring for hybrid container services with cost control.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/microsoft-hybridcontainerservice-provisionedclusters

- **Log Analytics tables for microsoft.kubernetes/connectedclusters**
  
  Marked Perf as supported in resource-specific workspaces. This improves performance visibility for connected Kubernetes clusters.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/microsoft-kubernetes-connectedclusters

- **Supported metrics for Microsoft.MachineLearningServices/workspaces**
  
  Added six toolbox-related metrics with dimensions for toolbox name, version, and status. These help track feature usage and performance of tooling in ML workspaces.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-machinelearningservices-workspaces-metrics

- **Supported metrics for Microsoft.NetworkCloud/bareMetalMachines**
  
  Removed several deprecated CPU and NTP metrics to clean up the list. This reduces confusion and focuses monitoring on supported signals.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-networkcloud-baremetalmachines-metrics

- **Supported log categories - Microsoft.NetworkCloud/clusterManagers**
  
  Added Cloud Init Diagnostic Logs with export and plan details. This supports troubleshooting cluster initialization issues.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-networkcloud-clustermanagers-logs

- **Supported metrics for Microsoft.NetworkCloud/clusterManagers**
  
  Removed the deprecated Cluster Deploy Requests metric. This streamlines dashboards and alerts to active metrics.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-networkcloud-clustermanagers-metrics

- **Supported metrics for Microsoft.NetworkCloud/clusters**
  
  Introduced Kubelet metrics with a new MachineRole dimension and marked older versions as deprecated. Also removed other deprecated metrics. This enables role-aware monitoring and guides migration from legacy signals.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-networkcloud-clusters-metrics

- **Supported metrics for Microsoft.Network/expressRouteCircuits**
  
  Expanded traffic metric aggregations to include Sum, Average, Minimum, and Maximum. This improves analysis for throughput and capacity trends.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-network-expressroutecircuits-metrics

- **Supported metrics for microsoft.network/expressroutegateways**
  
  Added Sum, Minimum, and Maximum aggregations to bits-in/out metrics. This supports broader operational and capacity reporting.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-network-expressroutegateways-metrics

- **Supported metrics for Microsoft.Network/expressRoutePorts**
  
  Removed Count aggregation from bits-in/out metrics, retaining Average/Min/Max. This standardizes rate metric analysis.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-network-expressrouteports-metrics

- **Supported metrics for Microsoft.Network/loadBalancers**
  
  Expanded SNAT port metrics to include Sum, Average, Minimum, and Maximum. This supports better capacity monitoring and alerting.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-network-loadbalancers-metrics

- **Supported metrics for Microsoft.Network/networkinterfaces**
  
  Broadened aggregations across bytes, packets, flow creation, and mirroring counters to include Sum/Average/Min/Max. This enables more flexible performance and reliability analysis.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-network-networkinterfaces-metrics

- **Supported metrics for Microsoft.Network/virtualnetworkappliances**
  
  Expanded all listed metrics to support Sum, Average, Minimum, and Maximum. This provides richer options for capacity planning and SLA reporting.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-network-virtualnetworkappliances-metrics

- **Supported log categories - MICROSOFT.OPENENERGYPLATFORM/ENERGYSERVICES**
  
  Added Seismic DDMS Logs as a supported category. This surfaces new telemetry for specialized energy workloads.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-openenergyplatform-energyservices-logs

- **Supported metrics for MICROSOFT.OPENENERGYPLATFORM/ENERGYSERVICES**
  
  Marked two metrics as Preview in display names without changing technical properties. This sets expectations for maturity while leaving integrations unaffected.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-openenergyplatform-energyservices-metrics

- **Log Analytics tables for microsoft.operationalinsights/workspaces**
  
  Updated Perf to available/enabled in LogManagement. This simplifies finding and using performance data in workspaces.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/microsoft-operationalinsights-workspaces

- **Supported log categories - Microsoft.RedHatOpenShift/hcpOpenShiftClusters**
  
  Added Cluster API Provider and Cluster Autoscaler categories with export details. This enhances observability for Red Hat OpenShift control-plane components.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-redhatopenshift-hcpopenshiftclusters-logs

- **Supported metrics for Microsoft.ServiceBus/Namespaces**
  
  Expanded CPU and memory aggregations to include Sum/Average/Min/Max. This improves resource usage analysis for premium namespaces.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-servicebus-namespaces-metrics

- **Supported metrics for Microsoft.Sql/managedInstances**
  
  Added new metrics (workers percentage, log rate limit, log rate) and clarified descriptions for several existing metrics. These updates improve performance tuning and capacity planning for managed instances.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-sql-managedinstances-metrics

- **Log Analytics tables for microsoft.sql/servers**
  
  Added DevOpsOperationsAudit to the tables list with reference linkage. This exposes a new audit dataset within LogManagement for SQL servers.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/microsoft-sql-servers

- **Supported metrics for Microsoft.Storage/storageAccounts/blobServices**
  
  Expanded time grains for capacity metrics to include PT6H, PT12H, and P1D. This enables coarser aggregation for long-term trending.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-storage-storageaccounts-blobservices-metrics

- **Supported metrics for Microsoft.Storage/storageAccounts/fileServices**
  
  Added PT6H, PT12H, and P1D time grains to capacity metrics. This supports lower-cost, long-horizon capacity reporting.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-storage-storageaccounts-fileservices-metrics

- **Supported metrics for Microsoft.Storage/storageAccounts**
  
  Expanded capacity metric time grains and added a new MigrationProgress transaction metric with export support. These changes improve redundancy migration tracking and long-term capacity analysis.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-storage-storageaccounts-metrics

- **Supported metrics for Microsoft.Storage/storageAccounts/objectReplicationPolicies**
  
  Tightened time grains for pending replication metrics to PT1M only. This focuses on high-resolution monitoring where it matters most.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-storage-storageaccounts-objectreplicationpolicies-metrics

- **Supported metrics for Microsoft.Storage/storageAccounts/queueServices**
  
  Added PT6H, PT12H, and P1D time grains for queue capacity metrics. This enables trend analysis without excessive data volume.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-storage-storageaccounts-queueservices-metrics

- **Supported metrics for Microsoft.Storage/storageAccounts/tableServices**
  
  Expanded time grains for table capacity metrics to include PT6H, PT12H, and P1D. This supports cost-effective historical reporting.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-storage-storageaccounts-tableservices-metrics

- **Log Analytics tables for microsoft.zerotrustsegmentation/segmentationmanagers**
  
  Enabled Basic logs support for ZTSGraph and ZTSMetadata tables. This reduces cost barriers for zero-trust segmentation analytics.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/microsoft-zerotrustsegmentation-segmentationmanagers

- **MPCAuditLogs**
  
  Enabled Basic table support. This offers a lower-cost option for storing and querying MPC audit data.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/mpcauditlogs

- **Supported metrics for Oracle.Database/exadbVmClusters**
  
  Updated REST API names to slash format and enabled DS Export for many metrics across availability, saturation, and traffic. This simplifies API integration and allows exporting a broader set of Oracle metrics.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/oracle-database-exadbvmclusters-metrics

- **Perf**
  
  Enabled Basic table support. This opens cost-optimized retention for performance counters across resources.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/perf

- **PreAuthenticationDiscoveryLogs**
  
  Enabled Basic table support. This reduces costs for storing pre-authentication discovery telemetry.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/preauthenticationdiscoverylogs

- **Azure Monitor log analytics queries by tables**
  
  Added a DevOpsOperationsAudit section with a reference link and a sample query. This helps users quickly start querying the new audit table.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/queries-by-table

- **Azure Monitor Logs table feature support reference**
  
  Updated the support matrix to add Basic logs for several tables (including AgentsInfo, CloudHsmHardwareOperationAuditLogs, MPCAuditLogs, Perf, PreAuthenticationDiscoveryLogs, ZTSGraph, ZTSMetadata) and Auxiliary/Lake for AzureMonitorPipelineLogErrors. Also added new entries for DevOpsOperationsAudit and QuantumProviderAccountDeviceOperationLogs, guiding feature adoption and cost management.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables-features

- **Enable VM monitoring in Azure Monitor**
  
  Corrected the Data Collection Rule example to use an array for streams with Microsoft-OtelPerfMetrics. This ensures configuration aligns with the performanceCountersOTel schema and avoids deployment errors.

  https://learn.microsoft.com/en-us/azure/azure-monitor/vm/vm-enable-monitoring

- **ZTSGraph**
  
  Enabled Basic table support. This provides a lower-cost option for zero-trust graph analytics.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/ztsgraph

- **ZTSMetadata**
  
  Enabled Basic table support. This helps reduce cost for storing zero-trust metadata used in policy and analysis.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/ztsmetadata