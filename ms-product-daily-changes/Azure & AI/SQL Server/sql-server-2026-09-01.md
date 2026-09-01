# SQL Server
**Date created:** 2026-09-01 UTC  
**Tags:** Billing, Configuration, Deprecation, Guidance, Licensing, Security, Troubleshooting  

## Major Changes

- **Check ODBC Driver Installation and DSN Configuration in Windows**

  Substantially expanded guidance clarifies when to use the 32-bit vs. 64-bit ODBC Data Source Administrator and why driver bitness must match the application. Updated connection string examples (DSN and DSN-less) and recommends using the Microsoft ODBC Driver for SQL Server instead of legacy drivers. Adds detailed verification steps and registry paths for drivers and DSNs, including validating DLL locations, plus a structured checklist for IM002 (DSN not found/no default driver) and Procmon tracing tips. These improvements make it easier to diagnose configuration issues and adopt supported drivers.

  https://learn.microsoft.com/en-us/troubleshoot/sql/database-engine/install/windows/odbc-driver-install-checking

- **End of Support Options**

  Expanded end-of-support choices to include Azure SQL Database alongside Azure SQL Managed Instance and Azure Virtual Machines, with clearer paths to upgrade during migration or use ESUs when staying on current environments. Introduces a modernization section for Azure SQL Database Hyperscale outlining benefits (elastic scale, fast backup/restore, read scale-out) and key considerations, resources, and migration tools. Adds a decision aid linking to the Azure SQL Decision Tree and updates the options summary table, emphasizing that fully managed PaaS offerings don’t reach end of support. Clarifies ESU guidance for planning upgrades or migrations while remaining on existing platforms.

  https://learn.microsoft.com/en-us/sql/sql-server/end-of-support/sql-server-end-of-support-overview?view=sql-server-ver17

## Moderate Changes

- **Set trace flags with DBCC TRACEON (Transact-SQL)**

  Added trace flag 4671 to enable PBKDF2 (RFC 2898) password verifiers with 100,000 SHA-512 iterations in SQL Server 2022 starting with CU12, improving SQL authentication security. The article clarifies upgrade behavior: verifiers update on password change and don’t downgrade if the flag is later disabled. It also notes compatibility limits with earlier builds, applicability (unnecessary in SQL Server 2025), scope (global or session), and rollback guidance when reverting.

  https://learn.microsoft.com/en-us/sql/t-sql/database-console-commands/dbcc-traceon-trace-flags-transact-sql?view=sql-server-ver17

- **Manage licensing and billing of SQL Server enabled by Azure Arc**

  Clarified eligibility for Azure Arc–enabled SQL Server PAYG customers to use Power BI Report Server or SQL Server Reporting Services. Since PAYG activation isn’t available today, eligible customers may need a product key and should open a Microsoft Support request to validate eligibility and obtain the key.

  https://learn.microsoft.com/en-us/sql/sql-server/azure-arc/manage-license-billing?view=sql-server-ver17