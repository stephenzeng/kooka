# Dynamics 365 Contact Center
**Date created:** 2026-07-28 UTC  
**Tags:** Agent  

## Moderate Changes

- **Use service representative availability APIs**

  Clarified API behavior and limits, including that overflow handling and workstream-level percentage routing are not considered, and that when multiple route-to-queue rules match, the first matching queue is used. Documented refresh cadences to set expectations for integrations: queue metrics update near real time, representative availability about every five minutes, and queue configuration every 10 minutes. Updated wording to generalize channel applicability and to explicitly scope the APIs to Dynamics 365 Contact Center.

  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/representative-availability-overview