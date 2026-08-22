# Azure Monitor
**Date created:** 2026-08-22 UTC  
**Tags:** Analytics, Configuration, Deprecation, Guidance, Identity, Monitoring, Performance, Security, Troubleshooting  

## New Articles

- **Supported metrics - Microsoft.AzureStackHCI/edgeMachines**
  
  Introduced a new metrics reference for Azure Stack HCI edge machines, grouped under Errors, Saturation, and Traffic. The page details metric names, units, aggregations, 1-minute granularity, and rich dimensions such as device, direction, EdgeMachineName, region, protocol, and mountpoint. This helps operators monitor disk, filesystem, and network health consistently and wire metrics into alerts and exports.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-azurestackhci-edgemachines-metrics

- **Supported metrics - Microsoft.Network/expressRouteLags**
  
  Added a metrics reference for ExpressRoute Link Aggregation Groups (LAGs). The content lists available metrics (for example, light levels, admin state, throughput) with units, dimensions, time grains, default aggregations, and diagnostic export support. This enables more granular monitoring of LAG health and capacity for network reliability and throughput planning.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-network-expressroutelags-metrics

- **Supported log categories - Microsoft.Peering/peeringServices**
  
  Published a new logging reference introducing operational and prefixValidation categories for Peering Services. The page clarifies export costs and lack of support for basic logs and ingestion-time transformations, and links to guidance for streaming, analysis, and summaries. This makes it easier to enable and use logs for peering validation and operations.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-peering-peeringservices-logs

- **Supported metrics - Microsoft.Storage/contextCaches/contextCacheContainers**
  
  Added a metrics reference for Storage context cache containers, covering latency (lookup, read, write) and traffic (hit rate, read/write TPM). Each metric documents units, aggregations, provider/model dimensions, 1-minute time grain, and diagnostic export availability. These metrics help assess cache performance and optimize cache-aware workloads.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-storage-contextcaches-contextcachecontainers-metrics

- **Azure Monitor Logs reference - PaymentHsmHardwareOperationAuditLogs**
  
  Introduced a new table reference for auditing hardware operations on Azure Payment HSM partitions. The schema includes fields for Atalla audit data, signed binary logs, certificate publishing, versioning, identifiers, operation outcomes, and standard Azure Monitor metadata. This enables rigorous traceability and compliance reporting for Payment HSM activities.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/paymenthsmhardwareoperationauditlogs

## Major Changes

- **Understand autoscale settings in Azure Monitor**
  
  Clarified that autoscale cooldown is evaluated per rule, not globally. Updated the scaleAction cooldown description and evaluation logic, and rewrote examples to show independent cooldowns for scale-in and scale‑out. Noted that updating an autoscale setting resets cooldown state and that capacity adjustments to new profile bounds aren’t subject to metric-rule cooldowns, with concurrent behavior dependent on the target resource provider.

  https://learn.microsoft.com/en-us/azure/azure-monitor/autoscale/autoscale-understanding-settings

- **Application Insights availability tests**
  
  Announced retirement of URL ping tests on September 30, 2026, with guidance to migrate to standard tests. Documented differences (for example, headers, bodies, TLS/SSL checks), billing implications, and that creating a standard test doesn’t modify existing ping tests or migrate alert rules. Updated prerequisites, Resource Graph queries, and corrected a PowerShell script parameter to streamline discovery and migration.

  https://learn.microsoft.com/en-us/azure/azure-monitor/app/availability

- **Manage access to Azure Monitor workspaces**
  
  Expanded access control mode documentation with tabbed guidance across portal, Azure CLI, PowerShell, and ARM templates. Added portal steps, a properties screenshot, and explicit commands to set properties.metrics.enableAccessUsingResourcePermissions. Clarified semantics: true uses resource/workspace permissions and false requires workspace permissions, improving governance and rollout confidence.

  https://learn.microsoft.com/en-us/azure/azure-monitor/metrics/azure-monitor-workspace-manage-access

- **Supported Resource log categories for Azure Monitor**
  
  Refreshed supported resources by removing Microsoft.Devices provisioningServices, adding Microsoft.Network expressRouteLags metrics, introducing Microsoft.Peering/peeringServices logs, adding Microsoft.Storage contextCaches/contextCacheContainers metrics, and adding Microsoft.AzureStackHCI edgeMachines metrics. These updates align the reference with current platform coverage and ensure accurate planning for logging and metrics.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/logs-index

- **Supported metrics - Microsoft.Cache/redisEnterprise**
  
  Updated the Cache Latency metric to measure in microseconds and changed the unit from MilliSeconds to Count. This correction improves accuracy and consistency for latency analysis and alert tuning.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-cache-redisenterprise-metrics

