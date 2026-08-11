# Azure Monitor
**Date created:** 2026-08-01 UTC  
**Tags:** Administration, AI, Analytics, Monitoring  

## Major Changes

- **What's new in Azure Monitor documentation**

  Expanded the July–June 2026 roundup with major updates across agents, Application Insights, containers, data collection, fundamentals, health models, logs, metrics, virtual machines, alerts, and platform diagnostics. Highlights include retirements and migration guidance (for Diagnostics extension, Container Insights auth, and VM Dependency Agent), new and GA capabilities (OTLP ingestion, autoinstrumentation metrics, metrics export, SLIs), and previews (Fabric mirroring, multi-stage transformations, advanced platform metrics). It also adds new tutorials, governance and billing clarifications, and broader guidance for exporting, protected tables, and health rollups to help teams plan migrations and adopt new capabilities.

  https://learn.microsoft.com/en-us/azure/azure-monitor/fundamentals/whats-new

## Moderate Changes

- **Azure Monitor health model concepts (preview)**

  Updated dynamic thresholds guidance by removing the Lookback window parameter so only Sensitivity is configurable. This simplifies setup and focuses tuning on how aggressively the model reacts to baseline deviations.

  https://learn.microsoft.com/en-us/azure/azure-monitor/health-models/concepts

- **Log data ingestion time in Azure Monitor | Microsoft Docs**

  Removed the Auxiliary tier warning about rejecting API calls with TimeGenerated values spanning more than 30 minutes. This lifts a prior constraint, allowing broader time ranges per call.

  https://learn.microsoft.com/en-us/azure/azure-monitor/logs/data-ingestion-time

- **Azure Monitor Logs**

  Added Export job (preview) to the table plan comparison with support for Analytics and Basic, but not Auxiliary. Also clarified regional availability, noting Auxiliary generally matches Log Analytics regions except for Qatar Central, helping plan deployments and exports.

  https://learn.microsoft.com/en-us/azure/azure-monitor/logs/data-platform-logs

- **Ingest events from Azure Event Hubs into Azure Monitor Logs (Preview)**

  Added availability constraints and deployment guidance, including a requirement to create the data collection endpoint in the same region as the workspace and clearer limits (for example, 64 KB message size). Updated destination table guidance, renamed Known issues to Considerations, and introduced Alternative solutions (such as AMA, Azure Monitor pipeline, Logs Ingestion API, Logic Apps, or deploying in another region) to unblock ingestion when capacity is constrained.

  https://learn.microsoft.com/en-us/azure/azure-monitor/logs/ingest-logs-event-hub

- **Logs Ingestion API in Azure Monitor**

  Removed the Auxiliary tier warning limiting TimeGenerated timestamps to a 30‑minute range per API call. This change removes a previous ingestion restriction for broader data submit scenarios.

  https://learn.microsoft.com/en-us/azure/azure-monitor/logs/logs-ingestion-api-overview

- **Supported metrics - Microsoft.MachineLearningServices/workspaces/onlineEndpoints/deployments**

  Set DS Export availability to No for several utilization and latency metrics. This clarifies export capabilities and prevents relying on unsupported data export paths for these metrics.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-machinelearningservices-workspaces-onlineendpoints-deployments-metrics

- **Move a Log Analytics workspace in Azure Monitor**

  Clarified that moving a workspace across regions requires creating a new workspace and provided guidance for migrating to availability zone support. Added related content for cross-region relocation to help plan compliant, low-risk moves.

  https://learn.microsoft.com/en-us/azure/azure-monitor/logs/move-workspace

- **Connect self-managed Prometheus to Azure Monitor managed service for Prometheus**

  Corrected minimum Prometheus versions for authentication: system-assigned managed identity requires 3.5.0, and Microsoft Entra workload identity requires 3.7.0. This ensures configurations meet the supported versions for reliable connectivity.

  https://learn.microsoft.com/en-us/azure/azure-monitor/metrics/prometheus-remote-write

- **Restore logs in Azure Monitor**

  Documented a new limitation: restores are supported only for tables on the Analytics or Basic plans, not Auxiliary. This helps plan table placement and recovery strategies accordingly.

  https://learn.microsoft.com/en-us/azure/azure-monitor/logs/restore

- **Tutorial: Configure signals in an Azure Monitor health model (preview)**

  Adjusted dynamic thresholds setup to remove the Lookback window, leaving Sensitivity as the control. This streamlines configuration and clarifies how to tune anomaly detection behavior.

  https://learn.microsoft.com/en-us/azure/azure-monitor/health-models/tutorial-signals