# SQL Server
**Date created:** 2026-08-22 UTC  
**Tags:** Best Practices, Configuration, Guidance, Security  

## Major Changes

- **Enable Least Privilege**

  Clarified which Azure Extension for SQL Server versions enable least privilege by default and when manual configuration is required. Documented that the extension creates and manages the NT SERVICE\SqlServerExtension account with only the minimum permissions, revokes them when no longer needed, and removes the account on uninstall or when least privilege is disabled. Updated procedures to enable or disable least privilege via the LeastPrivilege feature flag. Added guidance for optional management of the SQL Server database engine service account, including Deployer.exe behavior, temporary sysadmin needs, NT AUTHORITY\SYSTEM CONNECT SQL requirements, just-in-time permissions, and how to pause automatic upgrades to control permission changes. Verification steps and prerequisites were refined to align with these behaviors.

  https://learn.microsoft.com/en-us/sql/sql-server/azure-arc/configure-least-privilege?view=sql-server-ver17

- **Create a Format File with bcp (SQL Server)**

  Reorganized the article to clearly separate XML and non-XML format files, with step-by-step examples and commands for -c, -n, -N, and -w options. Updated examples to AdventureWorks2025 and improved explanations of qualifiers, field terminators, and trusted connections (-T). Expanded limitations and compatibility guidance for SQL Server 2025 vs. 2022, including format version considerations. Clarified that format files can carry collation/code page metadata that may override code page options, with instructions to remove collation data when needed. Streamlined mapping guidance and refreshed related references for quicker, more accurate setup.

  https://learn.microsoft.com/en-us/sql/relational-databases/import-export/create-a-format-file-sql-server?view=sql-server-ver17