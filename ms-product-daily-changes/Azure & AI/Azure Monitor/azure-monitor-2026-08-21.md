# Azure Monitor
**Date created:** 2026-08-21 UTC  
**Tags:** Automation, Configuration, Deprecation, Guidance, Monitoring  

## Major Changes

- **Use Azure Monitor Issues**

  Expanded guidance for associating an Azure Monitor Workspace with a subscription. Added step-by-step, multi-tab instructions for Portal, Azure CLI (az rest), Azure PowerShell (Invoke-AzRestMethod), and direct REST calls, including request construction, variables, and payload examples. This improves clarity and enables teams to automate or script association tasks consistently across environments. Minor wording refinements improve overall readability.

  https://learn.microsoft.com/en-us/azure/azure-monitor/aiops/issues-how-to

## Moderate Changes

- **Azure Monitor Agent extension versions**

  Removed support for CentOS 7 on Linux for the Azure Monitor Agent and updated the July 2026 release highlights accordingly. This deprecation notice helps administrators plan migrations to supported Linux distributions to maintain compatibility and support.

  https://learn.microsoft.com/en-us/azure/azure-monitor/agents/azure-monitor-agent-extension-versions

- **Azure Monitor REST API index**

  Added a preview operation group for managing Azure Monitor Workspace subscription settings, including the default workspace at the subscription level. The entry notes its dependency for Azure Monitor Issues and specifies API version 2025-06-03-preview; the dedicated REST reference page is not yet published.

  https://learn.microsoft.com/en-us/azure/azure-monitor/fundamentals/azure-monitor-rest-api-index