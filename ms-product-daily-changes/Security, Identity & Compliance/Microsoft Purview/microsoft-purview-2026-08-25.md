# Microsoft Purview
**Date created:** 2026-08-25 UTC  
**Tags:** Compliance, Configuration, Governance, Security  

## New Articles

- **Permanently delete files with Microsoft Purview Priority Cleanup**

  Introduced a new capability to permanently delete files in SharePoint and OneDrive using Priority Cleanup. Outlines prerequisites and readiness steps, including required roles, enabling auditing in advance, and feature availability considerations. Highlights safeguards and risks, noting that permanent deletion can bypass retention policies and eDiscovery holds, with guidance on when review set items are exempt. Provides end-to-end setup, approval workflow, and monitoring guidance, including use of cleanup IDs and audit logs.

  https://learn.microsoft.com/en-us/purview/priority-cleanup-permanent-deletion

## Moderate Changes

- **Assign permissions in eDiscovery**

  Updated app-only authentication guidance to use Microsoft Exchange Online Protection’s Exchange.ManageAsApp permission, clarifying that Office 365 Exchange Online permission is not required for Security & Compliance PowerShell. Improved setup by adding explicit navigation steps, recommending a descriptive -DisplayName when creating the service principal, and clarifying role group visibility and assignment using the enterprise app Object ID. Refined troubleshooting to direct HTTP 401 errors to the correct permission path.

  https://learn.microsoft.com/en-us/purview/edisc-permissions