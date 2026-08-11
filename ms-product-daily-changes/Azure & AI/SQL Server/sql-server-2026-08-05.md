# SQL Server
**Date created:** 2026-08-05 UTC  
**Tags:** Administration  

## Moderate Changes

- **Prerequisites - SQL Server enabled by Azure Arc**
  Updated guidance on proxy configuration for the Azure Arc-enabled SQL Server extension. Starting with the April 2024 release (v1.1.2986.256), explicit URL exclusions are no longer required and NO_PROXY can be used to bypass specific endpoints; conditions are provided for earlier versions or when a system HTTPS_PROXY is set. Clarified which addresses may need exclusion to prevent proxying local identity endpoint traffic.
  https://learn.microsoft.com/en-us/sql/sql-server/azure-arc/prerequisites?view=sql-server-ver17

- **Resolve Blocking Problems Caused by Lock Escalation**
  Expanded diagnostics using Extended Events and clearer criteria to confirm when lock escalation is causing blocking. Added actionable prevention strategies—such as breaking large transactions, optimizing queries and indexes, ensuring SARGable predicates—and a practical workaround to suppress escalation by holding a compatible table-level lock on a separate connection. Clarified when to disable escalation and related trace flag behaviors, while emphasizing prevention-first guidance.
  https://learn.microsoft.com/en-us/troubleshoot/sql/database-engine/performance/resolve-blocking-problems-caused-lock-escalation

- **Understand and Resolve SQL Server Blocking Problems**
  Retitled and reorganized the article with a stronger SQL Server focus and clearer troubleshooting flow to identify head blockers and long-running transactions. Improved DMV guidance with examples, recommended Extended Events over deprecated SQL Trace, and refined common scenarios with concrete resolutions. Enhanced explanations of wait types and practical fixes, including transaction handling options and Query Store usage.
  https://learn.microsoft.com/en-us/troubleshoot/sql/database-engine/performance/understand-resolve-blocking