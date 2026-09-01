# Microsoft Defender XDR
**Date created:** 2026-09-01 UTC  
**Tags:** Configuration, Guidance, Governance, Identity, Monitoring, Security  

## Major Changes

- **Investigate data loss prevention alerts with Microsoft Defender XDR**

  Added guidance on a built-in alert tuning rule that will convert DLP signals into behaviors (not alerts) starting in early October 2026, affecting alert volumes and incident workflows. Clarified that these signals remain queryable in advanced hunting via the BehaviorInfo and BehaviorEntities tables, and provided steps to disable the rule if you need to continue receiving DLP signals as alerts. Updated guidance to reflect that DLP alert/incident management applies when the rule is disabled, removed outdated instructions about support cases, and linked to related content on built-in alert tuning rules.

  https://learn.microsoft.com/en-us/defender-xdr/dlp-investigate-alerts-defender

## Moderate Changes

- **Create custom roles with Microsoft Defender unified RBAC**

  Added a “Remote tenant group” assignment option that lets you select GDAP remote tenant groups whose members inherit the configured permissions, data source access, and scopes. This enables extending unified RBAC to external tenants for centralized governance and simpler cross-tenant administration.

  https://learn.microsoft.com/en-us/defender-xdr/create-custom-rbac-roles