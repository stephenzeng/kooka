# Dynamics 365 Customer Insights
**Date created:** 2026-08-28 UTC  
**Tags:** Automation, Best Practices, Guidance  

## Moderate Changes

- **View tables in Customer Insights - Data**

  Added critical guidance on Dataverse refresh behavior: rows may be deleted and recreated during refreshes, which resets Created On and emits delete/create events. Updated recommendations to avoid using Created On or row-level events for change detection; instead use CustomerId as the stable key, perform upserts, and trigger downstream processing after refresh completion (for example, via the Power Automate connector). Minor wording clarifications were made without changing technical behavior.

  https://learn.microsoft.com/en-us/dynamics365/customer-insights/data/tables