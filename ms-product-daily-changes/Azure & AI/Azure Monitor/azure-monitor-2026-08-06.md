# Azure Monitor
**Date created:** 2026-08-06 UTC  
**Tags:** Monitoring  

## Moderate Changes

- **Understand autoscale settings in Azure Monitor**

  Updated the example to clearly use a single default profile with two metric rules and clarified the scale-in evaluation window as 10 minutes via the timeWindow parameter. This improves accuracy and helps operators configure when scale-out and scale-in actions are triggered to avoid unexpected scaling behavior.

  https://learn.microsoft.com/en-us/azure/azure-monitor/autoscale/autoscale-understanding-settings

- **Use Azure Monitor Dashboards with Grafana**

  Added guidance on linking between dashboards using Grafana data links, including built-in links for AKS dashboards that carry cluster and namespace context. This enables faster drill-through from overview to detailed views, with step-by-step instructions to configure link titles, URLs with query parameters, and optional new-tab behavior.

  https://learn.microsoft.com/en-us/azure/azure-monitor/visualize/visualize-use-grafana-dashboards