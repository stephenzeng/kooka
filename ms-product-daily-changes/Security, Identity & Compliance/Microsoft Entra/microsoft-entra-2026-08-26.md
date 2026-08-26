# Microsoft Entra
**Date created:** 2026-08-26 UTC  
**Tags:** Configuration, Guidance, Identity, Security, Troubleshooting  

## Major Changes

- **What is Microsoft single sign-on for Linux?**

  Updated guidance shifts Linux SSO from device registration to Microsoft Entra join for device trust starting with version 2.0.2. Admins must allow target users to join devices; registration settings alone no longer suffice. Instructions and terminology now use “unjoin” instead of “unregister,” with updated dsreg usage and cleanup steps. A new support statement clarifies apps must integrate via MSAL and that direct broker interface use is unsupported, helping ensure compatibility and secure deployments.

  https://learn.microsoft.com/en-us/entra/identity/devices/sso-linux

- **What's new in Microsoft single sign-on for Linux**

  Versions 2.0.2+ now rely on Microsoft Entra join rather than registration to establish device trust. Admins need to enable “Users may join devices to Microsoft Entra,” and upgrades from earlier versions require devices to be re-joined and re-enrolled. Troubleshooting guidance was updated from re-register to re-join to align with the new trust model, and a prior version note was removed to avoid confusion.

  https://learn.microsoft.com/en-us/entra/identity/devices/whats-new-linux

## Moderate Changes

- **Backup, difference report, and recovery model in Microsoft Entra Backup and Recovery**

  Expanded supported objects to explicitly include agent-related resources: agent user accounts, agent identity blueprints, and agent identities/blueprint principals. This improves clarity on what is protected and reported, ensuring agent artifacts are covered across backup, difference reports, and recovery workflows.

  https://learn.microsoft.com/en-us/entra/backup/backup-difference-report-recovery-model

- **Manage device identities using the Microsoft Entra admin center**

  Added a practical tip to verify registration or join settings per operating system when users face device registration/join errors. Updated guidance now reflects that the “Users may join devices” setting applies beyond Windows to include macOS and Linux, with other updates limited to formatting.

  https://learn.microsoft.com/en-us/entra/identity/devices/manage-device-identities

- **Supported objects and recoverable properties in Microsoft Entra Backup and Recovery**

  Clarified that Agent ID objects are included through their underlying directory object types (users, applications, and service principals). Only the documented properties for each object type are backed up, reported, and recoverable, providing precise expectations for coverage.

  https://learn.microsoft.com/en-us/entra/backup/scope-supported-objects-limitations