# Azure Monitor
**Date created:** 2026-09-04 UTC  
**Tags:** Analytics, Configuration, Guidance, Monitoring, Troubleshooting  

## Major Changes

- **Delete Data from a Log Analytics Workspace by Using the Delete Data API**

  Expanded the how-to article with end-to-end Azure CLI, REST, and updated PowerShell examples for calling the Tables - Delete Data API. Updated guidance emphasizes using Invoke-AzRestMethod and polling Azure-AsyncOperation/Location to track asynchronous completion, clarifying that 202 Accepted only confirms request receipt. Added detailed procedures, sample payloads/outputs, and operation status checks via CLI, PowerShell, and REST, plus notes on limitations like missing record counts in Activity Log events. This improves reliability and safety when automating deletions by ensuring correct request construction and proper status validation.

  https://learn.microsoft.com/en-us/azure/azure-monitor/logs/delete-log-data

## Moderate Changes

- **Monitor your AKS cluster network with Azure Monitor**

  Updated terminology and parameters from Retina Network Flow Logs to Container Network Logs, including replacing enableRetinaNetworkFlowLogs with enableContainerNetworkLogs and updating stream names. Revised Log Analytics references to use the ContainerNetworkLogs table and related table plan guidance, aligning deployments and queries with the current schema.

  https://learn.microsoft.com/en-us/azure/azure-monitor/containers/container-insights-network-monitoring