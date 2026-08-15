# Dynamics 365 Field Service
**Date created:** 2026-08-15 UTC  
**Tags:** Billing, Configuration, Guidance  

## Moderate Changes

- **Not-to-exceed values on work orders**

  Updated guidance on how NTE is automatically selected: price and price-and-cost-margin NTEs prioritize service account, then billing account, then unmapped; cost NTEs use best field match and then lowest amount, and automatic selection applies only to work orders with a single incident type. Clarified mobile behavior, warnings, and that Applied amount reflects the NTE limit with updated source labels and reset behavior. Added an important caution that customizing work order NTE can disrupt automated selection.

  https://learn.microsoft.com/en-us/dynamics365/field-service/work-order-not-to-exceed

- **Work order lifecycle and system statuses**

  Clarified that when a work order is canceled, Closed By and Closed On are set, and refined billing to calculate Total Billable Duration from booking journals marked billable (working hours billable by default; breaks billable only if price list specifies). Updated travel charge behavior to add a work order product at booking completion when the service account has a travel charge type and Actual Travel Duration is greater than zero, removing the previous note about adding charges at work order completion.

  https://learn.microsoft.com/en-us/dynamics365/field-service/work-order-status-booking-status