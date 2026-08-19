# Dev and Admin for Dynamics 365 Business Central
**Date created:** 2026-08-19 UTC  
**Tags:** Automation, Compliance, Configuration, Deprecation, Governance, Guidance, Monitoring  

## Major Changes

- **Business Central Admin Center API - App Management**

  Added new Admin Center API v2.29 capabilities for per-tenant extensions (PTEs), including endpoints to upload and schedule installs/updates, list scheduled actions, and cancel scheduled installs/updates. Clarified scope differences between global app and PTE operations and updated related sections to prevent misuse, including an uninstall note for PTE schedules. Standardized parameter naming and headings, and removed the in-product permissions section to streamline guidance. These changes enable more complete automation of the PTE lifecycle and reduce operational errors.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/administration/administration-center-api_app_management

- **Managing Apps**

  Overhauled Admin Center app management guidance with a capability matrix for Global apps, PTEs, and DEV extensions, and clearer update flows. Clarified that new Global apps are installed from Marketplace, while Admin Center manages updates to the highest compatible version; use the API to target specific versions. Expanded PTE guidance: upload .app packages, select deployment schedules and sync mode, track progress in Operations, and view/cancel scheduled installs, with refined dependency handling and an Action Required state. Added guidance on uninstall behavior and highlighted deprecation of PTE management in the Extension Management page by 2027 release wave 1, helping admins adopt consistent, future-proof processes.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-manage-apps

## Moderate Changes

- **Business Central Admin Center API - Environment database export**

  Marked the Get export history endpoint as deprecated starting with API version 2.30 (supported through 2.29) and directed users to the Environment Operations API for export history. Request and response schemas remain unchanged, helping teams plan migrations without immediate code updates.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/administration/administration-center-api_environment_database_export

- **Auditing events in Microsoft Purview**

  Added new audited activities for PTE operations: “Uploaded PTE” and “Removed Scheduled PTE Version,” including detailed custom dimensions for troubleshooting and governance. Clarified that these audit signals are emitted only for PTE actions via the admin center and its API, improving visibility into extension lifecycle events.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/auditing/audit-events-in-purview

- **Deprecated features in the platform - Clients, Server, and Database**

  Announced deprecation of uploading/installing PTEs from the Extension Management page and Automation API for SaaS, starting in 2026 release wave 1, with removal of the Extension Management upload surface expected in 2027 release wave 1. SaaS admins should use the Admin Center or Admin Center API for PTE lifecycle tasks; on-premises admins should use the Microsoft.Dynamics.Nav.Apps.Management PowerShell module.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/upgrade/deprecated-features-platform

- **Deploy a per-tenant extension**

  Reframed PTE deployment guidance with step-by-step instructions for uploading and scheduling via the Admin Center and the Extension Management page, and recommended sticking to one method for consistent visibility. Clarified behavior for scheduling against the next version, and updated the upgrade policy to explain enforced update periods and automatic uninstalls when an extension blocks updates.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/devenv-deploy-tenant-customization

- **Extension types and scope**

  Clarified that forced uninstalls occur only if an app blocks upgrades during the Enforced Update Period. Expanded PTE installation guidance to include uploading from the Admin Center’s Manage Apps page and noted that upgrades can apply when a newer version is already staged for the target environment update.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/devenv-extension-types-and-scope

- **Export databases in the admin center**

  Updated navigation: export history is now accessed from the Operations page rather than the environment details page. Clarified that only internal and delegated admins with appropriate Entra roles and the D365 BACKUP/RESTORE permission set can export databases, reducing access issues and audit risk.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-database-export