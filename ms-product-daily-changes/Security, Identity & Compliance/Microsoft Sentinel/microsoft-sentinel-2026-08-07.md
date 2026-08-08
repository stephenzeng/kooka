# Microsoft Sentinel
**Change date:** 2026-08-07 UTC  
**Tags:** Governance, Security  

## Moderate Changes

- **Configure delegated access with governance relationships for multitenant organizations (preview)**

  Updated guidance to keep administrators working from governing-tenant accounts, without creating local admins or Entra B2B guests in governed tenants; template security groups appear as remote-tenant groups. Added an automation option using Tenant Governance APIs in Microsoft Graph. Clarified that Microsoft Sentinel Azure RBAC grants management-plane access only; assign required data‑plane roles separately following least privilege.

  https://learn.microsoft.com/en-us/unified-secops/governance-relationships

- **How Microsoft names threat actors**

  Updated the threat actor mapping table by adding Storm-2945 with a reference to Microsoft’s security blog. Identified it as a Midnight Blizzard sub-cluster to improve cross-referencing and tracking.

  https://learn.microsoft.com/en-us/unified-secops/microsoft-threat-actor-naming