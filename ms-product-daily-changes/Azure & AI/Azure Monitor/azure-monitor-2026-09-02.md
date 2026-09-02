# Azure Monitor
**Date created:** 2026-09-02 UTC  
**Tags:** Automation, Configuration, Governance, Guidance, Monitoring  

## Major Changes

- **Use Azure Monitor Dashboards with Grafana**

  Expanded guidance for managing Grafana dashboards as ARM templates, replacing the brief export section with a full “Manage a dashboard as an ARM template” workflow. Added step-by-step export instructions, a detailed breakdown of template structure and parameters, and API version considerations for Microsoft.Dashboard resources. Included end-to-end deployment options via Portal, Azure CLI, PowerShell, and REST with prerequisites and access guidance. Introduced best practices to maintain dashboards as code with parameter files, source control, pipelines, and diagnostic settings for version tracking.

  https://learn.microsoft.com/en-us/azure/azure-monitor/visualize/visualize-use-grafana-dashboards

## Moderate Changes

- **Azure Monitor Agent Supported Operating Systems**

  Added support for multiple Linux distributions and versions, including AlmaLinux 10, Oracle Linux 10, Rocky Linux 10, Ubuntu 26.04 LTS, SUSE Linux Enterprise Server 16, SUSE Linux Enterprise Server 12 SP5, and Azure Linux 4.0. This broadens deployment options and simplifies planning for organizations standardizing on newer or diverse Linux environments.

  https://learn.microsoft.com/en-us/azure/azure-monitor/agents/azure-monitor-agent-supported-operating-systems

- **Supported metrics - Microsoft.DocumentDB/DatabaseAccounts**

  Updated the Throttled Request Percentage metric to support 1-minute granularity. This enables more precise monitoring and alerting for throttling events and faster detection of performance issues.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/supported-metrics/microsoft-documentdb-databaseaccounts-metrics

- **PaymentHsmHardwareOperationAuditLogs**

  Enabled Basic table support for the PaymentHsmHardwareOperationAuditLogs table. This provides a lower-cost option and simpler querying for scenarios that don’t require advanced table capabilities.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables/paymenthsmhardwareoperationauditlogs