- **Supported log categories - Microsoft.DBforPostgreSQL/flexibleServers**
  
  Standardized category names to compact identifiers across PostgreSQL Flexible Server logs (for example, PostgreSQLFlexDatabaseXacts, PostgreSQLFlexPGBouncer, PostgreSQLFlexQueryStoreRuntime). No changes to export costs, target tables, or transformation support. The clearer naming improves configuration accuracy and query consistency.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-dbforpostgresql-flexibleservers-logs

- **Supported metrics - Microsoft.DocumentDB/DatabaseAccounts**
  
  Deprecated legacy metrics (DataUsage, IndexUsage) and introduced a new SLI category with V2 metrics (DataUsageV2, DocumentCountV2, IndexUsageV2). Updated units, dimensions, aggregations, and time grains to reflect the new model. This shifts monitoring to service-level indicators that offer more reliable capacity and usage visibility.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-documentdb-databaseaccounts-metrics

- **Supported metrics - Microsoft.Monitor/pipelineGroups**
  
  Reorganized metrics into Export, Ingestion, Persistent storage, Processing, and Runtime categories and added new signals (for example, logs pending export, accepted, rejected, dropped, storage utilization, processing duration, processor I/O). Renamed export metrics (for example, exported_log_records) and revised dimensions (adding signal and outcome), and updated DS Export flags. Removed preview labels and confirmed runtime metrics’ exportability, enabling more complete end-to-end pipeline health monitoring.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-monitor-pipelinegroups-metrics

- **Supported metrics - Microsoft.StorageCache/amlFilesystems**
  
  Significantly expanded metrics to include Auto Importer and Manual Importer counts (files, directories, symlinks, blobs, conflicts, errors) with a phase dimension. Added client average read/write latency and MDT/OST latency metrics, and aligned units and aggregations across latency measures. These additions improve observability of HPC cache workflows and performance bottlenecks.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-storagecache-amlfilesystems-metrics

## Moderate Changes

- **Autoscale diagnostics**
  
  Clarified cooldown evaluation: lastScaleActionTime tracks the most recent action, cooldown aligns to the candidate rule’s configured value, and the rule is skipped if evaluated before its cooldown ends. This improves accuracy when diagnosing autoscale behavior during profile cool-down periods.

  https://learn.microsoft.com/en-us/azure/azure-monitor/autoscale/autoscale-diagnostics

- **Get started with autoscale in Azure**
  
  Rewrote cooldown guidance to emphasize per‑rule evaluation and how rules with different cooldowns can become eligible at different times. Retained the default five-minute cooldown purpose to prevent repeated scaling on the same condition.

  https://learn.microsoft.com/en-us/azure/azure-monitor/autoscale/autoscale-get-started

- **Configure autoscale using PowerShell**
  
  Clarified ScaleActionCooldown as the minimum time before the same rule can trigger another scale, with cooldowns evaluated per rule. Removed an example-based explanation to reduce ambiguity.

  https://learn.microsoft.com/en-us/azure/azure-monitor/autoscale/autoscale-using-powershell

- **Azure Monitor supported metrics by resource type**
  
  Updated index entries to remove Microsoft.Devices provisioningServices, add Microsoft.Network expressRouteLags, introduce Microsoft.Peering/peeringServices logs, and add Microsoft.Storage contextCaches/contextCacheContainers and Microsoft.AzureStackHCI edgeMachines metrics. Keeps the reference in sync with current platform capabilities.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/metrics-index

- **Supported log categories - Microsoft.AgFoodPlatform/farmBeats**
  
  Standardized log category names to concatenated identifiers (for example, ApplicationAuditLogs, FarmManagementLogs). Improves consistency for configuration and querying.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-agfoodplatform-farmbeats-logs

- **Supported log categories - Microsoft.ApiManagement/service**
  
  Renamed category labels to canonical identifiers (for example, DeveloperPortalAuditLogs, GatewayLlmLogs, GatewayLogs, GatewayMCPLogs, WebSocketConnectionLogs). Aligns naming with actual category identifiers without functional changes.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-apimanagement-service-logs

- **Supported log categories - Microsoft.ApiManagement/service/workspaces**
  
  Renamed “Gateway logs for API Management workspaces” to “GatewayLogs.” Streamlines category naming for workspace scenarios.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-apimanagement-service-workspaces-logs

- **Supported log categories - Microsoft.App/managedEnvironments**
  
  Standardized category names to specific identifiers (for example, AppEnvSessionConsoleLogs, AppEnvSessionLifeCycleLogs, ContainerAppHTTPLogs). Ensures the labels match identifier format used in configuration and queries.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-app-managedenvironments-logs

