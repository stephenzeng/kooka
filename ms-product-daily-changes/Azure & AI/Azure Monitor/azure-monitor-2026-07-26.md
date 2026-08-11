# Azure Monitor
**Date created:** 2026-07-26 UTC  
**Tags:** Security  

## Moderate Changes

- **Access the Azure Monitor Log Analytics API**
  
  Updated authentication guidance for the Log Analytics API client credentials flow to use the resource https://api.loganalytics.io instead of https://api.loganalytics.azure.com. This ensures tokens are requested for the correct audience and prevents authentication failures. Update any app registrations, scripts, and configurations to use the new resource value.
  
  https://learn.microsoft.com/en-us/azure/azure-monitor/logs/api/access-api