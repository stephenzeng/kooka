# Microsoft Intune
**Date created:** 2026-09-03 UTC  
**Tags:** Best Practices, Configuration, Governance, Guidance, Troubleshooting  

## New Articles

- **Integrate Windows Update client policies**

  Introduced comprehensive guidance for integrating Windows Update client policies (formerly Windows Update for Business) with Configuration Manager, including how update scan sources and categories behave across Windows versions. Clarifies co-management considerations, including the Windows Update policies workload slider and when Configuration Manager stops setting scan source policies. Highlights common pitfalls like partial scan source configurations, legacy Dual Scan artifacts, and conflicting policy providers, with prescriptive remediation. Provides detailed troubleshooting steps using registry paths, PolicyManager, WindowsUpdate.log/WUAHandler.log, and includes a cleanup PowerShell script and version history to aid in rollout and rollback planning.

  https://learn.microsoft.com/en-us/intune/configmgr/sum/deploy-use/integrate-windows-update-client-policies

## Moderate Changes

- **Device Query**

  Updated role requirements by removing eligibility for the Help Desk Operator role and clarifying the need for a custom role that includes the Managed Devices/Query permission plus sufficient read access to view managed devices. Administrators should review role assignments to ensure qualified users retain access to run device queries.

  https://learn.microsoft.com/en-us/intune/advanced-analytics/device-query

- **Device Query for Multiple Devices**

  Simplified the prerequisite and role guidance to emphasize that operators must have permissions to view and access managed devices, with examples such as Organization/Read and Managed devices/Read. This streamlines role design and helps ensure the right level of access without over-specifying individual permissions.

  https://learn.microsoft.com/en-us/intune/advanced-analytics/device-query-multiple-devices