# Dynamics 365 Customer Service
**Date created:** 2026-07-25 UTC  
**Tags:** Administration  

## Moderate Changes

- **Create and manage queues for unified routing**

  Updated guidance on configuring queues to set conversation owner and business unit during routing based on the queue owner. Introduced an organization-level setting (msdyn_issetowneridfromqueueoninitenabled) on msdyn_omnichannelconfiguration, with a Web API example and clarified behavior: it won’t overwrite an existing owner, falls back gracefully if no queue owner or on errors, and applies to both user- and team-owned queues. This helps admins ensure consistent ownership and BU alignment for routed conversations.

  https://learn.microsoft.com/en-us/dynamics365/customer-service/administer/queues-omnichannel