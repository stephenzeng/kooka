# SQL Server
**Date created:** 2026-08-26 UTC  
**Tags:** Guidance, Monitoring, Performance, Troubleshooting  

## Moderate Changes

- **IS [NOT] NULL (Transact-SQL)**
  
  Expanded the article to cover both IS NULL and IS NOT NULL, updating the title and headings for clarity. Clarified terminology and capitalization for NULL to reduce ambiguity. This improves guidance for writing predicate logic and helps users avoid misinterpreting NULL checks.

  https://learn.microsoft.com/en-us/sql/t-sql/queries/is-null-transact-sql?view=sql-server-ver17

- **SQL Server 2025 Known Issues**
  
  Added two issues: an incorrect UTC "Z" qualifier on committime in change event streaming for non-UTC databases (fix pending), and missing database performance counters after DBCC CHECKDB. Documented workarounds, including taking the database offline/online, failing over, or restarting the instance. These updates help administrators diagnose behavior and restore monitoring data more quickly.

  https://learn.microsoft.com/en-us/sql/sql-server/sql-server-2025-known-issues?view=sql-server-ver17