# Azure Monitor
**Date created:** 2026-09-05 UTC  
**Tags:** Automation, Best Practices, Configuration, Guidance  

## Moderate Changes

- **Set up the Azure Monitor Agent on Windows client devices**

  Expanded end-to-end setup guidance with full CLI, PowerShell, and REST examples for creating role assignments, monitored objects, and data collection rule associations on Windows clients. Added a preview note with steps to list supported API versions, standardized parameters and REST endpoint patterns, and clarified reauthentication. Included reusable scripts and cleanup procedures to accelerate deployments and troubleshooting.

  https://learn.microsoft.com/en-us/azure/azure-monitor/agents/azure-monitor-agent-windows-client

- **Add or delete tables and columns in Azure Monitor Logs**

  Standardized CLI, PowerShell, REST, Bicep, and ARM examples with consistent variable naming and correct resource URLs, and added prerequisite steps such as installing the monitor-control-service extension. Clarified that the az monitor log-analytics workspace table update --columns command replaces the entire custom column set and documented how to remove all columns using REST/PowerShell with an empty array. Fixes and cleanups improve reliability and readability of deployment scripts.

  https://learn.microsoft.com/en-us/azure/azure-monitor/logs/create-custom-table