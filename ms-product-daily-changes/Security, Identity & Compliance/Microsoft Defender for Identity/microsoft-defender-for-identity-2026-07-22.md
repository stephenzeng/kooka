# Microsoft Defender for Identity
**Date created:** 2026-07-22 UTC  
**Tags:** Administration, Security  

## Moderate Changes

- **Configure Windows event auditing**

  The troubleshooting section about detecting and remediating GPO conflicts that revert automatic auditing (including use of the Find-MdiAuditingGpoConflicts.ps1 script) was removed, reversing an earlier addition. Guidance now focuses on core auditing configuration; for conflict detection and remediation, refer to the dedicated health alert documentation.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/configure-windows-event-collection

- **Microsoft Defender for Identity health issues**

  Added a new health alert for cases where auditing settings on a domain controller are repeatedly reverted. The guidance advises keeping Automatic Windows auditing enabled, running the Find-MdiAuditingGpoConflicts.ps1 script to locate conflicting GPOs, updating or unlinking the conflicts, running gpupdate /force, and confirming the settings remain stable.

  https://learn.microsoft.com/en-us/defender-for-identity/health-alerts

- **Migrate from Defender for Identity sensor v2 to sensor v3.x**

  Added that starting with sensor version 3.0.8 (July 2026), RPC auditing is enabled automatically on upgrade, eliminating manual setup. Clarified that v3.x sensors update via Windows Update and the v2.x per-sensor Delayed update option no longer applies. The “Not ready for migration” troubleshooting was reworked to use a reason-based table with verification steps and resolutions, helping admins quickly address readiness blockers.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/migrate-to-sensor-v3

- **What's new in Microsoft Defender for Identity**

  The August 2026 entry announcing a new health alert was removed. July 2026 updates were added, including support to migrate Windows Server 2025 domain controllers to sensor v3.x and a Sensors page tooltip that explains why a server is marked Not ready for migration, with links to relevant migration and troubleshooting guidance.

  https://learn.microsoft.com/en-us/defender-for-identity/whats-new