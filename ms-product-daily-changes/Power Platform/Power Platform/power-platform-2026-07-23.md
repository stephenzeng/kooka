# Power Platform
**Date created:** 2026-07-23 UTC  
**Tags:** Administration, Programming  

## Major Changes

- **Programmability and extensibility - what's new or changed**

  Added June and May 2026 updates covering expanded APIs and regular SDK releases. Introduced Copilot Studio bot APIs to get/set Connector Consent Bypass, enabling finer control over connector governance. Added extensive Power Pages website management REST APIs for certificates, host names, custom domains, allowed IP addresses, and SSL bindings, improving automation for site operations. Also added an Environment Management API (Preview) to retrieve environment operation status by ID and noted ongoing monthly releases for the Power Platform Management SDKs (Python, C#) and the Admins V2 connector.

  https://learn.microsoft.com/en-us/power-platform/admin/programmability-whats-new-changed

## Moderate Changes

- **Filter, Search, and LookUp functions**

  Clarified that, for Dataverse sources, a Filter formula can reference a Dataverse view and noted how returned columns are handled. Power Apps will only return columns known to be part of the specified Dataverse data source, even if the Dataverse view includes additional related columns—helping makers design queries with predictable results.

  https://learn.microsoft.com/en-us/power-platform/power-fx/reference/function-filter-lookup