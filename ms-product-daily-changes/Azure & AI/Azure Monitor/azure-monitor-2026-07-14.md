# Azure Monitor
**Date created:** 2026-07-14 UTC  
**Tags:** Monitoring, Security  

## Moderate Changes

- **Monitor multiple time series in a single metric alert rule**

  Increased the documented default maximum of time series per metric alert rule from 5,000 to 10,000, enabling broader monitoring within a single rule. Clarifies that the limit can be removed by submitting a support request for scenarios that require greater scale.

  https://learn.microsoft.com/en-us/azure/azure-monitor/alerts/alerts-metric-multiple-time-series-single-rule

- **Best practices for autoscale**

  Streamlined the concepts section into a concise overview with links to detailed schema and common metrics. Clarifies multi-rule evaluation—scale out on any rule and scale in only when all rules match—supported by an evaluation example, and removes an outdated TLS 1.2 section.

  https://learn.microsoft.com/en-us/azure/azure-monitor/autoscale/autoscale-best-practices

- **Manage table-level access in a Log Analytics workspace**

  Added protected tables as a recommended, deny-by-default approach alongside granular RBAC. Explains granting access via ABAC conditions or the Privileged Monitoring Data Reader role, with configuration links, and updates the overview/navigation to reflect these options to strengthen data protection.

  https://learn.microsoft.com/en-us/azure/azure-monitor/logs/manage-table-access

- **Use Azure Private Link to connect networks to Azure Monitor**

  Reworked Access modes by replacing a dense table with clear bullets for Open and Private Only. Clarifies that ingestion and query modes are configured separately and can differ per connected VNet, and directs readers to the design article for deep dives and override choices to better convey security implications.

  https://learn.microsoft.com/en-us/azure/azure-monitor/fundamentals/private-link-security

- **Customize collection of Prometheus metrics from your Kubernetes cluster using ConfigMap**

  Removed a prior IMPORTANT notice about AKS Automatic clusters’ default managed system node pools and their impact on Prometheus custom scrape jobs. This aligns the article with current guidance and reduces confusion about expected behavior.

  https://learn.microsoft.com/en-us/azure/azure-monitor/containers/prometheus-metrics-scrape-configuration

- **Sample code to send data to Azure Monitor using Logs ingestion API**

  Updated throttling guidance for HTTP 429 to reflect current per-DCR limits: up to 2 GB of data per minute and 12,000 requests per minute. Clarifies handling when limits are exceeded, points to the service limits documentation for the latest values, and retains Retry-After–based backoff recommendations.

  https://learn.microsoft.com/en-us/azure/azure-monitor/logs/tutorial-logs-ingestion-code