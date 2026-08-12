# SQL Server
**Date created:** 2026-08-12 UTC  
**Tags:** Analytics, Best Practices, Configuration, Get Started, Guidance, Monitoring, Performance, Security, Troubleshooting  

## Major Changes

- **Microsoft.Data.SqlClient for SQL Server**
  The article was overhauled to emphasize Microsoft.Data.SqlClient as the supported .NET provider and to guide production-ready use across SQL Server, Azure SQL, Managed Instance, Synapse, and Fabric. It introduces a structured “Choose your starting point” path to setup, auth, resiliency, bulk copy, migration from System.Data.SqlClient, and troubleshooting. A comprehensive C# example demonstrates secure connection strings, Entra ID/managed identity, TLS/TDS 8.0 encryption, idle connection resiliency, configurable retries with logging, and MultiSubnetFailover usage for high availability. Content is reorganized into practical sections and older moniker-based walkthroughs were removed in favor of targeted guidance and references.
  https://learn.microsoft.com/en-us/sql/connect/ado-net/microsoft-ado-net-sql-server?view=sql-server-ver17

## Moderate Changes

- **mssql-django configuration reference**
  Expanded guidance for OPTIONS.connection_timeout to account for Azure SQL Database serverless with auto-pause; initial connections can take 30–60+ seconds while the database resumes. Recommends setting at least 60 seconds to avoid premature failures during cold starts.
  https://learn.microsoft.com/en-us/sql/connect/python/mssql-django/configuration-reference?view=sql-server-ver17

- **Connection options for mssql-django**
  Updated connection guidance to enable MultiSubnetFailover (safe even on single-IP targets) for Azure SQL, Managed Instance, Microsoft Fabric SQL databases, AG listeners, and FCIs, and clarified default/alias behavior. Clarified that a timeout of 0 defers to the ODBC driver default, recommended setting explicit positive timeouts, and advised longer timeouts or retries for serverless databases resuming from auto-pause. Improved parameter explanations and network/performance guidance, including aliases and behaviors for connection resiliency.
  https://learn.microsoft.com/en-us/sql/connect/python/mssql-django/connection-options?view=sql-server-ver17

- **go-mssqldb Connection Strings**
  Clarified connection timeout behavior for Azure SQL Database serverless with auto-pause, where the first connection may fail with error 40613 during resume. Recommends implementing retry logic instead of simply increasing timeouts and links to auto-pause/auto-resume guidance.
  https://learn.microsoft.com/en-us/sql/connect/golang/connection-strings?view=sql-server-ver17

- **Display an actual execution plan**
  Expanded applicability to include additional Fabric services and added the =fabric moniker, and reorganized related Synapse dedicated SQL pool guidance. Clarified required permissions and refined instructional wording without changing procedural steps.
  https://learn.microsoft.com/en-us/sql/relational-databases/performance/display-an-actual-execution-plan?view=sql-server-ver17

- **File-snapshot backups for database files in Azure**
  Substantially refreshed and reorganized content, clarifying how file-snapshot backups work and emphasizing backup-to-URL recommendations with updated architecture visuals. Expanded restore guidance (to backup time and point-in-time) and consolidated maintenance procedures for deleting backup sets and orphaned snapshots with relevant system procedures and functions. Added detailed considerations and limitations (premium storage cadence, snapshot caps, storage account requirements, bulk-logged implications, restore constraints, billing impacts) and updated examples and links for clarity.
  https://learn.microsoft.com/en-us/sql/relational-databases/backup-restore/file-snapshot-backups-for-database-files-in-azure?view=sql-server-ver17

- **The msdb Database**
  Rewrote the introduction to highlight msdb’s role for Agent jobs, alerts, backup history, Service Broker, and Database Mail, and added explicit recovery model guidance. Reorganized sections and strengthened recommendations on backups, avoiding user objects, security, job ownership, and auditing, while clarifying unsupported operations.
  https://learn.microsoft.com/en-us/sql/relational-databases/databases/msdb-database?view=sql-server-ver17

- **queryinsights.exec_requests_history (Transact-SQL)**
  Added the is_accelerated column to indicate when query acceleration was applied and updated terminology to reference Fabric Data Warehouse. Clarified permission requirements and corrected examples and view name references.
  https://learn.microsoft.com/en-us/sql/relational-databases/system-views/queryinsights-exec-requests-history-transact-sql?view=fabric

- **queryinsights.frequently_run_queries (Transact-SQL)**
  Documented a new number_of_accelerated_runs column that reports how many times a query was accelerated. Other updates were editorial cleanups for clarity.
  https://learn.microsoft.com/en-us/sql/relational-databases/system-views/queryinsights-frequently-run-queries-transact-sql?view=fabric

- **queryinsights.long_running_queries (Transact-SQL)**
  Added a new number_of_accelerated_runs column to show the total count of accelerated executions. This helps analyze performance impact of acceleration on long-running queries.
  https://learn.microsoft.com/en-us/sql/relational-databases/system-views/queryinsights-long-running-queries-transact-sql?view=fabric

- **Release Notes for the Microsoft Drivers for PHP for SQL Server**
  Added the 5.13.2 release with Windows download and GitHub tag, plus support for installing via PIE in addition to PECL. Addressed a SQL injection vulnerability in PDO::lastInsertId() and multiple fixes, including binary parameter truncation with emulated prepares, Windows ZTS link issues, unixODBC INI cache handling, AddressSanitizer ODR conflicts, and CodeQL findings.
  https://learn.microsoft.com/en-us/sql/connect/php/release-notes-php-sql-driver?view=sql-server-ver17

- **go-mssqldb Troubleshooting**
  Expanded the 40613 error guidance to include initial connection failures while an Azure SQL Database serverless database is resuming from auto-pause. Emphasizes implementing retry logic and references retry patterns and auto-pause/auto-resume documentation.
  https://learn.microsoft.com/en-us/sql/connect/golang/troubleshooting?view=sql-server-ver17