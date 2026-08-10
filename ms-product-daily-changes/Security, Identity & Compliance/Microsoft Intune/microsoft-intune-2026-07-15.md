# Microsoft Intune
**Date created:** 2026-07-15 UTC  
**Tags:** Administration, Security  

## Major Changes

- **Modify infrastructure**

  Added critical guidance that the “Modify SQL Server configuration” maintenance path doesn’t validate SQL Server collation and that admins must ensure both the instance and site database use SQL_Latin1_General_CP1_CI_AS (with exceptions for China GB18030 collations). Introduced a new section with a comprehensive SQL script to verify required settings, including instance and database collation, CLR, max text replication size, database owner, TRUSTWORTHY, Service Broker, and Service Broker priority. Enhanced the “Move the site database” steps to require running the verification script and confirming collation before proceeding. These updates help prevent failed moves or upgrades and ensure environments remain in a supported state.

  https://learn.microsoft.com/en-us/intune/configmgr/core/servers/manage/modify-your-infrastructure

## Moderate Changes

- **Multiple managed accounts for app protection policies**

  Expanded the supported apps list to include Microsoft Teams (iOS/iPadOS) minimum v8.10.0 and newly added Microsoft Outlook (iOS/iPadOS) minimum v5.2626.0. Replaced the prior single-app statement with guidance that more apps and platforms are coming soon, helping admins plan broader app protection policy adoption.

  https://learn.microsoft.com/en-us/intune/app-management/protection/multiple-managed-accounts

- **Task sequence steps**

  Clarified that embedding a signed PowerShell script via “Enter a PowerShell script” can break the signature under the AllSigned policy due to byte changes in task sequence XML. Recommended distributing the signed .ps1 in a Configuration Manager package and referencing it by Package and Script name to preserve the original bytes and ensure execution under AllSigned.

  https://learn.microsoft.com/en-us/intune/configmgr/osd/understand/task-sequence-steps