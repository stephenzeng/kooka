# Azure Monitor
**Date created:** 2026-09-01 UTC  
**Tags:** Analytics, Configuration, Guidance, Monitoring, Troubleshooting  

## New Articles

- **Supported log categories - Oracle.Database/goldenGateDeployments**

  Introduced a new reference page detailing the supported log categories for Oracle GoldenGate deployments in Azure Monitor. It lists available categories (Backup, Creation, Critical, Delete, Information, Maintenance, Restore, Update), notes export cost applicability, and clarifies that the basic logs plan and ingestion-time transformations aren’t supported. The page also links to the related supported metrics page and next steps for deeper monitoring guidance.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-logs/oracle-database-goldengatedeployments-logs

- **Supported metrics - Oracle.Database/goldenGateDeployments**

  Added a comprehensive metrics reference for Oracle GoldenGate deployments, covering Availability, Latency, and Saturation metrics with names, units, default aggregations, dimensions, and a 1-minute time grain. It clarifies that data export via data sources isn’t available and outlines key metrics such as deployment health, path statuses, lag metrics, and resource utilization. The page includes links to guidance on metrics export, diagnostic settings, retention, and to the corresponding supported logs page.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/oracle-database-goldengatedeployments-metrics

## Moderate Changes

- **Create or edit a log search alert rule**

  Updated guidance for 1-minute frequency log alert rules: when an AzureDiagnostics category has an equivalent resource-specific table, query the resource-specific table (for example, AZFWThreatIntel) to improve performance and reliability. Added a reference to diagnostics mode documentation and reorganized notes about empty tables without changing their meaning.

  https://learn.microsoft.com/en-us/azure/azure-monitor/alerts/alerts-create-log-alert-rule

- **Get started with autoscale in Azure**

  Reworked the walkthrough to focus on configuring autoscale for an App Service plan, including default CPU-based scale-out, complementary scale-in, instance limits, and both recurring and date-based schedules. Clarified portal navigation, highlighted that autoscale scope applies to the entire App Service plan and that App Service automatic scaling is a separate option, and noted that predictive autoscale and scale-in policy guidance applies to Virtual Machine Scale Sets. Expanded explanations for Run history and JSON views and refreshed related content.

  https://learn.microsoft.com/en-us/azure/azure-monitor/autoscale/autoscale-get-started

- **Supported Resource log categories for Azure Monitor**

  Expanded coverage for Oracle.Database to include GoldenGate deployments, adding the appropriate entries and links for resource log categories. This improves discoverability of log options when monitoring GoldenGate resources.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/logs-index

- **Azure Monitor supported metrics by resource type**

  Updated the Oracle.Database section to include goldenGateDeployments, adding the relevant supported metrics and log references. This enables accurate metric selection for GoldenGate monitoring scenarios.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/metrics-index

- **PaymentHsmHardwareOperationAuditLogs**

  Updated the table reference to indicate support for Auxiliary (Lake) table capabilities. This enables downstream analytics scenarios that depend on Lake-integrated logs.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/paymenthsmhardwareoperationauditlogs

- **Azure Monitor Logs table feature support reference**

  Updated the feature matrix to show that PaymentHsmHardwareOperationAuditLogs now supports the Auxiliary (Lake) logs plan. This clarifies deployment choices for customers standardizing on Lake-based log storage.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables-features