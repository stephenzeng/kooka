# Azure Monitor
**Date created:** 2026-08-10 UTC  
**Tags:** Best Practices, Billing, Configuration, Consumption, Deprecation, Governance, Guidance, Monitoring, Security, Troubleshooting  

## Moderate Changes

- **Legacy authentication for Container insights**

  Reorganized guidance to emphasize migrating from legacy authentication to managed identity, with new prerequisites and streamlined steps for AKS and Arc-enabled Kubernetes. Clarified cluster identification queries, added a post-migration verification step, and removed instructions to enable legacy auth while highlighting behavior during Log Analytics key rotation.

  https://learn.microsoft.com/en-us/azure/azure-monitor/containers/container-insights-authentication

- **Configure the ContainerLogV2 schema for Container insights**

  Updated ContainerLogV2 schema details (standardized lowercase KubernetesMetadata fields and added imageID/imageRepo), standardized LogLevel values, and clarified log truncation limits. Improved enablement guidance, metadata inclusion examples, Grafana dashboard usage, and multiline logging instructions, and reinforced the migration path with the ContainerLog table retiring on 30 September 2026.

  https://learn.microsoft.com/en-us/azure/azure-monitor/containers/container-insights-logs-schema

- **Azure Monitor cost and usage**

  Updated pricing guidance to clarify that native custom metrics are free during preview. Revised Operation table details to specify new string formats and clarified how Defender and Per Node benefits combine in legacy tiers.

  https://learn.microsoft.com/en-us/azure/azure-monitor/fundamentals/cost-usage

- **Data collection endpoints in Azure Monitor**

  Added prerequisites to register the Microsoft.Insights resource provider and expanded portal steps with post-deployment verification. Enhanced CLI and REST examples (including disabling public network access, checking provisioning state, API version 2024-03-11, and DCR associations) and clarified when a DCE is required with AMA and Private Link/AMPLS.

  https://learn.microsoft.com/en-us/azure/azure-monitor/data-collection/data-collection-endpoint-overview

- **Metrics in Azure Monitor**

  Updated the metrics comparison to reflect a new cost model: Prometheus metrics are billed while native custom metrics are no charge during preview. Added deprecation guidance noting the Log Analytics agent retirement in August 2024 and recommending Azure Monitor Agent, with clarified retention details for legacy deployments.

  https://learn.microsoft.com/en-us/azure/azure-monitor/metrics/data-platform-metrics

- **Monitor Azure resources with Azure Monitor**

  Reorganized the article and added a summary table that explains each Azure portal monitoring menu item and how to learn more. Standardized section headings and clarified when logs are available and how to use Metrics explorer, improving consistency with Azure Monitor terminology.

  https://learn.microsoft.com/en-us/azure/azure-monitor/platform/monitor-azure-resource

- **Design Azure Monitor Private Link configuration**

  Expanded guidance with a comparison of Private Only versus Open access modes, including reachability and data exfiltration considerations. Clarified global versus per-network overrides, recommended safe adoption of Private Only, and explained exceptions for ingestion and the impact of blocking public queries on workbooks, dashboards, insights, and external tools.

  https://learn.microsoft.com/en-us/azure/azure-monitor/fundamentals/private-link-design

- **Roles, permissions, and security in Azure Monitor**

  Added a capabilities comparison for Monitoring Reader versus Monitoring Contributor and explicit ListKeys prerequisites for configuring diagnostic settings to storage/Event Hubs. Clarified that these roles don’t grant read access to data in storage or Event Hubs, updated legacy/retired notes, strengthened role assignment guidance, and improved PowerShell examples.

  https://learn.microsoft.com/en-us/azure/azure-monitor/fundamentals/roles-permissions-security