- **Supported log categories - Microsoft.AppPlatform/spring**
  
  Normalized category names by removing spaces (for example, ApplicationConsole, BuildLogs, ContainerEventLogs, IngressLogs, SystemLogs). Supports consistent diagnostics configuration.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-appplatform-spring-logs

- **Supported log categories - Microsoft.Attestation/attestationProviders**
  
  Updated category names to canonical identifiers: AuditEvent, NotProcessed, Operational. Enhances clarity and alignment with log identifiers.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-attestation-attestationproviders-logs

- **Supported log categories - microsoft.avs/privateClouds**
  
  Renamed “VMware Syslog” to “vmwaresyslog.” Aligns documentation with the category identifier.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-avs-privateclouds-logs

- **Supported log categories - Microsoft.Batch/batchaccounts**
  
  Standardized category names: AuditLog and ServiceLog. Reduces confusion when setting diagnostic categories and writing queries.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-batch-batchaccounts-logs

- **Supported log categories - microsoft.botservice/botservices**
  
  Renamed the ABSBotRequests category label to “BotRequest.” Improves consistency with the associated table.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-botservice-botservices-logs

- **Supported logs - Microsoft.Cdn/edgeactions**
  
  Standardized category names to ServiceLog and UserLog. Simplifies category selection and log parsing.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-cdn-edgeactions-logs

- **Supported log categories - Microsoft.Cdn/profiles/endpoints**
  
  Replaced a descriptive label with the identifier “CoreAnalytics.” Aligns the category with platform naming.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-cdn-profiles-endpoints-logs

- **Supported log categories - Microsoft.Cdn/profiles**
  
  Unified category names by removing spaces: AzureCdnAccessLog, FrontDoorAccessLog, FrontDoorHealthProbeLog, FrontDoorWebApplicationFirewallLog. Improves predictability across configurations.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-cdn-profiles-logs

- **Supported log categories - Microsoft.CognitiveServices/accounts**
  
  Updated to formal identifiers (for example, Audit, AzureOpenAIRequestUsage, ManagedNetworkEvent, RequestResponse, Trace). Facilitates accurate diagnostics configuration and querying.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-cognitiveservices-accounts-logs

- **Supported log categories - microsoft.community/communityTrainings**
  
  Renamed categories to DataPlaneException and DataPlaneLog. Standardizes naming to identifier format.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-community-communitytrainings-logs

- **Supported log categories - Microsoft.ConfidentialLedger/Ledgers**
  
  Updated names to transactionlogs and userdefinedlogs. Aligns identifiers with the platform without changing functionality.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-confidentialledger-ledgers-logs

- **Supported log categories - Microsoft.ContainerService/fleets**
  
  Standardized Kubernetes-related categories to canonical forms (for example, kube-apiserver, kube-audit, kube-controller-manager, kube-scheduler). Improves cross-service consistency for container fleet logging.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-containerservice-fleets-logs

- **Supported log categories - Microsoft.ContainerService/managedClusters**
  
  Updated Kubernetes categories to standardized identifiers (for example, cluster-autoscaler, kube-apiserver, kube-audit-admin) and replaced “Node Auto Provisioning” with “karpenter-events.” Aligns AKS logging with current component terminology.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-containerservice-managedclusters-logs

- **Supported log categories - Microsoft.Dashboard/grafana**
  
  Renamed categories to GrafanaAlertAuthFailure, GrafanaLoginEvents, and GrafanaUsageInsightsEvents. Supports consistent identification and filtering in Log Analytics.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-dashboard-grafana-logs

- **Supported metrics - Microsoft.Dashboard/grafana**
  
  Added NetworkBytesReceived and NetworkBytesTransmitted metrics with Bytes units, multiple aggregations, ContainerName dimension, and 1-minute granularity. These metrics enable visibility into Grafana network usage for capacity planning and troubleshooting.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-dashboard-grafana-metrics

- **Supported log categories - Microsoft.Databricks/workspaces**
  
  Normalized category labels to concise identifiers (for example, accounts, clusters, sqlanalytics) without changing mappings. Improves consistency across entries and queries.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-databricks-workspaces-logs

- **Supported log categories - Microsoft.DataFactory/factories**
  
  Standardized category names to canonical identifiers (for example, ActivityRuns, PipelineRuns, TriggerRuns, and SSIS/Airflow entries). Simplifies configuration and reduces naming ambiguity.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-datafactory-factories-logs

- **Supported log categories - Microsoft.DataLakeAnalytics/accounts**
  
  Updated category names (for example, Audit, ConfigurationChange, JobEvent, JobInfo, Requests). Aligns with standardized naming patterns across services.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-datalakeanalytics-accounts-logs

- **Supported log categories - Microsoft.DataProtection/BackupVaults**
  
  Renamed categories to AddonAzureBackupJobs, AddonAzureBackupPolicy, AddonAzureBackupProtectedInstance, and CoreAzureBackup. Makes category selection consistent across backup services.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-dataprotection-backupvaults-logs

