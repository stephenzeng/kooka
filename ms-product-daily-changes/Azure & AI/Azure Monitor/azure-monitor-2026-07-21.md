# Azure Monitor
**Date created:** 2026-07-21 UTC  
**Tags:** Monitoring  

## Major Changes

- **Autoinstrumentation for Azure Monitor Application Insights**
  Expanded AKS coverage in the codeless autoinstrumentation support matrix to reflect broad runtime support rather than limited .NET and Python capabilities. Removed the limited preview footnote for AKS and aligned the entry with the public preview status. This clarifies support expectations and signals readiness for wider adoption on AKS.
  https://learn.microsoft.com/en-us/azure/azure-monitor/app/codeless-overview

## Moderate Changes

- **Overview of Log Analytics in Azure Monitor**
  Updated the More tools section with clearer, consolidated tool descriptions and added an Autosave subsection that explains how session state (scope, time range, tab names, and settings) is preserved, including scope and 30-day retention details. Added a note on query history behavior and simple mode’s single-query limit, and reorganized content with “Related content” replacing “Next steps” to streamline navigation.
  https://learn.microsoft.com/en-us/azure/azure-monitor/logs/log-analytics-overview

- **Supported Resource log categories for Azure Monitor**
  Removed the supported logs reference for Microsoft.Network/NetworkVirtualAppliances in the logs index. Metrics listings and other log references remain unchanged, reducing confusion about currently supported log categories.
  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/logs-index

- **Supported metrics with Azure Monitor**
  Updated the Microsoft.Network row to remove the supported logs entry for NetworkVirtualAppliances while keeping the metrics entry intact. This aligns the metrics index with current logging support and prevents misconfiguration.
  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/metrics-index