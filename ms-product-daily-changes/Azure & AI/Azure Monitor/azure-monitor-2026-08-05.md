# Azure Monitor
**Date created:** 2026-08-05 UTC  
**Tags:** Monitoring  

## Moderate Changes

- **Create Azure Monitor log search alert rules**

  Clarified behavior when linked storage is configured for the Alerts data source: fired alert payloads redact and omit the alert query because it’s stored in a customer-managed storage account. Updated guidance recommends using alert dimensions to provide context for investigations and links to considerations for customer-managed keys for saved log alert queries.

  https://learn.microsoft.com/en-us/azure/azure-monitor/alerts/alerts-create-log-alert-rule

- **Use customer-managed storage accounts in Azure Monitor Logs**

  Updated the Alerts data source guidance to note that, with linked storage enabled, alert payloads no longer include the query and show a redaction comment instead. The article advises using alert dimensions to add meaningful context and references considerations for customer-managed keys for saved log alert queries.

  https://learn.microsoft.com/en-us/azure/azure-monitor/logs/private-storage

- **Connect Grafana to Azure Monitor managed service for Prometheus**

  Revised instructions to reflect Grafana 13+ changes: Azure authentication is supported only via the Azure Monitor Managed Service for Prometheus data source plugin, not the core Prometheus data source. Included a migration note that existing Azure-authenticated Prometheus data sources are automatically moved to the plugin and updated version-specific setup steps for Azure Managed Grafana and self-managed Grafana. Added references for managing data source plugins.

  https://learn.microsoft.com/en-us/azure/azure-monitor/metrics/prometheus-grafana

- **Resource-scoped queries for Azure Monitor workspace**

  Added a prerequisite to register the Microsoft.Monitor resource provider in every subscription containing resources you query, especially when resources and the workspace span different subscriptions. Introduced troubleshooting for 403 errors caused by a missing registration and provided portal, CLI, and PowerShell options to register the provider.

  https://learn.microsoft.com/en-us/azure/azure-monitor/metrics/prometheus-resource-scoped-queries