- **Supported log categories - Microsoft.DataReplication/replicationVaults**
  
  Standardized categories (for example, HealthEvents, JobEvents, ProtectedItems, ReplicationExtensions, ReplicationPolicies, ReplicationVaults). Enhances clarity and accuracy for replication diagnostics.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-datareplication-replicationvaults-logs

- **Supported log categories - Microsoft.DBforMariaDB/servers**
  
  Updated category names to MySqlAuditLogs and MySqlSlowLogs. Aligns MariaDB diagnostics categories with MySQL naming.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-dbformariadb-servers-logs

- **Supported log categories - Microsoft.DBforMySQL/flexibleServers**
  
  Renamed categories to MySqlAuditLogs and MySqlSlowLogs. Improves consistency across MySQL offerings.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-dbformysql-flexibleservers-logs

- **Supported log categories - Microsoft.DBforMySQL/servers**
  
  Standardized the categories to MySqlAuditLogs and MySqlSlowLogs. Ensures consistent configuration and queries for MySQL server diagnostics.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-dbformysql-servers-logs

- **Supported log categories - Microsoft.DBForPostgreSQL/serverGroupsv2**
  
  Renamed “PostgreSQL Server Logs” to “PostgreSQLLogs.” Aligns with other PostgreSQL category updates.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-dbforpostgresql-servergroupsv2-logs

- **Supported log categories - Microsoft.DesktopVirtualization/hostpools**
  
  Updated multiple categories to concise identifiers (for example, AutoscaleEvaluationPooled, ConnectionGraphicsData, MultiLinkAdd, NetworkData, SessionHostManagement). Improves readability and consistency for AVD diagnostics.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-desktopvirtualization-hostpools-logs

- **Supported log categories - Microsoft.DevCenter/devcenters**
  
  Standardized category names (AgentHealthStatus, ConnectionEvent, DataplaneAuditEvent, ResourceOperation, Usage). Facilitates straightforward category selection and querying.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-devcenter-devcenters-logs

- **Supported log categories - Microsoft.Devices/IotHubs**
  
  Normalized category names by removing spaces and preview labels (for example, C2DCommands, DeviceStreams, DistributedTracing). Reduces confusion and ensures identifiers match configuration expectations.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-devices-iothubs-logs

- **Supported metrics - Microsoft.Devices/IotHubs**
  
  Added the “Number of throttled requests” metric (throttledRequests) with a ThrottleType dimension, 1-minute granularity, and alert support. This aids in detecting rate limiting and tuning client behavior and capacity.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-devices-iothubs-metrics

- **Supported log categories - Microsoft.Discovery/bookshelves**
  
  Renamed “Audit Logs” to “BookshelvesAudit.” Aligns category naming with platform identifiers.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-discovery-bookshelves-logs

- **Supported log categories - Microsoft.Discovery/supercomputers**
  
  Renamed “Audit Logs” to “SupercomputersAudit.” Improves consistency across Discovery resources.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-discovery-supercomputers-logs

- **Supported log categories - Microsoft.Edge/diagnostics**
  
  Updated names to UserAudits and UserDiagnostics. Clarifies category purpose and matches identifiers.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-edge-diagnostics-logs

- **Supported log categories - Microsoft.EventGrid/domains**
  
  Renamed categories to DataPlaneRequests, DeliveryFailures, and PublishFailures. Standardizes identifiers across Event Grid domain diagnostics.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-eventgrid-domains-logs

- **Supported log categories - Microsoft.EventGrid/topics**
  
  Renamed categories to DataPlaneRequests, DeliveryFailures, and PublishFailures. Aligns topic diagnostics with domain category naming.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-eventgrid-topics-logs

- **Supported log categories - Microsoft.EventHub/Namespaces**
  
  Normalized identifiers (for example, ApplicationMetricsLogs, ArchiveLogs, AutoScaleLogs, CustomerManagedKeyUserLogs, DiagnosticErrorLogs, EventHubVNetConnectionEvent, KafkaCoordinatorLogs, KafkaUserErrorLogs, OperationalLogs, RuntimeAuditLogs). Ensures category names accurately reflect underlying identifiers.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-eventhub-namespaces-logs

- **Supported log categories - Microsoft.HardwareSecurityModules/cloudHsmClusters**
  
  Renamed categories to HsmOperations and HsmServiceOperations. Improves clarity and uniformity.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-hardwaresecuritymodules-cloudhsmclusters-logs

- **Supported log categories - Microsoft.HealthcareApis/workspaces/dicomservices**
  
  Updated categories to AuditLogs and DiagnosticLogs. Provides clear, standardized identifiers.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-healthcareapis-workspaces-dicomservices-logs

