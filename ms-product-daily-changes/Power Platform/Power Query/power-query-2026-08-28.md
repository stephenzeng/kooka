# Power Query
**Date created:** 2026-08-28 UTC  
**Tags:** Deprecation, Guidance  

## Major Changes

- **Power Platform dataflows in Microsoft Teams (deprecated)**

  Announced deprecation of Power Platform dataflows in Dataverse for Teams with a staged retirement: creation disabled on Sept 1, 2026; experience marked deprecated and refresh disabled on Oct 1, 2026; and entry points removed/disabled on Oct 31, 2026. Existing dataflows are not deleted, but they will stop refreshing and won’t be accessible through the retired Teams experience. This change does not affect dataflows in Power BI, Power Automate, Dynamics 365, or Power Apps outside Dataverse for Teams. Customers should upgrade the Teams environment to full Dataverse to use standard V2 dataflows in Power Apps Maker or migrate to Dataflow Gen2 in Microsoft Fabric to maintain continuity.

  https://learn.microsoft.com/en-us/power-query/dataflows/dataflows-teams