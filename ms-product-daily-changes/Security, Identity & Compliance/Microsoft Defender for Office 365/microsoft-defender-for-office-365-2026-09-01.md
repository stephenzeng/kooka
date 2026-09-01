# Microsoft Defender for Office 365
**Date created:** 2026-09-01 UTC  
**Tags:** Guidance, Security  

## Moderate Changes

- **Manage quarantined messages and files as an admin**

  Clarified that PermissionTo* values from Get-QuarantineMessage reflect the permissions of the account running the cmdlet, not end-user capabilities. Explained scenarios where admins may see PermissionToRelease, PermissionToAllowSender, and PermissionToDownload as True even when AdminOnlyAccessPolicy limits end-user actions. Directed admins to use Get-QuarantinePolicy to verify actual end-user permissions, with a pointer to the View quarantine policies in PowerShell section.

  https://learn.microsoft.com/en-us/defender-office-365/quarantine-admin-manage-messages-files