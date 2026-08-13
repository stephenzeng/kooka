# Microsoft Purview
**Date created:** 2026-08-13 UTC  
**Tags:** Compliance, Configuration, Monitoring, Troubleshooting  

## Major Changes

- **Audit log activities**

  Expanded coverage of audit events by adding two Microsoft Fabric activities for tenant-admin connection role changes and introducing a comprehensive People Skills (Viva) activities section. The new entries capture key lifecycle actions such as skill creation, updates, deletions, ingestion, exports, tenant settings changes, and provisioning/offboarding. These additions improve visibility for investigations and strengthen compliance and governance auditing across Fabric and Viva workloads.

  https://learn.microsoft.com/en-us/purview/audit-log-activities

## Moderate Changes

- **Automatically apply a sensitivity label to Microsoft 365 data**

  Added targeted troubleshooting for “Policy rule fails to load” in Exchange email, including how to identify a malformed rule, remove and recreate it, validate via simulation and new messages, and account for temporary enforcement gaps. Enhanced PowerShell guidance references Get/Remove/New-AutoSensitivityLabelRule and clarifies using Connect-IPPSSession with EnableSearchOnlySession to correctly start or rerun auto-labeling simulations.

  https://learn.microsoft.com/en-us/purview/apply-sensitivity-label-automatically