- **Supported log categories - Microsoft.HorizonDB/clusters**
  
  Replaced human-readable names with identifier-style categories (for example, HorizonDBServerLogs, HorizonDBQueryStoreRuntimeStats). Aligns HorizonDB logging with the standard format.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-horizondb-clusters-logs

- **Supported log categories - microsoft.insights/autoscalesettings**
  
  Removed spaces in category names: AutoscaleEvaluations and AutoscaleScaleActions. Matches the canonical identifiers used by diagnostics.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-insights-autoscalesettings-logs

- **Supported metrics - microsoft.keyvault/managedhsms**
  
  Added EKM Proxy Availability (EkmProxyAvailability) to measure connectivity between Managed HSM and the EKM proxy. Includes relevant dimensions, 1-minute grain, and multiple aggregations, enabling proactive monitoring of key operations routing.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-keyvault-managedhsms-metrics

- **Supported log categories - Microsoft.KeyVault/vaults**
  
  Updated categories to AuditEvent and AzurePolicyEvaluationDetails. Provides accurate identifiers for configuration and analysis.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-keyvault-vaults-logs

- **Supported log categories - Microsoft.Logic/automationProjects/applications**
  
  Renamed “Workflow runtime diagnostic events” to “WorkflowRuntime.” Aligns Logic Apps categories across resources.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-logic-automationprojects-applications-logs

- **Supported log categories - Microsoft.Logic/automationProjects**
  
  Renamed “Workflow runtime diagnostic events” to “WorkflowRuntime.” Ensures consistent naming in automation projects.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-logic-automationprojects-logs

- **Supported log categories - Microsoft.Logic/IntegrationAccounts**
  
  Updated to IntegrationAccountTrackingEvents. Standardizes the integration account diagnostics category.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-logic-integrationaccounts-logs

- **Supported log categories - Microsoft.ManagedNetworkFabric/networkDevices**
  
  Renamed categories to PascalCase identifiers (for example, BfdStateUpdates, ComponentStateUpdates, InterfaceGeneralEvents). Improves consistency across network fabric diagnostics.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-managednetworkfabric-networkdevices-logs

- **Supported log categories - Microsoft.NetApp/netAppAccounts/capacityPools**
  
  Renamed “Capacity Pool Autoscaled” to “Autoscale.” Aligns with category identifier conventions.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-netapp-netappaccounts-capacitypools-logs

- **Supported log categories - Microsoft.NetworkAnalytics/DataProducts**
  
  Standardized multiple categories (for example, DatabaseQuery, IngestionDelete, IngestionRead, ReadStorage). Aligns identifiers across network analytics data products.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-networkanalytics-dataproducts-logs

- **Supported log categories - Microsoft.Network/azureFirewalls**
  
  Updated categories to standardized AZFW* identifiers and aligned DNS-related entries (for example, AZFWDnsAdditional, AZFWFqdnResolveFailure). This ensures category names mirror actual table mappings and simplifies query authoring.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-network-azurefirewalls-logs

- **Supported log categories - Microsoft.NetworkCloud/bareMetalMachines**
  
  Renamed security and system categories to concise identifiers (for example, DefenderSecurity, SecurityWarning, SyslogCritical). Provides uniform naming across log rows.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-networkcloud-baremetalmachines-logs

- **Supported log categories - Microsoft.NetworkCloud/clusterManagers**
  
  Renamed categories to CloudInitDiagnostics and ClusterManagerDeployOrUpgradeLogs. Clarifies category intent and aligns with identifier patterns.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-networkcloud-clustermanagers-logs

- **Supported log categories - Microsoft.NetworkCloud/clusters**
  
  Standardized categories (for example, CustomerContainerLogs, IdracContainerLogs, KubeAPIAudit, PlatformOperations, VMOrchestrationLogs). Ensures consistent cluster diagnostics naming.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-networkcloud-clusters-logs

- **Supported log categories - Microsoft.NetworkCloud/kubernetesClusters**
  
  Renamed “Tenant Operation Logs” to “TenantOperationTraces.” Aligns tenant diagnostics naming.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-networkcloud-kubernetesclusters-logs

- **Supported log categories - Microsoft.NetworkCloud/storageAppliances**
  
  Renamed categories to StorageApplianceAlert, StorageApplianceAudit, and StorageApplianceLogs. Improves naming clarity and alignment.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-networkcloud-storageappliances-logs

- **Supported log categories - Microsoft.Network/dnsResolverPolicies**
  
  Renamed “DNS Response” to “DnsResponse.” Matches the actual identifier for DNSQueryLogs.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-network-dnsresolverpolicies-logs

