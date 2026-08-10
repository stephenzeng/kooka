# Microsoft Defender for Identity
**Date created:** 2026-07-14 UTC  
**Tags:** Administration, Monitoring, Security  

## Moderate Changes

- **Deploy the Defender for Identity sensor v3.x**

  Removed the prior limitation and clarified that Windows Server 2025 domain controllers can be migrated from sensor v2.x to v3.x. Renamed the RPC auditing tag to Sensor Extended RPC Audit and raised the prerequisite sensor version to 3.0.7, with notes on behavior for earlier versions; updated guidance also explains how to combine rule conditions with AND/OR and refreshed screenshots.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/deploy-sensor-v3

- **Migrate from Defender for Identity sensor v2 to sensor v3.x (Preview)**

  Eliminated the previously stated limitation for Windows Server 2025 domain controllers, indicating migration to sensor v3.x is now supported. This enables broader adoption of v3.x across newer domain controller OS versions.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/migrate-to-sensor-v3

- **Troubleshooting Microsoft Defender for Identity known issues**

  Removed guidance that advised keeping Windows Server 2025 domain controllers on sensor v2.x, reflecting updated migration support to v3.x. This reduces confusion and aligns troubleshooting with current capabilities.

  https://learn.microsoft.com/en-us/defender-for-identity/troubleshooting-known-issues

- **What's new in Microsoft Defender for Identity**

  Added a July 2026 entry announcing support to migrate Windows Server 2025 domain controllers to sensor v3.x and introduced the Sensor Extended RPC Audit tag (requires v3.0.7+) for enhanced RPC-based detections, while removing the prior non-support notice. Also expanded release notes with a new sensor update entry (2.255.19247.44775) that adds Group Policy event collection properties and includes general bug fixes.

  https://learn.microsoft.com/en-us/defender-for-identity/whats-new