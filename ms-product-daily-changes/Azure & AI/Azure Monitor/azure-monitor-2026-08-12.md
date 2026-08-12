# Azure Monitor
**Date created:** 2026-08-12 UTC  
**Tags:** Analytics, Automation, Best Practices, Billing, Compliance, Configuration, Deprecation, Get Started, Governance, Guidance, Monitoring, Security, Troubleshooting  

## Major Changes

- **Best practices for autoscale**

  Expanded guidance to reflect autoscale support across more Azure services and added a pointer to the current supported list. Clarified diagnostics metric aggregation (statistic and timeAggregation) with allowed values and an example of how evaluations work. Reworked multiple-rule behavior to explicitly document scale-out (any rule) versus scale-in (all rules) logic, with updated queue-length thresholds using instance-normalized counts. Enhanced activity log guidance with flapping event types, recommended actions, alerting/notification advice, and added Next steps links.

  https://learn.microsoft.com/en-us/azure/azure-monitor/autoscale/autoscale-best-practices

- **Monitor Azure Monitor workspace metrics ingestion**

  Introduced a comprehensive ingestion limits section with default/maximum values, auto-approval criteria, and when to open support tickets. Updated alerting recommendations (30-minute aggregation, five‑minute evaluation), mapped portal metric names to metric IDs, and clarified portal enablement steps. Adjusted thresholds in ARM/Bicep templates (Active Time Series utilization from 85% to 75%) and improved instructions for requesting higher limits via API, including rules above 2M up to 20M. Refined deployment/verification steps and expanded troubleshooting for API errors.

  https://learn.microsoft.com/en-us/azure/azure-monitor/metrics/azure-monitor-workspace-monitor-ingest-limits

- **Multicloud monitoring with Azure Monitor**

  Reorganized the article around practical scenarios and added a mapping of AWS/GCP services to Azure Monitor capabilities. Strengthened guidance for VMs, Kubernetes, and applications, including Arc, AMA, VM insights, Managed Prometheus, Container insights, and Application Insights SDK usage. Clarified audit collection with first‑party Microsoft Sentinel connectors, expanded custom ingestion options, and added management guidance for non‑Azure machines (Azure Update Manager, Change Tracking and Inventory, Hybrid Runbook Worker). Updated links, terminology, and structure for clarity.

  https://learn.microsoft.com/en-us/azure/azure-monitor/fundamentals/best-practices-multicloud

- **Rule Groups in Azure Monitor Managed Service for Prometheus**

  Significantly expanded guidance for creating and managing rule groups via portal, CLI, PowerShell, ARM, and Bicep, including prerequisites and clearer terminology. Corrected schema/property names and examples, and added navigation for filtering, viewing health states, and bulk deletion. Introduced best practices for scoping rule groups to specific clusters (scopes and clusterName) to control evaluation and reduce noise. Improved instructional flow throughout.

  https://learn.microsoft.com/en-us/azure/azure-monitor/metrics/prometheus-rule-groups

- **Query packs in Azure Monitor Logs**

  Overhauled operations with updated permissions guidance and explicit role assignments, including Log Analytics Contributor at resource group scope. Modernized REST workflows to use Microsoft.OperationalInsights queryPacks with API version 2025-07-01, dedicated payloads, and updated PUT/PATCH endpoints for creating and managing packs and queries. Added CLI token acquisition, refined portal navigation/limits, and clarified property definitions and metadata references.

  https://learn.microsoft.com/en-us/azure/azure-monitor/logs/query-packs

- **Restore logs in Azure Monitor**

  Rewrote the guide to clarify restore behavior, naming requirements (_RST), and when to use restores versus search jobs, with noted Azure Lighthouse limitations. Added prerequisites and detailed, end-to-end examples for CLI, PowerShell, and REST, including required fields and status handling. Expanded guidance for querying restored data, dismissal, and key limitations (range, volume, concurrency, caps). Updated pricing rules and examples, highlighting minimum volume/duration and no query charge.

  https://learn.microsoft.com/en-us/azure/azure-monitor/logs/restore

## Moderate Changes

- **Understand autoscale settings in Azure Monitor**

  Updated scope to highlight support for Virtual Machine Scale Sets and other resources, refreshed ARM examples to apiVersion 2022-10-01, and clarified metricTrigger fields and allowed values (timeGrain, statistic, timeAggregation) including dividePerInstance. Reworked profile guidance with a comparison of Default, Fixed-date, and Recurrence, plus clearer evaluation behavior emphasizing conservative scale-in to prevent flapping.

  https://learn.microsoft.com/en-us/azure/azure-monitor/autoscale/autoscale-understanding-settings

- **Manage an Azure Monitor workspace**

  Added prerequisites for subscription, resource group, and required role assignments. Updated templates to API version 2023-04-03, corrected the delete command to az monitor account delete, and added a verification step to confirm managed resource group removal. Included minor clarifications for access modes and integration examples without changing procedures.

  https://learn.microsoft.com/en-us/azure/azure-monitor/metrics/azure-monitor-workspace-manage

