# Azure Monitor
**Date created:** 2026-08-09 UTC  
**Tags:** Administration, Governance, Monitoring  

## Moderate Changes

- **Analyze metrics with Azure Monitor metrics explorer**

  Clarified that Monitoring Reader at the subscription level is required to visualize metrics across multiple resources, resource groups, or an entire subscription. Expanded PromQL guidance to cover label filtering, math operations, and cross–time series aggregations, and specified that an Azure Monitor workspace is required; removed the preview label. Corrected alert severities to include Warning as a distinct level.

  https://learn.microsoft.com/en-us/azure/azure-monitor/metrics/analyze-metrics

- **Get started with autoscale in Azure**

  Added prerequisites, detailed programmatic setup options (PowerShell, CLI, ARM templates, REST), and clarified default rule behavior with concrete scale-in/out examples, including scheduled scenarios. Documented the five-minute cool-down period and added guidance on disabling autoscale by switching to Manual. These updates make it easier to deploy, understand, and manage autoscale consistently.

  https://learn.microsoft.com/en-us/azure/azure-monitor/autoscale/autoscale-get-started

- **Cost optimization in Azure Monitor**

  Restructured content to align with the Azure Well-Architected Framework’s cost optimization pillar and provided feature-specific guidance to reduce data collection and spend. Renamed sections to emphasize cost optimization and corrected the Alerts include. Expanded next steps with targeted links to cost guidance.

  https://learn.microsoft.com/en-us/azure/azure-monitor/fundamentals/best-practices-cost

- **Create a Log Analytics Workspace**

  Expanded end-to-end instructions across portal, PowerShell, CLI, Bicep, and ARM templates, including runnable samples and verification commands. Clarified retention guidance—especially for the Free tier—and set a default of 30 days for heartbeatTableRetention in Bicep and ARM templates. Improved references and related content for easier setup and governance.

  https://learn.microsoft.com/en-us/azure/azure-monitor/logs/quick-create-workspace