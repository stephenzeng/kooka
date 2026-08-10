# Microsoft Purview
**Date created:** 2026-07-11 UTC  
**Tags:** Monitoring  

## Moderate Changes

- **Monitor device health with the device health reports dashboard**

  Updated guidance clarifies that the “Last time devices were seen online” buckets (24 hours, 3 days, 7 days, 30 days) are separate and non-cumulative. Each device is counted once in the most recent applicable bucket based on its latest Last seen timestamp. This helps interpret recency accurately and avoids double counting in activity reports.

  https://learn.microsoft.com/en-us/purview/device-onboarding-health-reports-dashboard