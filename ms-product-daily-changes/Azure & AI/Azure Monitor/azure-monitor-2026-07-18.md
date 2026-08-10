# Azure Monitor
**Date created:** 2026-07-18 UTC  
**Tags:** Monitoring  

## Moderate Changes

- **Azure Monitor health model concepts (preview)**

  Expanded guidance to explain how entity health is determined by both signals and child dependencies. Updated the Signals section to include Azure Resource Health and support for external health reports via the ingestion API, and clarified dependency configuration by renaming Minimum healthy/Maximum not healthy to Healthy limit/Not-healthy limit with revised threshold semantics and examples. Added explanations and screenshots for Worst of, Healthy limit, and Not-healthy limit, renamed Embedded to Nested health models, and clarified that alerts fire on degraded/unhealthy only when an alert is configured on the entity.

  https://learn.microsoft.com/en-us/azure/azure-monitor/health-models/concepts

- **Create discovery rules for Azure Monitor health models (preview)**

  Clarified discovery behavior, noting that selecting a service group generates a Resource Graph query and that health models can recursively discover nested service groups. Updated the heading to emphasize creating discovery rules, improving findability and setup accuracy.

  https://learn.microsoft.com/en-us/azure/azure-monitor/health-models/discoveries

- **Health models in Azure Monitor (preview)**

  Strengthened the introduction to highlight the shift from resource-centric alerting to health-based alerting to reduce alert fatigue, and refreshed visuals to show the Graph view. Added first-class IaC and CLI support for defining health models, removed an outdated SLO-related benefit, and updated Next steps with a link to monitoring a health model.

  https://learn.microsoft.com/en-us/azure/azure-monitor/health-models/overview

- **Configure hybrid Kubernetes clusters (deprecated) with Container insights**

  Updated configuration to require the secure kubelet cAdvisor port 10250 with authenticated access via a service account bearer token, deprecating any use of the read-only port 10255. Guidance and troubleshooting now align to current Kubernetes defaults and kubelet authentication/authorization requirements.

  https://learn.microsoft.com/en-us/azure/azure-monitor/containers/container-insights-hybrid-setup

- **Troubleshoot collection of container logs in Azure Monitor**

  Adjusted troubleshooting steps for non-Azure clusters to use authenticated access on port 10250 instead of the deprecated read-only port 10255. Added references to hybrid prerequisites, kubelet readOnlyPort settings, and kubelet authentication/authorization to ensure reliable log collection.

  https://learn.microsoft.com/en-us/azure/azure-monitor/containers/container-insights-troubleshoot

- **Set up a table with the Auxiliary plan in your Log Analytics workspace**

  Corrected the ARM template example by updating the $schema URL from 2019-08-01 to 2019-04-01 for Data Collection Rule deployment. This ensures templates validate and deploy correctly against the supported schema.

  https://learn.microsoft.com/en-us/azure/azure-monitor/logs/create-custom-table-auxiliary