- **Supported log categories - Microsoft.Network/expressRouteCircuits**
  
  Renamed “Peering Route Table Logs” to “PeeringRouteLog.” Aligns the category with current naming.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-network-expressroutecircuits-logs

- **Supported log categories - Microsoft.Network/frontdoors**
  
  Updated to FrontdoorAccessLog and FrontdoorWebApplicationFirewallLog. Ensures identifiers match configuration options.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-network-frontdoors-logs

- **Supported log categories - Microsoft.NetworkFunction/azureTrafficCollectors**
  
  Renamed categories (for example, ATCMicrosoftPeeringMetadata, ATCPrivatePeeringMetadata, ExpressRouteCircuitIpfix). Improves clarity for traffic collector diagnostics.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-networkfunction-azuretrafficcollectors-logs

- **Supported log categories - Microsoft.Network/networkManagers**
  
  Removed spaces to match actual identifiers: ConnectivityConfigurationChange, NetworkGroupMembershipChange, RuleCollectionChange. Aligns categories with platform usage.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-network-networkmanagers-logs

- **Supported log categories - Microsoft.Network/networksecuritygroups**
  
  Standardized to NetworkSecurityGroupEvent, NetworkSecurityGroupFlowEvent, and NetworkSecurityGroupRuleCounter. Ensures consistent NSG diagnostics naming.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-network-networksecuritygroups-logs

- **Supported log categories - Microsoft.Network/networkSecurityPerimeters**
  
  Replaced descriptive names with standardized NSP identifiers (for example, NspCrossPerimeterInboundAllowed, NspPublicOutboundPerimeterRulesDenied). Supports precise filtering and policy analysis.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-network-networksecurityperimeters-logs

- **Supported log categories - Microsoft.Network/networkSecurityPerimeters/profiles**
  
  Renamed to canonical identifiers (NSPInboundAccessAllowed/Denied, NSPOutboundAccessAllowed/Denied). Streamlines diagnostics setup for profiles.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-network-networksecurityperimeters-profiles-logs

- **Supported log categories - microsoft.network/p2svpngateways**
  
  Updated to GatewayDiagnosticLog, IKEDiagnosticLog, and P2SDiagnosticLog. Unifies VPN logging categories.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-network-p2svpngateways-logs

- **Supported log categories - Microsoft.Network/publicIPAddresses**
  
  Standardized DDoS-related categories to DDoSMitigationFlowLogs, DDoSMitigationReports, and DDoSProtectionNotifications. Enhances consistency across DDoS diagnostics.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-network-publicipaddresses-logs

- **Supported log categories - Microsoft.Network/publicIPPrefixes**
  
  Updated DDoS categories to DDoSMitigationFlowLogs, DDoSMitigationReports, and DDoSProtectionNotifications. Aligns IP prefix diagnostics with public IP updates.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-network-publicipprefixes-logs

- **Supported log categories - microsoft.network/virtualnetworkgateways**
  
  Standardized categories (GatewayDiagnosticLog, IKEDiagnosticLog, P2SDiagnosticLog, RouteDiagnosticLog, TunnelDiagnosticLog). Simplifies VNet gateway diagnostics configuration.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-network-virtualnetworkgateways-logs

- **Supported log categories - microsoft.network/vpngateways**
  
  Updated to GatewayDiagnosticLog, IKEDiagnosticLog, RouteDiagnosticLog, and TunnelDiagnosticLog. Ensures consistent naming across VPN gateways.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-network-vpngateways-logs

- **Supported log categories - MICROSOFT.OPENENERGYPLATFORM/ENERGYSERVICES**
  
  Standardized many categories to concise identifiers and removed “WellDelivery Service Logs.” These changes bring consistency to diagnostics across Open Energy Platform services.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-openenergyplatform-energyservices-logs

- **Supported log categories - Microsoft.OpenLogisticsPlatform/Workspaces**
  
  Updated categories to SupplyChainEntityOperations and SupplyChainEventLogs. Aligns naming with identifier conventions.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-openlogisticsplatform-workspaces-logs

- **Supported log categories - Microsoft.ProviderHub/providerMonitorSettings**
  
  Standardized to UserRPHttpIncomingRequests, UserRPHttpOutgoingRequests, and UserRPProvisioningOperations. Improves consistency for provider diagnostics.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-providerhub-providermonitorsettings-logs

- **Supported log categories - microsoft.purview/accounts**
  
  Renamed categories: DataSensitivityLogEvent, ScanStatusLogEvent, and Security. Clarifies category purposes and improves alignment.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-purview-accounts-logs

- **Supported log categories - Microsoft.Quantum/providerAccounts**
  
  Updated to AuditEvent and Operational. Standardizes categories used in quantum provider accounts.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-quantum-provideraccounts-logs

