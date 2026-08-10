# Power Query
**Date created:** 2026-07-16 UTC  
**Tags:** Security  

## Moderate Changes

- **Google BigQuery (Microsoft Entra ID)**
  
  Updated guidance clarifies that cloud connections do not support the optional Audience URI parameter. Users leveraging Workforce Identity Federation should use the default Audience URI format //iam.googleapis.com/locations/global/workforcePools/powerquery-<TenantId>/providers/azuread, as custom Audience URI values are ignored by cloud connections. This helps prevent misconfiguration and authentication issues.
  
  https://learn.microsoft.com/en-us/power-query/connectors/google-bigquery-aad