# Microsoft Intune
**Date created:** 2026-08-19 UTC  
**Tags:** Configuration, Governance, Guidance  

## Moderate Changes

- **Device Action: Delete**

  Clarified a tenant-wide daily limit of 1,000 Delete actions, counted cumulatively across individual device actions, bulk actions, and Microsoft Graph API requests. Noted that the limit applies even when Delete initiates Retire or Wipe, helping admins plan large-scale operations. Added guidance to request limit changes through Microsoft support and referenced the Daily tenant limits documentation for details.

  https://learn.microsoft.com/en-us/intune/device-management/actions/delete

- **Device Actions - Wipe, Lock, Locate, and More**

  Introduced a new Daily tenant limits section specifying per-tenant caps: Wipe (500), Retire (1,000), and Delete (1,000). Clarified that limits are cumulative across individual, bulk, and API submissions, and updated bulk action guidance to state these operations count toward the daily limits.

  https://learn.microsoft.com/en-us/intune/device-management/actions/

- **Device Action: Retire**

  Added an IMPORTANT note establishing a tenant-wide daily limit of 1,000 Retire actions across individual, bulk, and API methods. Provided direction to contact Microsoft support to request limit adjustments and linked to the Daily tenant limits page to aid capacity planning.

  https://learn.microsoft.com/en-us/intune/device-management/actions/retire

- **Device Action: Wipe**

  Documented a tenant-wide daily limit of 500 Wipe actions, aggregated across individual, bulk, and Graph API requests. Included guidance on requesting limit changes via Microsoft support and a reference to the Daily tenant limits page for governance and planning.

  https://learn.microsoft.com/en-us/intune/device-management/actions/wipe