- **Supported log categories - Microsoft.Quantum/workspaces**
  
  Renamed “Audit Logs” to “AuditEvent” for QuantumWorkspaceJobAuditLogs. Ensures consistency across quantum workspace diagnostics.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-quantum-workspaces-logs

- **Supported log categories - Microsoft.RecoveryServices/Vaults**
  
  Standardized many backup and site recovery categories to match table identifiers (for example, AddonAzureBackupAlerts, AzureBackupOperations, AzureSiteRecoveryJobs, CoreAzureBackup). Improves mapping clarity and query reliability.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-recoveryservices-vaults-logs

- **Supported log categories - Microsoft.RedHatOpenShift/hcpOpenShiftClusters**
  
  Standardized Kubernetes component categories to canonical identifiers (for example, capi-provider, cloud-controller-manager, cluster-autoscaler, kube-apiserver, kube-audit-admin). Aligns OpenShift diagnostics with Kubernetes norms.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-redhatopenshift-hcpopenshiftclusters-logs

- **Supported log categories - Microsoft.Relay/namespaces**
  
  Updated to HybridConnectionsEvent and VNetAndIPFilteringLogs. Aligns relay diagnostics with Event Hubs/Service Bus naming.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-relay-namespaces-logs

- **Supported log categories - Microsoft.Security/antiMalwareSettings**
  
  Renamed “AntimalwareScanResults” to “ScanResults.” Harmonizes antimalware category naming.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-security-antimalwaresettings-logs

- **Supported log categories - Microsoft.Security/defenderForStorageSettings**
  
  Renamed “AntimalwareScanResults” to “ScanResults.” Maintains consistency with antimalware category updates.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-security-defenderforstoragesettings-logs

- **Supported log categories - Microsoft.ServiceBus/Namespaces**
  
  Standardized multiple categories by removing spaces and special characters (for example, ApplicationMetricsLogs, DataDRLogs, DiagnosticErrorLogs, OperationalLogs, RuntimeAuditLogs, VNetAndIPFilteringLogs). Enables predictable configuration and filters.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-servicebus-namespaces-logs

- **Supported log categories - Microsoft.ServiceNetworking/trafficControllers**
  
  Renamed to TrafficControllerAccessLog and TrafficControllerFirewallLog. Clarifies AGC category roles for access vs. firewall.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-servicenetworking-trafficcontrollers-logs

- **Supported log categories - Microsoft.SignalRService/WebPubSub**
  
  Standardized categories to ConnectivityLogs, HttpRequestLogs, and MessagingLogs. Improves discoverability and query composition for Web PubSub diagnostics.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-signalrservice-webpubsub-logs

- **Supported log categories - Microsoft.SignalRService/WebPubSub/replicas**
  
  Standardized categories to ConnectivityLogs, HttpRequestLogs, and MessagingLogs. Ensures parity between replica and parent resources.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-signalrservice-webpubsub-replicas-logs

- **Supported log categories - Microsoft.Sql/managedInstances/databases**
  
  Updated category names to QueryStoreRuntimeStatistics, QueryStoreWaitStatistics, and SQLInsights. Aligns identifiers with AzureDiagnostics expectations.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-sql-managedinstances-databases-logs

- **Supported log categories - Microsoft.Sql/managedInstances**
  
  Renamed categories to DevOpsOperationsAudit, ResourceUsageStats, and SQLSecurityAuditEvents. Streamlines SQL MI diagnostics naming.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-sql-managedinstances-logs

- **Supported log categories - Microsoft.Sql/servers/databases**
  
  Standardized multiple categories (for example, AutomaticTuning, DatabaseWaitStatistics, DevOpsOperationsAudit, DmsWorkers, ExecRequests, RequestSteps, SQLInsights, SqlRequests, SQLSecurityAuditEvents). Improves consistency across SQL Database diagnostics.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-sql-servers-databases-logs

- **Supported log categories - Microsoft.StandbyPool/standbycontainergrouppools**
  
  Renamed categories to ContainerGroupExecution and ContainerGroupRequest. Improves clarity for standby container group diagnostics.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-standbypool-standbycontainergrouppools-logs

- **Supported log categories - Microsoft.StorageCache/caches**
  
  Updated category labels to AscCacheOperationEvent, AscUpgradeEvent, and AscWarningEvent. Aligns cache diagnostics naming.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-storagecache-caches-logs

- **Supported log categories - Microsoft.StorageMover/storageMovers**
  
  Renamed to CopyLogsFailed and JobRunLogs. Clarifies the types of Storage Mover operational logs.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-storagemover-storagemovers-logs

- **Supported log categories - Microsoft.Storage/storageAccounts/blobServices**
  
  Standardized categories to StorageDelete, StorageRead, and StorageWrite. Simplifies filtering and alerting on storage operations.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-storage-storageaccounts-blobservices-logs

