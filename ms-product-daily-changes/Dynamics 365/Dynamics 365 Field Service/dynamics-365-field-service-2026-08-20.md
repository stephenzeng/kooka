# Dynamics 365 Field Service
**Date created:** 2026-08-20 UTC  
**Tags:** Billing, Configuration, Guidance, Troubleshooting  

## Moderate Changes

- **Get help with Field Service**

  Expanded and clarified troubleshooting guidance, distinguishing platform-level versus Field Service-specific errors and providing concrete next steps, including license checks, app installation validation, and running solution health rules. Added five common error scenarios with causes and resolutions: required service account, required price list, price list currency must match work order currency, status change blocked by current state, and booking creation blocked for canceled work orders. This improves diagnostic accuracy and speeds resolution for admins and support teams.

  https://learn.microsoft.com/en-us/dynamics365/field-service/field-service-get-help

- **Work order lifecycle and system statuses**

  Updated guidance so Actual Arrival Time is set when a technician changes booking status to In Progress, removing prior channel-specific differences. Revised Total Cost calculation to use per-booking journal duration with applicable pay type and markup, plus additional cost amounts, improving clarity and cost accuracy for billing and reporting.

  https://learn.microsoft.com/en-us/dynamics365/field-service/work-order-status-booking-status