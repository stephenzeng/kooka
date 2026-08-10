# Azure Monitor
**Date created:** 2026-07-17 UTC  
**Tags:** Monitoring  

## Moderate Changes

- **Query data in a Basic and Auxiliary table in Azure Monitor Logs**

  Removed Azure CLI and PowerShell examples for running Log Analytics queries against Basic and Auxiliary tables. Guidance now centers on using the REST /search endpoint, providing a single, consistent approach for programmatic queries.

  https://learn.microsoft.com/en-us/azure/azure-monitor/logs/basic-logs-query

- **Azure Monitor Metrics overview**

  Added guidance on Advanced platform metrics, offering deeper, more granular metrics for supported resource providers. Clarified that this feature is preview, requires explicit resource-level opt-in, and is billed as a paid capability, with a link to learn more.

  https://learn.microsoft.com/en-us/azure/azure-monitor/metrics/data-platform-metrics

- **What's new in Azure Monitor documentation**

  Announced Advanced platform metrics (preview), a paid option for more granular platform metrics. Highlighted that these metrics can be analyzed with existing Azure Monitor tools and APIs for a familiar analysis experience.

  https://learn.microsoft.com/en-us/azure/azure-monitor/fundamentals/whats-new