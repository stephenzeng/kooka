# SQL Server
**Change date:** 2026-08-07 UTC  
**Tags:** Administration  

## Moderate Changes

- **sys.sp_updatestats (Transact-SQL)**

  Updated guidance clarifies that for memory-optimized tables, sys.sp_updatestats updates all statistics unconditionally. Added a limitation noting that when Memory-optimized TempDB metadata is enabled, the procedure fails with error 41317 due to cross-database access restrictions—helping administrators avoid unexpected failures. Removed outdated advice that discouraged running sp_updatestats more than necessary for memory-optimized tables.

  https://learn.microsoft.com/en-us/sql/relational-databases/system-stored-procedures/sp-updatestats-transact-sql?view=sql-server-ver17