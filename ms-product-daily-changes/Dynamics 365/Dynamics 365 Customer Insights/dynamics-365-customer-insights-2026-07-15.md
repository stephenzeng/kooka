# Dynamics 365 Customer Insights
**Date created:** 2026-07-15 UTC  
**Tags:** Administration, Analytics, Governance  

## Moderate Changes

- **Export segments to Adobe Experience Platform (preview)**

  Updated the export connection setup to require Resource group and Storage account instead of Account name and Account key, with Container unchanged. Removed an outdated storage configuration screenshot and refined guidance on who can use the connection and the steps to follow. These changes help admins configure the AEP export more reliably.

  https://learn.microsoft.com/en-us/dynamics365/customer-insights/data/export-adobe-experience-platform

- **Service limits and fair use policy**

  Added a section clarifying how segment limits classify static versus dynamic segments. This guidance explains when segments are counted as static (snapshot or manual include/exclude only) versus dynamic, helping teams plan capacity and stay within policy.

  https://learn.microsoft.com/en-us/dynamics365/customer-insights/journeys/fair-use-policy

- **Build segments in Customer Insights - Journeys**

  Added detailed guidance on grouping conditions and how logic differs within a group versus across separate groups. Expanded static membership management up to 2,000,000 members via Dataverse grid and CSV, clarified inclusion/exclusion precedence, Contacts tab limits, and combining static with dynamic criteria. Added notes on estimate and sample limitations and directed users to consent-based criteria, improving accuracy and compliance.

  https://learn.microsoft.com/en-us/dynamics365/customer-insights/journeys/real-time-marketing-build-segments

- **Transfer data with the Configuration Migration tool**

  Clarified migration steps for segments, requiring both msdynmkt_segment and msdynmkt_segmentdefinition in the schema to avoid incomplete records. Recommended transferring segments in Draft and publishing after import. Updated the title and description to emphasize Customer Insights - Journeys scope and constraints.

  https://learn.microsoft.com/en-us/dynamics365/customer-insights/journeys/transfer-data