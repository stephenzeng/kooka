# Microsoft Defender XDR
**Date created:** 2026-07-15 UTC  
**Tags:** Security  

## Moderate Changes

- **Activate Microsoft Defender unified role-based access control (URBAC)**

  Updated guidance to note that starting July 2026, the Microsoft Defender unified RBAC model becomes the default permissions model for new Microsoft Defender for Office 365 Plan 2 organizations. This helps admins plan for onboarding and align governance with the upcoming default. A reference to Message Center post MC1246006 is included for further details.

  https://learn.microsoft.com/en-us/defender-xdr/activate-defender-rbac

- **Map existing RBAC permissions to Microsoft Defender unified RBAC permissions**

  Expanded RBAC mappings by adding the “Quarantine Emails (read)” permission to multiple role groups and the Quarantine role. Also added Exchange admin mappings for Security Reader and View-Only Configuration (core security settings read) and Security Operator (detection tuning manage). These updates clarify least-privilege assignments and improve operational coverage.

  https://learn.microsoft.com/en-us/defender-xdr/compare-rbac-roles

- **Permissions in Microsoft Defender unified role-based access control (RBAC)**

  Introduced a new “Security posture – AI code scan” section detailing permissions to run scans, upload results, and view or manage AI code scan outcomes. This defines governance for AI code scanning workflows and helps admins assign appropriate capabilities for development security operations.

  https://learn.microsoft.com/en-us/defender-xdr/custom-permissions-details

- **Microsoft Defender unified role-based access control (RBAC)**

  Added a note that starting July 2026, the unified RBAC model becomes the default permissions model for new Microsoft Defender for Office 365 Plan 2 organizations. This prepares administrators for default behavior changes and supports permission model standardization. A reference to Message Center post MC1246006 is provided.

  https://learn.microsoft.com/en-us/defender-xdr/manage-rbac