- **Supported log categories - Microsoft.Synapse/workspaces/kustoPools**
  
  Updated categories to PascalCase (for example, DataOperation, FailedIngestion, IngestionBatching, SucceededIngestion, TableDetails, TableUsageStatistics). Aligns Synapse Kusto diagnostics with naming patterns.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-synapse-workspaces-kustopools-logs

- **Supported log categories - Microsoft.Synapse/workspaces**
  
  Standardized multiple categories (for example, BuiltinSqlReqsEnded, GatewayApiRequests, IntegrationActivityRuns, SQLSecurityAuditEvents, SynapseRbacOperations). Enhances coherence across Synapse workspace diagnostics.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-synapse-workspaces-logs

- **Supported log categories - Microsoft.Synapse/workspaces/scopePools**
  
  Renamed categories to ScopePoolScopeJobsEnded and ScopePoolScopeJobsStateChange. Aligns scope pools logging with canonical identifiers.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-synapse-workspaces-scopepools-logs

- **Supported log categories - Microsoft.Synapse/workspaces/sqlPools**
  
  Standardized to DmsWorkers, ExecRequests, RequestSteps, SqlRequests, and SQLSecurityAuditEvents. Provides alignment across Synapse SQL pool diagnostics.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-synapse-workspaces-sqlpools-logs

- **NetworkAccessTraffic**
  
  Added new columns: ApplicationObjectId, AppLoginDeviceId, AppLoginUserId, and ConnectorGroupId. These fields apply to Private Access traffic and are null for other transaction types, enabling richer identity and connector analytics for Private Access scenarios.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/networkaccesstraffic

- **Supported log categories - NGINX.NGINXPLUS/nginxDeployments**
  
  Standardized categories to NginxLogs, NginxSecurityLogs, and NginxUpstreamUpdateLogs. Improves clarity for NGINX diagnostics setup.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/nginx-nginxplus-nginxdeployments-logs

- **Supported log categories - Oracle.Database/autonomousDatabases**
  
  Removed the “Events” suffix across multiple categories (for example, Backup, Creation, Critical, Delete, Information, Restore, Update). Aligns Oracle diagnostics with concise identifier naming.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/oracle-database-autonomousdatabases-logs

- **Supported log categories - Oracle.Database/cloudVmClusters**
  
  Standardized category names (for example, AddVm, Backup, Creation, Critical, Delete, Health, Information, Restore, TerminateVm, Update). Improves clarity and consistency; note that “Critical” appears twice in the source list.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/oracle-database-cloudvmclusters-logs

- **Supported log categories - Oracle.Database/dbSystems**
  
  Updated categories to concise names (Backup, Creation, Critical, Delete, Health, Information, Restore, Update). Enhances uniformity across Oracle Database resources.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/oracle-database-dbsystems-logs

- **Supported log categories - Oracle.Database/exadbVmClusters**
  
  Standardized category names (AddVm, Creation, Critical, Delete, Information, Maintenance, TerminateVm, Update). Aligns ExaDB VM clusters diagnostics with identifier-based naming.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/oracle-database-exadbvmclusters-logs

- **Azure Monitor Logs table feature support reference**
  
  Added PaymentHsmHardwareOperationAuditLogs to the feature support matrix with no feature flags indicated for Basic, Auxiliary, or DCR transformation. This provides visibility into the new table’s feature support status for planning and governance.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables-features

- **Supported log categories - Microsoft.Web/sites**
  
  Standardized categories to canonical identifiers (for example, AppServiceAntivirusScanAuditLogs, AppServiceAppLogs, AppServiceAuditLogs, AppServiceAuthenticationLogs, WorkflowRuntime). Removes preview labels where applicable and aids consistent diagnostics setup.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-web-sites-logs

- **Supported log categories - Microsoft.Web/sites/slots**
  
  Updated to standardized category names (for example, AppServiceAntivirusScanAuditLogs, AppServiceAppLogs, AppServiceAuditLogs, AppServiceConsoleLogs, AppServiceHTTPLogs, FunctionAppLogs). Ensures parity between site and slot diagnostics.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-web-sites-slots-logs

- **Supported log categories - Microsoft.Web/staticsites**
  
  Renamed to StaticSiteDiagnosticLogs and StaticSiteHttpLogs. Clarifies static site diagnostics categories.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-web-staticsites-logs

- **Supported log categories - Microsoft.ZeroTrustSegmentation/segmentationManagers**
  
  Updated categories to Request and ZTSJobStatus. Streamlines logging identifiers for Zero Trust Segmentation workflows.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/microsoft-zerotrustsegmentation-segmentationmanagers-logs

## Minor Changes