# Microsoft Fabric
**Date created:** 2026-07-26 UTC  
**Tags:** Analytics  

## Moderate Changes

- **Explore Fabric workspace item events in Fabric Real-Time hub**

  Removed the capacityId and domainId properties from the top-level schema for Fabric workspace item events. Update any event consumers, parsers, or filtering logic that rely on these fields to prevent failures and ensure accurate processing. This aligns the documentation with the current payload structure and reduces confusion.

  https://learn.microsoft.com/en-us/fabric/real-time-hub/explore-fabric-workspace-item-events