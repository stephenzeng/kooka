# Azure Monitor
**Date created:** 2026-08-26 UTC  
**Tags:** Best Practices, Configuration, Deprecation, Guidance, Identity, Monitoring, Security  

## Major Changes

- **Migrate from Diagnostic Settings Storage Retention to Azure Storage Lifecycle Management**

  Expanded migration guidance in response to the retirement of diagnostic settings storage retention on September 30, 2025. Added prerequisites with required RBAC permissions and a clear end-to-end flow using Azure CLI, including variable setup, policy files, and verification commands. Provided complete Bicep and ARM templates and noted that deployments replace any existing lifecycle policies. Clarified that diagnostic setting retention values no longer apply, and that new lifecycle policies affect only newly ingested data.

  https://learn.microsoft.com/en-us/azure/azure-monitor/platform/migrate-to-azure-storage-lifecycle-policy

- **Register an App to Request Authorization Tokens and Work with APIs**

  Introduced prerequisites that specify required Microsoft Entra roles and reworked the portal steps to include explicit role assignment via Access control (IAM). Expanded CLI and PowerShell examples with parameterized variables, clearer secret handling, and scoped role assignments to streamline RBAC setup. Reorganized the article end-to-end and refined next steps to map common roles (such as Reader and Monitoring Metrics Publisher) to typical API scenarios.

  https://learn.microsoft.com/en-us/azure/azure-monitor/logs/api/register-app-for-token

## Moderate Changes

- **Create and manage a dedicated cluster in Azure Monitor Logs**

  Updated SkuCapacity guidance to remove outdated instructions about minimums via CLI/templates and reliance on REST API for lower tiers. The section now lists the valid commitment tiers and links to dedicated cluster costs, simplifying capacity planning.

  https://learn.microsoft.com/en-us/azure/azure-monitor/logs/logs-dedicated-clusters

- **Standard columns in Azure Monitor log records**

  Added a concise summary table for key standard columns with descriptions and applicability, including classic Application Insights name differences. Clarified TimeGenerated behavior, advised sparing use of union withsource=tt due to cost, standardized headings, refined use of _ResourceId/_SubscriptionId, and updated example queries for clarity.

  https://learn.microsoft.com/en-us/azure/azure-monitor/logs/log-standard-columns

- **Monitor virtual machines with Azure Monitor: Alerts**

  Expanded guidance on when to use metric vs. log search alerts and how to scale alert rules. Clarified that VM availability alerts reflect machine state while agent heartbeat indicates agent health, with tips for ingestion latency. Corrected guest OS network metric mappings and refined instructions across CPU, memory, and disk alert sections.

  https://learn.microsoft.com/en-us/azure/azure-monitor/vm/monitor-virtual-machine-alerts

- **Audit queries in Azure Monitor log queries**

  Clarified configuration via Azure portal and templates, corrected AADEmail to reference the user account, and improved explanations for when QueryTimeRangeStart/End and RequestContext are populated. Standardized the product name to Microsoft Sentinel and clarified that enabling query auditing has no cost, though data ingestion charges may apply.

  https://learn.microsoft.com/en-us/azure/azure-monitor/logs/query-audit

- **Analyze metrics for an Azure resource**

  Clarified that the tutorial covers the classic metrics explorer and directed users of the newer experience to PromQL-based guidance. Added a prerequisite requiring at least the Monitoring Reader role and refined several instructional notes for accuracy.

  https://learn.microsoft.com/en-us/azure/azure-monitor/platform/tutorial-metrics

- **Collect resource logs from an Azure resource**

  Added steps to verify data ingestion with a log query and noted expected latency of about 10 minutes before data appears. Streamlined prerequisites and setup instructions without changing destinations or core workflow.

  https://learn.microsoft.com/en-us/azure/azure-monitor/platform/tutorial-resource-logs

- **Tutorial: Add a Workspace Transformation by Using the Azure Portal**

  Clarified DCR behavior, including user-defined naming, automatic linking, and schema changes based on transformation output. Expanded testing with explicit Kusto queries to confirm filtering and the presence of the Workspace_CF column with RequestContext cleared, and improved step-by-step guidance.

  https://learn.microsoft.com/en-us/azure/azure-monitor/logs/tutorial-workspace-transformations-portal

- **VM Insights Map and Dependency Agent retirement guidance**

  Strengthened retirement guidance with clearer impact details, including that the Service Map REST API is no longer queryable. Directed customers to alternative monitoring and diagnostics solutions and AMA with Change Tracking and Inventory, and updated key milestone dates and FAQs.

  https://learn.microsoft.com/en-us/azure/azure-monitor/vm/vminsights-maps-retirement