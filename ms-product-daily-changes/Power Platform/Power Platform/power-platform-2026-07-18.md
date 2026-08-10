# Power Platform
**Date created:** 2026-07-18 UTC  
**Tags:** Administration, Monitoring  

## Moderate Changes

- **Administration mode  **
  Clarified how administration mode affects flows: scheduled Power Automate cloud flows continue running because they execute in the Power Automate service, while Dataverse-triggered flows do not fire when background operations are disabled. Updated the description of background operations to specify it applies to Dataverse asynchronous operations, and noted that disabling background operations requires enabling administration mode.

  https://learn.microsoft.com/en-us/power-platform/admin/admin-mode

- **Create alerts for your resources**
  Added guidance for configuring a Data review period on resource-scoped alerts, with 24-hour and 1-hour options. The 1-hour option enables hourly metric aggregation and a Review period selector in charts; this capability is in preview and currently limited to code apps.

  https://learn.microsoft.com/en-us/power-platform/admin/monitoring/alerts