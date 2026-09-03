# Power Apps
**Date created:** 2026-09-03 UTC  
**Tags:** Configuration, Guidance, Performance, Troubleshooting  

## Moderate Changes

- **Azure Synapse Link for Dataverse trouble shooting guide**

  Expanded troubleshooting for SYN-805 to include checks for managed virtual networks, Synapse IP firewall rules, and public network access restrictions. Added links to connectivity and firewall configuration docs to speed diagnosis and resolution. This helps admins quickly identify network blocks that prevent access to the Synapse workspace.

  https://learn.microsoft.com/en-us/power-apps/maker/data-platform/azure-synapse-link-troubleshooting-guide

- **Delete Data in Bulk to Reduce Storage Use**

  Updated guidance to replace “recycle bin” with “deleted record keeping” and clarified how CanRecoverDeletedRecords depends on environment-level settings. Clarified that RunJobForSandbox is supported only in sandbox; other environments use the standard pipeline without errors and continue to honor plug-ins, workflows, and deleted record keeping. These changes help admins avoid unintended permanent deletions and correctly plan bulk delete behavior across environments.

  https://learn.microsoft.com/en-us/power-apps/developer/data-platform/delete-data-bulk

- **Troubleshooting common issues with link to Fabric**

  Added a new cause for invalid Fabric-to-Dataverse connection errors when the original data connection was deleted or its creator account was removed. Provided steps to unlink and recreate the Fabric link to generate a new connection, with a pointer to the setup guidance. This streamlines recovery from broken connections caused by account or resource removal.

  https://learn.microsoft.com/en-us/power-apps/maker/data-platform/fabric-troubleshoot