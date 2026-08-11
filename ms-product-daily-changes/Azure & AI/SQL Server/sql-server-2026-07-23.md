# SQL Server
**Date created:** 2026-07-23 UTC  
**Tags:** Administration, Programming, Security  

## Major Changes

- **SET ARITHABORT (Transact-SQL)**

  Clarified how SET ARITHABORT behaves, including its interaction with ANSI_WARNINGS and its effects on query plan caching differences between SSMS and client apps. Expanded guidance details outcomes for arithmetic errors during DML, reiterates that ARITHABORT OFF isn’t supported in Azure Synapse dedicated SQL pools, and adds an explicit Permissions section. Added structured, step-by-step examples covering divide-by-zero and overflow scenarios under different settings, and updated syntax to include Microsoft Fabric SQL DB. These updates help developers predict error handling behavior and avoid unexpected performance or compatibility issues.

  https://learn.microsoft.com/en-us/sql/t-sql/statements/set-arithabort-transact-sql?view=sql-server-ver17

## Moderate Changes

- **Operate SQL Server enabled by Azure Arc with least privilege**

  Updated prerequisites to require Windows Server 2016 or later and SQL Server 2014 or later. This ensures least-privilege guidance aligns with currently supported platforms and reduces configuration issues.

  https://learn.microsoft.com/en-us/sql/sql-server/azure-arc/configure-least-privilege?view=sql-server-ver17

- **Migration to Azure SQL Managed Instance - SQL Server migration in Azure Arc**

  Raised the minimum supported starting version for Azure Arc-enabled migrations to SQL Managed Instance from SQL Server 2012 (v11) to SQL Server 2014 (v14). This narrows eligibility to supported sources and helps teams plan upgrades before migrating.

  https://learn.microsoft.com/en-us/sql/sql-server/azure-arc/migrate-to-azure-sql-managed-instance?view=sql-server-ver17

- **Migration to SQL Server on Azure VMs - SQL Server migration in Azure Arc**

  Increased the minimum supported SQL Server source version for Azure Arc-enabled migration availability from 2012 to 2014. This clarifies migration readiness and prevents attempts from unsupported versions.

  https://learn.microsoft.com/en-us/sql/sql-server/azure-arc/migrate-to-sql-server-on-azure-vms?view=sql-server-ver17

- **Assess migration readiness - SQL Server enabled by Azure Arc**

  Clarified that Windows Server versions earlier than 2016 aren’t supported and raised the minimum supported SQL Server version from 2012 to 2014. These updates refine assessment criteria so organizations can accurately validate readiness.

  https://learn.microsoft.com/en-us/sql/sql-server/azure-arc/migration-assessment?view=sql-server-ver17

- **SQL Server migration in Azure Arc Overview**

  Updated migration availability guidance to set the baseline source version at SQL Server 2014 instead of 2012. This aligns the overview with current support policies and helps teams scope supported scenarios.

  https://learn.microsoft.com/en-us/sql/sql-server/azure-arc/migration-overview?view=sql-server-ver17

- **SET ARITHIGNORE (Transact-SQL)**

  Expanded documentation to clarify suppression of divide-by-zero and overflow messages, detailed interactions with ARITHABORT and ANSI_WARNINGS, and added instructions to view the current setting via @@OPTIONS. Platform-specific syntax was separated, examples were broadened, and Synapse/PDW support clarified. These changes make it easier to configure predictable error handling across environments.

  https://learn.microsoft.com/en-us/sql/t-sql/statements/set-arithignore-transact-sql?view=sql-server-ver17

- **Troubleshoot connectivity to the data processing service and telemetry endpoints**

  Consolidated OS guidance to require Windows Server 2016 or later for telemetry endpoints and aligned notes to remove conflicting statements. This simplifies TLS/OS compatibility requirements and reduces setup confusion.

  https://learn.microsoft.com/en-us/sql/sql-server/azure-arc/troubleshoot-telemetry-endpoint?view=sql-server-ver17