# SQL Server
**Date created:** 2026-08-11 UTC  
**Tags:** Guidance, Performance, Troubleshooting  

## New Articles

- **Troubleshoot Slow Performance After an Edition Change**

  Introduced a comprehensive guide for diagnosing and resolving performance regressions after changing SQL Server editions. The article outlines a structured workflow, including capturing a SQL LogScout baseline and validating environment parity, to pinpoint edition-related differences. It explains how edition limits and features (compute and buffer pool caps, DOP restrictions, batch mode availability, IQP variations, columnstore optimizations, and Resource Governor) can affect CPU, query times, and maintenance. It provides practical checks using DMVs, Performance Monitor, wait stats, Query Store, and plan comparisons, with clear steps to address memory grant pressure, plan shifts, and I/O changes due to buffer pool limits. The guidance helps teams quickly isolate root causes and apply targeted fixes.

  https://learn.microsoft.com/en-us/troubleshoot/sql/database-engine/performance/troubleshoot-performance-edition-change

## Moderate Changes

- **SET IDENTITY_INSERT (Transact-SQL)**

  Clarified how the current identity value is determined when inserting explicit identity values with positive or negative IDENTITY increments, improving predictability after inserts. Refined introductory and parameter descriptions, with minor updates in Permissions and Examples to tighten accuracy and wording.

  https://learn.microsoft.com/en-us/sql/t-sql/statements/set-identity-insert-transact-sql?view=sql-server-ver17