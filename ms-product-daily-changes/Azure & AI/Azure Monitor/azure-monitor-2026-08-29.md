# Azure Monitor
**Date created:** 2026-08-29 UTC  
**Tags:** Best Practices, Configuration, Get Started, Governance, Guidance, Identity, Monitoring, Performance, Security, Troubleshooting  

## Major Changes

- **Add or Delete Tables and Columns in Azure Monitor Logs**

  Expanded and reorganized end-to-end guidance for creating and managing custom tables and columns across Portal, CLI, PowerShell, REST, Bicep, and ARM. Added variable-based CLI scripts, comprehensive PowerShell examples (including DCR creation and delete operations), and clarified REST/Bicep/ARM templates with consistent placeholders and <TableName>_CL naming. Standardized tabs, clarified GUID and datetime handling, and documented CLI limitations with detailed PowerShell/REST update patterns, making schema management more consistent and reliable.

  https://learn.microsoft.com/en-us/azure/azure-monitor/logs/create-custom-table

## Moderate Changes

- **Create metric alerts in Azure Monitor Logs**

  Updated ARM/Bicep samples to parameterize API versions, correct data types (for example, threshold and failingPeriods as integers), and add StaticThresholdCriterion to criteria. Fixed parameter file schemas and removed hard-coded values to improve deployment correctness and maintainability.

  https://learn.microsoft.com/en-us/azure/azure-monitor/alerts/alerts-metric-logs

- **Create And Configure Application Insights Resources**

  Standardized REST, Bicep, and ARM examples to use parameterized apiVersion values and consolidated REST references to a unified Azure Monitor API index. Updated pricing guidance to modify Log Analytics workspace SKUs via Workspaces Update (PATCH), replacing the legacy pricingPlans API, for more reliable, version-agnostic deployments.

  https://learn.microsoft.com/en-us/azure/azure-monitor/app/create-workspace-resource

- **Application Insights managed workspaces**

  Expanded deletion guidance with prerequisites to remove AMPLS associations and clear locks/policy before proceeding. Clarified two supported paths (delete Application Insights or reconnect to another workspace) and emphasized deleting the managed resource group rather than the workspace to avoid orphaned resources, noting AMPLS associations aren’t removed automatically.

  https://learn.microsoft.com/en-us/azure/azure-monitor/app/managed-workspaces

- **.NET Profiler for App Service**

  Clarified how Profiler captures traces, its preinstallation on App Service, and that it requires Always On for ASP.NET/ASP.NET Core on Windows Basic tier or higher. Added cross-subscription enablement steps, sovereign cloud endpoint settings, refined Entra-based ingestion guidance, clearer disable steps, and a best practice to exclude App_Data from Web Deploy to prevent profiler file deletion.

  https://learn.microsoft.com/en-us/azure/azure-monitor/profiler/profiler

- **Enable Azure Monitor OpenTelemetry Profiler Preview for .NET on Linux**

  Rebranded and added a prominent preview notice, with clearer steps to enable and configure using OpenTelemetry versus the legacy Application Insights SDK. Improved deployment guidance and connection string usage, and refined section titles and troubleshooting flow to set expectations and prerequisites.

  https://learn.microsoft.com/en-us/azure/azure-monitor/profiler/profiler-aspnetcore-linux

- **Profile .NET apps in containers**

  Refocused guidance around profiling .NET apps running in containers with a clear checklist and updated sample setup. Switched configuration to use ConnectionString instead of InstrumentationKey, refined Docker commands, and clarified how to verify profiler sessions and view traces in the portal, with strengthened troubleshooting.

  https://learn.microsoft.com/en-us/azure/azure-monitor/profiler/profiler-containers

- **View .NET Profiler trace data**

  Reorganized instructions for generating load, finding traces in the portal, and reading performance data and call stacks. Expanded explanations of profiler concepts (for example, allocation, lock contention, waits, AWAIT_TIME, BLOCKED_TIME, unmanaged async) and clarified timing metrics and “When” bucketing to improve analysis accuracy.

  https://learn.microsoft.com/en-us/azure/azure-monitor/profiler/profiler-data

- **.NET Profiler on Service Fabric**

  Emphasized production-load bottleneck detection and clarified that Profiler is included with Azure Diagnostics and enabled when the extension is installed. Updated templates to use an Application Insights connection string and provided explicit enablement guidance for stateless APIs and custom operations.

  https://learn.microsoft.com/en-us/azure/azure-monitor/profiler/profiler-servicefabric

- **.NET Profiler settings**

  Rewrote the settings guide with a clearer overview and streamlined navigation to traces. Clarified trigger behaviors for CPU and memory, added explicit CPU thresholds, restructured Sampling options (Normal, High, Maximum) with updated Normal rate details, and simplified “Profile now” and recent sessions descriptions to aid configuration.

  https://learn.microsoft.com/en-us/azure/azure-monitor/profiler/profiler-settings

- **.NET request tracking code**

  Highlighted that Profiler only captures profiles for tracked requests and reorganized guidance for manual request tracking and nested operations. Updated samples to use TelemetryConfiguration.Active.ConnectionString and showed how to nest DependencyTelemetry, link exceptions, and set success state.

  https://learn.microsoft.com/en-us/azure/azure-monitor/profiler/profiler-trackrequests

- **Troubleshoot Application Insights Profiler for .NET**

  Restructured troubleshooting with clarified runtime support, extended data retention to 15 days, and an explicit gateway URL check. Streamlined App Service diagnostics (including verifying the ApplicationInsightsProfiler3 WebJob), added manual install steps, documented one-session-per-VM limits and mitigations, expanded Web Deploy skip rules, and reinforced VM, proxy, and firewall validation using the Azure Monitor service tag.

  https://learn.microsoft.com/en-us/azure/azure-monitor/profiler/profiler-troubleshooting

- **Enable .NET Profiler on VMs**

  Retitled and reorganized enablement on Windows VMs and scale sets with three methods, recommending ARM template plus Visual Studio. Switched to connection strings in WadCfg, expanded PowerShell export/edit/reapply steps and Resource Explorer edits, added IIS HTTP Tracing enablement, and clarified that on-premises servers aren’t supported.

  https://learn.microsoft.com/en-us/azure/azure-monitor/profiler/profiler-vm

- **Resource Manager template samples for metric alerts**

  Parameterized API versions across ARM/Bicep samples, corrected example data types to integers, and added StaticThresholdCriterion to criteria objects. Renamed code tabs and standardized references to the unversioned Microsoft.Insights/metricAlerts path to improve template clarity and reuse.

  https://learn.microsoft.com/en-us/azure/azure-monitor/alerts/resource-manager-alerts-metric

- **Azure Monitor Resource log / log analytics tables**

  Aligned branding by renaming “Azure Active Directory Logs” to “Microsoft Entra ID Logs” and “Azure Sentinel” to “Microsoft Sentinel,” and reorganized their positions and ordering. No tables were added or removed, preserving content while improving consistency and navigation.

  https://learn.microsoft.com/en-us/azure/azure-monitor/reference/tables-index

- **Tutorial - Add ingestion-time transformation to Azure Monitor Logs using Resource Manager templates**

  Updated the tutorial to reference specific Azure Monitor REST operations and modernized PowerShell with placeholders and explicit API versions. Adjusted templates to parameterize dataCollectionRules apiVersion and simplified column definitions, with clearer portal steps and links for a smoother setup.

  https://learn.microsoft.com/en-us/azure/azure-monitor/logs/tutorial-workspace-transformations-api