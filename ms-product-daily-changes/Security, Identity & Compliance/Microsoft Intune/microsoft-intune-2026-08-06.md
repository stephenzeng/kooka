# Microsoft Intune
**Date created:** 2026-08-06 UTC  
**Tags:** Administration  

## Major Changes

- **Device action: collect diagnostics**

  Expanded the network requirements to list region-specific Azure Blob Storage endpoints that must be allowed for diagnostics uploads across Americas, Europe, Switzerland, East Asia, India, and Australia. Added guidance to identify your tenant geo and data center in endpoint.microsoft.com (Tenant Administration > Tenant status). These updates help administrators correctly configure firewalls and proxies, reducing upload failures and improving reliability. The clarified guidance also streamlines planning for network and compliance reviews.

  https://learn.microsoft.com/en-us/intune/device-management/actions/collect-diagnostics

- **Network endpoints for Microsoft Intune**

  Updated the Windows Autopilot diagnostics upload endpoints, replacing legacy lgmsap* hosts with the current amsua*/amsub*/amsuc*/amsud*/amsuin* blob.core.windows.net hosts in both the table and endpoint list. Administrators should update allow lists to ensure diagnostics uploads continue to work as the service evolves. This refresh aligns documentation with current service infrastructure and prevents connectivity gaps.

  https://learn.microsoft.com/en-us/intune/fundamentals/endpoints