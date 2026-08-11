# Microsoft Defender XDR
**Date created:** 2026-08-11 UTC  
**Tags:** Analytics, Governance, Security  

## Moderate Changes

- **DeviceInfo**

  Added the DeviceRoles column to the DeviceInfo table, providing device roles and characteristics in JSON, including confidence levels and last-seen timestamps. This enables more precise hunting, filtering, and correlation based on system-identified or user-defined device roles.

  https://learn.microsoft.com/en-us/defender-xdr/advanced-hunting-deviceinfo-table

- **Map existing RBAC permissions to Microsoft Defender unified RBAC permissions**

  Updated the RBAC comparison to include a Defender for Office permission for Email & collaboration content: Quarantine Emails (read). This clarifies which roles—Global administrator, Global reader, Security reader, and Security operator—have read access, helping admins validate least-privilege assignments and operational access.

  https://learn.microsoft.com/en-us/defender-xdr/compare-rbac-roles