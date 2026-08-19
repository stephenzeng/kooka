# Azure Monitor
**Date created:** 2026-08-19 UTC  
**Tags:** Best Practices, Configuration, Governance, Guidance, Identity, Monitoring, Security, Troubleshooting  

## Moderate Changes

- **Troubleshoot log alerts in Azure Monitor | Microsoft Docs**

  Expanded troubleshooting guidance for permission-related failures when creating or editing log alert rule queries. Clarified that data-plane query permission (Microsoft.OperationalInsights/workspaces/query/read) is required in addition to ARM read access, and explained common error patterns (HTTP 403 or AuthorizationRequiredError). Added steps for cross-tenant/Azure Lighthouse scenarios to register Microsoft.Insights in the managing tenant and create required Microsoft service principals with Contributor role for provider registration.

  https://learn.microsoft.com/en-us/azure/azure-monitor/alerts/alerts-troubleshoot-log

- **Troubleshoot Azure Monitor metric alerts**

  Added guidance to account for transient metric spikes during resource startup that can cause alerts with short aggregation periods. Recommended increasing Aggregation granularity (Period) or using alert processing rules to suppress alerts during expected start windows.

  https://learn.microsoft.com/en-us/azure/azure-monitor/alerts/alerts-troubleshoot-metric

- **Enable monitoring for Azure Kubernetes Service (AKS) clusters**

  Clarified that Managed Prometheus does not collect AKS control plane metrics by default and introduced the --enable-control-plane-metrics option. Provided az aks create/update examples to enable control plane metrics alongside managed Prometheus and documented prerequisites, default targets (API server and etcd), and a link to detailed monitoring guidance.

  https://learn.microsoft.com/en-us/azure/azure-monitor/containers/kubernetes-monitoring-enable

- **Default Prometheus metrics configuration in Azure Monitor**

  Updated default control plane metric target names from controlplane-apiserver/controlplane-etcd to apiserver/etcd to reflect current identifiers. This helps align configurations with the latest target naming.

  https://learn.microsoft.com/en-us/azure/azure-monitor/containers/prometheus-metrics-scrape-default