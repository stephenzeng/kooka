# Dynamics 365 Field Service
**Date created:** 2026-09-02 UTC  
**Tags:** Configuration, Troubleshooting  

## Major Changes

- **Troubleshoot issues with Solution Health Hub**

  Added new Solution Health Hub rules to detect unsupported custom controls on Bookable Resource Booking forms/views and to validate the default Line Status value on Work Order Product. Elevated the “Incomplete Field Service upgrade” rule from Low to Critical to prompt urgent remediation. Clarified that the “Waiting workflow instances owned by disabled users” rule evaluates the last year of activity. Corrected privilege identifiers by removing erroneous prefixes to improve rule accuracy. Removed obsolete checks for Field Service Settings and for Latitude/Longitude values on account records.

  https://learn.microsoft.com/en-us/dynamics365/field-service/troubleshoot-field-service-solution-health