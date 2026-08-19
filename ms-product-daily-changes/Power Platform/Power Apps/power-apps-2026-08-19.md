# Power Apps
**Date created:** 2026-08-19 UTC  
**Tags:** Best Practices, Guidance, Performance  

## New Articles

- **Plan your latency for Link to Fabric**

  Introduced a new conceptual guide to help makers plan and set expectations for data freshness when replicating Dataverse to Fabric via Link to Fabric. It explains key drivers of sync latency—such as initial load size, data churn, table width, number of tables, long-running transactions, and CDF—and clarifies that the observed figures are indicative rather than SLAs. The article shares P50/P95 latency observations across common load patterns and industries, and explains why latency varies and spikes (for example, environment operations, locking, and bursty loads). It also provides practical guidance to measure latency accurately in your own environment, including handling ModifiedOn nuances, excluding initial loads, and validating in UAT, with references to related documentation.

  https://learn.microsoft.com/en-us/power-apps/maker/data-platform/fabric-link-plan-latency