- **Reliability best practices in Azure Monitor**

  Refocused the introduction on minimizing impact during component failures across logs, alerts, virtual machines, and containers, streamlining to the Reliability pillar. Fixed a reference issue and added clarifying lead-ins that stress keeping monitoring available when failures occur.

  https://learn.microsoft.com/en-us/azure/azure-monitor/fundamentals/best-practices-reliability

- **Query container logs in Azure Monitor**

  Clarified prerequisites and updated examples to use ContainerLogV2 with current fields, standardized Kusto code fences, and improved context for lifecycle and event queries. Consolidated system container availability into a parameterized query, corrected variables and parameters, and clarified storage in ContainerLogV2 with improved alerting guidance.

  https://learn.microsoft.com/en-us/azure/azure-monitor/containers/container-insights-log-query

- **Create Diagnostic Settings at Scale by Using Azure Policy and Initiatives**

  Added prerequisites for roles and managed identity permissions needed for deployIfNotExists remediation. Introduced verification steps via portal and Azure CLI to confirm diagnostic settings deployment and clarified custom policy and initiative usage and remediation behavior. Updated terminology and improved wording throughout.

  https://learn.microsoft.com/en-us/azure/azure-monitor/platform/diagnostic-settings-policy

- **Azure Monitor enterprise monitoring architecture**

  Expanded end-to-end reference guidance for data collection across Log Analytics, Azure Monitor workspaces (Prometheus), and platform metrics, including routing for correlation. Clarified alerting design by workspace and subscription, detailed integrations with Microsoft Sentinel and Defender XDR, and provided prescriptive ITSM routing via action groups, secure webhooks, Functions, or Logic Apps. Noted legacy ServiceNow ITSM action deprecation and improved component descriptions and recommendations.

  https://learn.microsoft.com/en-us/azure/azure-monitor/fundamentals/enterprise-monitoring-architecture

- **Detect and analyze anomalies with KQL in Azure Monitor**

  Improved the tutorial with clearer context for Azure Monitor Logs vs. Log Analytics and explicit references to Kusto documentation. Renamed sections around make-series and series_decompose_anomalies(), expanded parameter explanations (including Test_points), and enhanced guidance for interpreting results. Updated root-cause analysis to use diffpatterns() with practical threshold tuning.

  https://learn.microsoft.com/en-us/azure/azure-monitor/logs/kql-machine-learning-azure-monitor

- **Export data from a Log Analytics workspace to a storage account by using Azure Logic Apps**

  Switched the workflow to run hourly and aligned sample KQL and templates with that cadence. Clarified UI labels for classic Consumption versus Standard workflows and corrected connection resource IDs and time range defaults in the template. Refreshed example payloads and provided guidance for adjusting frequency.

  https://learn.microsoft.com/en-us/azure/azure-monitor/logs/logs-export-logic-app

- **Monitor Kubernetes clusters using Azure Monitor and cloud native tools**

  Updated network monitoring to use Virtual Network flow logs with Traffic Analytics and streamlined Prometheus onboarding via remote write to Managed Prometheus. Clarified cost/collection guidance for container logs and Prometheus, refined control plane and activity log recommendations, and expanded troubleshooting and alerts guidance (including PromQL terminology and community rules). Modernized Grafana guidance with Azure Managed Grafana and Azure Monitor dashboards with Grafana public preview.

  https://learn.microsoft.com/en-us/azure/azure-monitor/containers/monitor-kubernetes

- **Manage personal data in Azure Monitor Logs**

  Clarified the Purge API workflow, including polling the x-ms-status-location URL with Get Purge Status after a 202 response. Reinforced planning before collecting personal data and highlighted operational/performance impacts of purge operations. Noted that Basic/Auxiliary plan tables aren’t supported by the query API and to use the Search API.

  https://learn.microsoft.com/en-us/azure/azure-monitor/logs/personal-data-mgmt

- **Connect Grafana to Azure Monitor managed service for Prometheus**

  Added prerequisites and clarified connection options from Azure Managed Grafana, self-managed on Azure VMs, and outside Azure with distinct authentication methods. Recommended using the Azure Monitor Managed Service for Prometheus data source plugin for Grafana 13+, with installation steps including air‑gapped scenarios and required configuration. Expanded steps for enabling Azure Authentication, managed identity, role assignments, and app registration values for data source setup.

  https://learn.microsoft.com/en-us/azure/azure-monitor/metrics/prometheus-grafana

- **Resource Manager template samples for diagnostic settings**

  Added a reference table mapping resource types to their diagnosticSettings resource types to ensure correct provider paths. Renamed a parameter in Azure Data Explorer samples and removed an unnecessary metadata block in Azure SQL Managed Instance templates; other changes were structural.

  https://learn.microsoft.com/en-us/azure/azure-monitor/platform/resource-manager-diagnostic-settings

- **Run Search Jobs in Azure Monitor**

  Expanded examples and clarified parameters across CLI, PowerShell, and REST, and updated REST references to the Azure Monitor API index with a version placeholder. Added an explanation of the provisioningState for search job tables, including when it appears and possible values, with an updated sample response.

  https://learn.microsoft.com/en-us/azure/azure-monitor/logs/search-jobs