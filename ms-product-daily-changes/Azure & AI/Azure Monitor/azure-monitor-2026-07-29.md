# Azure Monitor
**Date created:** 2026-07-29 UTC  
**Tags:** Monitoring, Security  

## Moderate Changes

- **What’s new in Azure Monitor documentation**  
  Announced a new reference that lists all Azure Monitor Logs tables and their support for Basic, Auxiliary/Lake, DCR workspace transformations, and Logs Ingestion API. Terminology is standardized across 900+ table reference articles, and the TOC reflects the new grouping for easier discovery and planning.

  https://learn.microsoft.com/en-us/azure/azure-monitor/fundamentals/whats-new

- **Create and manage action groups in Azure Monitor**  
  Expanded guidance for using Logic Apps with action groups, including an example posting alert notifications to Microsoft Teams and a link to step-by-step customization instructions. This improves clarity on notification types and automations for operational workflows.

  https://learn.microsoft.com/en-us/azure/azure-monitor/alerts/action-groups

- **Recommended alert rules for Kubernetes clusters**  
  Added guidance to route alerts to Microsoft Teams via Logic Apps, with references to configuring action groups and customizing notifications. This helps teams operationalize Kubernetes alerts with collaborative workflows.

  https://learn.microsoft.com/en-us/azure/azure-monitor/containers/kubernetes-metric-alerts

- **Supported KQL features in Azure Monitor transformations**  
  Added an important note that in data collection transformations, parse kind=regex must match the entire input string to populate fields (unlike Log Analytics/Sentinel). Guidance includes extending patterns to end-of-line and an example, plus an alternative using the parse operator, helping reduce parsing errors in transformations.

  https://learn.microsoft.com/en-us/azure/azure-monitor/data-collection/data-collection-transformations-kql

- **Azure Monitor pipeline extension versions**  
  Removed the “Version 1.5.0 - July 22, 2026” section from the version history, including upgrade warnings and release details. This clarifies the currently supported information and avoids confusion about deprecated notes.

  https://learn.microsoft.com/en-us/azure/azure-monitor/data-collection/pipeline-extension-versions

- **Alert (table reference)**  
  Standardized the capabilities section to use “Basic table support,” “Auxiliary/Lake table support,” and “DCR workspace transformation support,” and added “Ingestion API support.” This improves consistency and helps determine supported ingestion and transformation options for the table.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/alert

- **AppRequests (table reference)**  
  Updated capability labels to the new taxonomy and added the Ingestion API support row. This clarifies ingestion and transformation paths when designing data pipelines that rely on application request telemetry.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/apprequests

- **AzureActivity (table reference)**  
  Adopted standardized capability fields and added Ingestion API support status. These updates make it easier to assess ingestion routes and transformation support for activity logs at scale.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/azureactivity

- **DNSQueryLogs (table reference)**  
  Refreshed capability nomenclature and added an explicit Ingestion API support row. This helps network teams quickly validate transformation support and plan ingestion patterns.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/dnsquerylogs

- **SecurityAlert (table reference)**  
  Aligned the support matrix to the new labels and included Ingestion API support status. The change improves transparency on how security alerts can be ingested and transformed.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/securityalert

- **ContainerLog (table reference)**  
  Updated capability labels and added Ingestion API support status, clarifying how container logs can be transformed in DCR-based pipelines and which ingestion routes are available.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/containerlog

- **KubePodInventory (table reference)**  
  Standardized support fields and documented Ingestion API support. This streamlines planning for Kubernetes inventory data ingestion and downstream transformations.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/kubepodinventory

- **AppServiceHTTPLogs (table reference)**  
  Replaced legacy capability labels with the new taxonomy and added Ingestion API status. This helps teams validate supported paths for web app HTTP log ingestion and transformation.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/appservicehttplogs

- **Perf (table reference)**  
  Adopted the standardized capabilities (Basic, Auxiliary/Lake, DCR workspace transformations) and added Ingestion API support. The update simplifies understanding of supported routes for performance metrics in Logs.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/perf

- **Event (table reference)**  
  Updated capability fields to the new schema and recorded Ingestion API support (Yes/No). This provides clear guidance on event ingestion choices and whether DCR transformations are supported.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/event

- **Syslog (table reference)**  
  Standardized capability fields and added an explicit Ingestion API support indicator. This assists with planning Linux log ingestion strategies and DCR-based transformations.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/syslog