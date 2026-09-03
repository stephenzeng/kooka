# Microsoft Defender XDR
**Date created:** 2026-09-03 UTC  
**Tags:** Analytics, Governance, Security  

## Moderate Changes

- **EmailEvents table in the advanced hunting schema**

  Added new EmailEvents columns to capture delivery-time verdicts, detection methods, and confidence levels, plus granular multi-label topic classifications. These fields provide historical context for investigations, enable more precise filtering and correlation, and help analysts identify trends and false positives more effectively.

  https://learn.microsoft.com/en-us/defender-xdr/advanced-hunting-emailevents-table

- **Create custom detection rules in Microsoft Defender XDR**

  Updated guidance to enable governance actions on SaaS identities using queries that leverage the CloudAppEvents table (preview), including required output columns and allowance for joins. Documented supported services and actions (Box: Disable user; Google Workspace: Disable user, Force password reset; Salesforce: Disable user) and clarified that no action is taken if the selected action or service isn’t supported. This helps automate response for SaaS threats while avoiding unsupported operations.

  https://learn.microsoft.com/en-us/defender-xdr/custom-detection-rules