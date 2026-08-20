# SQL Server
**Date created:** 2026-08-20 UTC  
**Tags:** Best Practices, Configuration, Get Started, Guidance, Performance, Troubleshooting  

## New Articles

- **Format T-SQL in the MSSQL Extension for Visual Studio Code**

  Introduced a how-to guide for the new SQL formatter (Preview) in the MSSQL VS Code extension, covering on-demand formatting, format-on-save, and making MSSQL the default formatter. Detailed configuration options with example settings.json snippets, organized by categories such as Alignment, Indentation, Multiline, Spacing, and more. Documented that the formatter is powered by ScriptDOM and provided links to related quickstart and overview content to help users adopt consistent coding standards.

  https://learn.microsoft.com/en-us/sql/tools/visual-studio-code-extensions/mssql/mssql-sql-formatter?view=sql-server-ver17

## Major Changes

- **Manage retention of historical data in system-versioned temporal tables**

  Overhauled guidance on planning and operating temporal history retention, clarifying that cleanup is based on the ValidTo (end-of-period) column. Added end-to-end instructions for using a retention policy, including database-level enablement, table-level HISTORY_RETENTION_PERIOD, supported units, catalog inspection, and background cleanup behavior. Expanded mechanics and constraints for B-tree and clustered columnstore history tables, including index requirements, chunked deletions, and ordering considerations. Enhanced partitioning guidance with a sliding window design (RANGE LEFT), step-by-step maintenance (SWITCH/MERGE/SPLIT), updated scripts, and performance implications to avoid data movement. Refactored custom cleanup patterns with operational steps, chunk sizing, and scheduling to minimize workload impact.

  https://learn.microsoft.com/en-us/sql/relational-databases/tables/temporal/manage-retention?view=sql-server-ver17

## Moderate Changes

- **Decreased performance for SQL Server when you run a TOP, MAX, or MIN aggregating clause on columns other than the partitioning column**

  Corrected and reformatted the sample query to improve accuracy and readability, including fixing the OBJECT_ID call and aligning ORDER BY with the intended alias. These changes make the example easier to follow and prevent confusion when reproducing guidance.

  https://learn.microsoft.com/en-us/troubleshoot/sql/database-engine/performance/decreased-performance-run-aggregating-clause

- **IDENT_CURRENT (Transact-SQL)**

  Expanded and clarified the reference, including a new Exceptions section that calls out NULL behavior and permissions, and improved comparisons with @@IDENTITY and SCOPE_IDENTITY. Added a note that IDENT_CURRENT isn’t available for identity columns in Fabric Data Warehouse and refreshed examples and related links for easier navigation.

  https://learn.microsoft.com/en-us/sql/t-sql/functions/ident-current-transact-sql?view=sql-server-ver17

- **IDENT_INCR (Transact-SQL)**

  Clarified the description to explicitly state the function returns the identity increment and added supported platform/version details. Introduced a Remarks note that IDENT_INCR isn’t available for identity columns in Fabric Data Warehouse and streamlined sections for readability.

  https://learn.microsoft.com/en-us/sql/t-sql/functions/ident-incr-transact-sql?view=sql-server-ver17

- **@@IDENTITY (Transact-SQL)**

  Added a note that @@IDENTITY isn’t available for identity columns in Fabric Data Warehouse. This clarification helps avoid unsupported usage in Fabric DW scenarios.

  https://learn.microsoft.com/en-us/sql/t-sql/functions/identity-transact-sql?view=sql-server-ver17

- **IDENT_SEED (Transact-SQL)**

  Clarified function behavior, added supported platform/version scope, and reorganized the page with clear sections for syntax, arguments, return types, exceptions, and examples. Noted that IDENT_SEED isn’t available for identity columns in Fabric Data Warehouse and consolidated related links to streamline discovery.

  https://learn.microsoft.com/en-us/sql/t-sql/functions/ident-seed-transact-sql?view=sql-server-ver17

- **Create an Azure SQL Database**

  Removed the Preview designation from the title and preview notice to reflect general availability. This signals production readiness without changing existing steps or feature descriptions.

  https://learn.microsoft.com/en-us/sql/tools/visual-studio-code-extensions/mssql/mssql-azure-integration?view=sql-server-ver17

- **MSSQL extension for Visual Studio Code**

  Updated the feature overview to include the SQL Formatter (Preview) and promoted Azure integration and Shortcuts Configuration to GA. Clarified that the new Results Grid is enabled by default and explained how to adjust the mssql.preview.betaResultsGrid setting.

  https://learn.microsoft.com/en-us/sql/tools/visual-studio-code-extensions/mssql/mssql-extension-visual-studio-code?view=sql-server-ver17

- **sys.sp_adddistributor (Transact-SQL)**

  Added an optional @multi_subnet_failover parameter to control the MultiSubnetFailover setting on the dynamic linked server between a publisher and remote distributor. Guidance recommends enabling it for AG listeners or multi-subnet FCIs to improve failover reconnection and reduce timeouts; availability starts with CU 8 and later.

  https://learn.microsoft.com/en-us/sql/relational-databases/system-stored-procedures/sp-adddistributor-transact-sql?view=sql-server-ver17

- **SQL Server 2025 release notes**

  Replaced the inline GA build/version/date table with a link to the centralized SQL Server 2025 build versions article. This consolidates build information for easier maintenance and ensures readers always access the most current build details.

  https://learn.microsoft.com/en-us/sql/sql-server/sql-server-2025-release-notes?view=sql-server-ver17