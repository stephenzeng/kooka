# Microsoft Purview
**Date created:** 2026-08-18 UTC  
**Tags:** Compliance, Configuration, Guidance, Monitoring, Security, Troubleshooting  

## New Articles

- **Remove a retention hold from an unlicensed OneDrive site**

  New guidance explains how administrators can remove a blocking retention hold from an unlicensed, archived OneDrive for Business site using Security & Compliance PowerShell. It documents the Fix-PurviewConfig cmdlet with the RemoveHoldFromUnlicencedODBSite scenario, including prerequisites, command syntax, and example output. The article includes a detailed error and validation matrix to troubleshoot issues such as invalid site URLs or policy IDs, non-existent sites or policies, and licensing or applicability mismatches. It also provides verification steps, notes on idempotent behavior, and links to related retention and OneDrive guidance.

  https://learn.microsoft.com/en-us/purview/remove-retention-hold-unlicensed-onedrive-site

## Moderate Changes

- **Audit log activities**

  Added new audit events for Fabric Native PostgreSQL to the Microsoft Fabric activities table, covering schema changes, object browsing, query execution, schema export, sample data import, and audit policy retrieval/updates. This enhances visibility for PostgreSQL operations, improving compliance monitoring and investigation capabilities.

  https://learn.microsoft.com/en-us/purview/audit-log-activities