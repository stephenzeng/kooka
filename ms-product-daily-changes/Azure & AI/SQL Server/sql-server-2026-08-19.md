# SQL Server
**Date created:** 2026-08-19 UTC  
**Tags:** Best Practices, Configuration, Deprecation, Get Started, Governance, Guidance, Monitoring, Performance, Security, Troubleshooting  

## New Articles

- **Change the Schema of a System-Versioned Temporal Table**

  Introduced a how-to guide for altering the schema of temporal tables using ALTER TABLE, including permission requirements and lock behavior on current and history tables. Explains how changes propagate to history, implications of adding large types with defaults, and row-size limits for online operations. Details operations that require disabling SYSTEM_VERSIONING and provides examples for adding/dropping columns, changing sizes, toggling hidden period columns, and performing changes with SYSTEM_VERSIONING OFF within a transaction.

  https://learn.microsoft.com/en-us/sql/relational-databases/tables/temporal/change-schema?view=sql-server-ver17

- **Temporal Table Considerations and Limitations**

  Added a comprehensive overview of temporal table requirements, supported scenarios, and constraints, including object scope, history table rules, unsupported features, and default compression settings. Covers query and DML restrictions, trigger and replication rules, indexing guidance for current and history tables, and properties not replicated when creating history tables. Provides clear security and design guidance to avoid pitfalls and links to related topics.

  https://learn.microsoft.com/en-us/sql/relational-databases/tables/temporal/considerations-limitations?view=sql-server-ver17

- **Temporal Table System Consistency Checks**

  Documented system checks that validate schema and data consistency for temporal tables before enabling versioning and at runtime. Explains required schema parity, period column constraints, and limits on history table objects, plus the ValidTo >= ValidFrom requirement. Warns about manual clock changes impacting checks and notes DBCC CHECKCONSTRAINTS coverage.

  https://learn.microsoft.com/en-us/sql/relational-databases/tables/temporal/consistency-checks?view=sql-server-ver17

- **Create a Memory-Optimized System-Versioned Temporal Table**

  Provided step-by-step guidance to create memory-optimized temporal tables, including prerequisites for memory-optimized filegroups and supported platforms. Shows two approaches: creating with a default disk-based history table or linking to an existing history table. Includes T-SQL examples for SYSTEM_VERSIONING settings, durability options, and DATA_CONSISTENCY_CHECK.

  https://learn.microsoft.com/en-us/sql/relational-databases/tables/temporal/create-memory-optimized?view=sql-server-ver17

- **Get Started with System-Versioned Temporal Tables**

  Introduced an entry point to temporal tables with an overview of versioning behavior and a workflow diagram. Organizes learning into linked how-to articles for creating, modifying, querying, changing schema, and stopping system-versioning. Includes related links to deeper topics like consistency checks, partitioning, security, retention, and memory-optimized support.

  https://learn.microsoft.com/en-us/sql/relational-databases/tables/temporal/get-started?view=sql-server-ver17

- **Manage Historical Data in System-Versioned Temporal Tables**

  Added in-depth guidance for managing history retention with three options: partitioning with a sliding window, a custom cleanup script (with SYSTEM_VERSIONING OFF), and built-in retention policies. Details prerequisites, T-SQL scripts for partition maintenance, chunked deletion patterns, and how engine-side cleanup behaves for rowstore vs clustered columnstore histories. Helps plan operational retention with examples and scheduling recommendations.

  https://learn.microsoft.com/en-us/sql/relational-databases/tables/temporal/manage-retention?view=sql-server-ver17

- **System-Versioned Temporal Tables with Memory-Optimized Tables**

  Explained the architecture that uses an internal memory-optimized staging table with a disk-based history table. Covers constraints (durable only, limitations with native modules) and how the internal table is created and managed, including an extra Change_ID column and reduced max row size. Describes the asynchronous flush mechanism and how to monitor or manually flush history.

  https://learn.microsoft.com/en-us/sql/relational-databases/tables/temporal/memory-optimized?view=sql-server-ver17

- **Memory-Optimized System-Versioned Temporal Table Performance**

  Detailed performance impacts of versioning on memory-optimized tables, including higher memory use and slower updates/deletes. Recommends batching large DML operations or temporarily disabling SYSTEM_VERSIONING when appropriate and explains manual flush options. Suggests clustered columnstore indexes for disk-based history to improve compression and ingestion.

  https://learn.microsoft.com/en-us/sql/relational-databases/tables/temporal/memory-optimized-performance?view=sql-server-ver17

- **Temporal Table Metadata Views and Functions**

  Listed the catalog views and functions to discover temporal table metadata, including sys.tables, sys.columns, sys.periods, and related property functions. Helps administrators and developers script and audit temporal objects consistently.

  https://learn.microsoft.com/en-us/sql/relational-databases/tables/temporal/metadata-views-functions?view=sql-server-ver17

- **Monitor Memory-Optimized System-Versioned Temporal Tables**

  Provided practical T-SQL queries, including CTE-based examples, to analyze memory usage tied to temporal and internal history tables. Helps troubleshoot and plan capacity for memory-optimized temporal scenarios with links to related monitoring guidance.

  https://learn.microsoft.com/en-us/sql/relational-databases/tables/temporal/monitor-memory-optimized?view=sql-server-ver17

- **High Availability and Disaster Recovery**

  Described how the Microsoft ODBC Driver for SQL Server supports Always On availability groups and failover cluster instances. Recommends MultiSubnetFailover=Yes for faster failover and explains parallel IP behavior, safety on single-IP targets, and supported scenarios (Azure SQL, Managed Instance, Fabric, AG listeners, FCI). Covers retry logic, login timeout tuning (especially for serverless), key limitations, read-only routing, and the relevant connection keywords/attributes.

  https://learn.microsoft.com/en-us/sql/connect/odbc/odbc-driver-support-for-high-availability-disaster-recovery?view=sql-server-ver17

- **Partition with Temporal Tables**

  Explained how to use table partitioning with temporal tables and how edition support varies across SQL Server versions. Clarifies allowed and disallowed SWITCH operations with SYSTEM_VERSIONING ON to preserve history consistency. Provides links to broader temporal guidance.

  https://learn.microsoft.com/en-us/sql/relational-databases/tables/temporal/partitioning?view=sql-server-ver17

- **Query Data in a System-Versioned Temporal Table**

  Demonstrated how to use FOR SYSTEM_TIME to query temporal data, including AS OF, FROM…TO, BETWEEN…AND, CONTAINED IN, and ALL. Shows practical patterns such as point-in-time analysis across multiple tables, auditing row changes, and trend analysis with GROUP BY over time windows. Includes handling hidden period columns and applying aliases and views.

  https://learn.microsoft.com/en-us/sql/relational-databases/tables/temporal/query-data?view=sql-server-ver17

- **Temporal Table Security**

  Documented permissions and auditing behavior for enabling, disabling, and querying temporal tables and their histories. Clarifies allowed schema operations with SYSTEM_VERSIONING ON, DROP and partitioning constraints, and distinct SELECT permissions for history tables. Outlines required privileges for creating and altering temporal tables and links to related security topics.

  https://learn.microsoft.com/en-us/sql/relational-databases/tables/temporal/security?view=sql-server-ver17

- **Work with Memory-Optimized System-Versioned Temporal Tables**

  Provided how-to guidance for day-to-day operations with memory-optimized temporal tables. Shows how to discover metadata by joining sys.tables and sys.internal_tables and demonstrates data modifications via a natively compiled stored procedure. Includes links to creation, monitoring, performance, and metadata resources.

  https://learn.microsoft.com/en-us/sql/relational-databases/tables/temporal/work-with-memory-optimized?view=sql-server-ver17

## Major Changes

- **Configurable Retry Logic in SqlClient**

  Overhauled guidance on Microsoft.Data.SqlClient configurable retry logic and clarified that retries are off by default and must be assigned to connections and/or commands. Added a decision path to choose code-based setup, built-in providers, configuration file defaults, or custom providers, plus a detailed checklist for safe policies (bounded retries, jitter, transaction handling, idempotency, and logging). Introduced guidance on client-side timeouts and Azure SQL serverless resume scenarios, including why error -2 is not retried by built-in providers and when to increase timeouts.

  https://learn.microsoft.com/en-us/sql/connect/ado-net/configurable-retry-logic?view=sql-server-ver17

- **Configure Retry Logic in SqlClient**

  Rewrote the intro into a hands-on how-to for configuring built-in retry logic, with prerequisites and a guided setup for an exponential provider. Clarifies NumberOfTries semantics, jittered backoff, and MaxTimeInterval, and adds command retry guidance using AuthorizedSqlCondition. Highlights transaction safety by not retrying commands inside active transactions and explains how customizing TransientErrors replaces the baseline list.

  https://learn.microsoft.com/en-us/sql/connect/ado-net/configurable-retry-logic-sqlclient-introduction?view=sql-server-ver17

- **Built-In Retry Logic Providers in SqlClient**

  Expanded and reorganized provider documentation with a comparison of fixed, incremental, exponential, and none providers, and clarified jitter and retry semantics. Documented the baseline transient error list, how overriding TransientErrors replaces it, and how to extend the baseline using BaselineTransientErrors (v7.0) or source tags for earlier versions. Added guidance on connection vs command errors, client timeouts, and transaction-safe patterns with AuthorizedSqlCondition, plus updated examples and links.

  https://learn.microsoft.com/en-us/sql/connect/ado-net/internal-retry-logic-providers-sqlclient?view=sql-server-ver17

## Moderate Changes

- **Configure SqlClient Retry Logic with a Configuration File**

  Refocused guidance on using app configuration to set default retry providers for SqlConnection and SqlCommand, clarifying that without config or object-level providers, no retries occur. Expanded attribute definitions (numberOfTries ranges, transientErrors replacement semantics, retryMethod and retryLogicType names), updated examples in XML, and noted providers are cached on first use (restart required to apply changes). Clarified fallback to no-retry on config read errors and how to diagnose via event tracing.

  https://learn.microsoft.com/en-us/sql/connect/ado-net/configurable-retry-logic-config-file-sqlclient?view=sql-server-ver17

- **Create a Custom Retry Provider for SqlClient**

  Retitled and refocused instructions on building a custom provider using base classes and assigning it to connections and commands. Clarifies responsibilities for concurrency, cancellation, scheduling, exception handling, and events, and advises favoring built-in providers when possible. Updated examples and limitations, including handling TimeoutException alongside SqlException.

  https://learn.microsoft.com/en-us/sql/connect/ado-net/configurable-retry-logic-core-apis-sqlclient?view=sql-server-ver17

- **Connection options for mssql-django**

  Consolidated updates across connection option docs: clarified where parameter aliases are recognized versus requiring exact parameter names, and distinguished login exchange timeout from dial/connection timeouts. Expanded MultiSubnetFailover guidance, including parallel IP behavior, limits, and compatibility, and updated Azure SQL serverless timeout behavior (possible 40613 and multiple timeouts before resume). Improves reliability by setting accurate expectations and configurations.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-django/connection-options?view=sql-server-ver17

- **go-mssqldb Connection Strings**

  Clarified that parameter aliases apply only to ADO-format strings and that URL/ODBC formats require exact parameter names (case-insensitive). Refined timeout descriptions by separating login exchange from dial timeout and specifying default behaviors, while reiterating the use of Go contexts and retries for serverless resume.

  https://learn.microsoft.com/en-us/sql/connect/golang/connection-strings?view=sql-server-ver17

- **Temporal tables**

  The temporal overview page was moved into a dedicated temporal folder with shorter topic filenames and updated include/image paths; content received minor clarifications and formatting improvements. Additionally, the GitHub Copilot for MSSQL extension overview now explicitly lists support for Azure SQL Database and Azure SQL Managed Instance, clarifying platform scope.

  https://learn.microsoft.com/en-us/sql/relational-databases/tables/temporal/overview?view=sql-server-ver17

- **Release Notes for the Microsoft Drivers for PHP for SQL Server**

  Added release 5.13.3 with the date and new support for installing the drivers on Windows using PIE (PHP Installer for Extensions). Provides example commands for installing sqlsrv and pdo_sqlsrv and clarifies parity with prior Linux and macOS support.

  https://learn.microsoft.com/en-us/sql/connect/php/release-notes-php-sql-driver?view=sql-server-ver17

- **Step 4: Connect resiliently to SQL with ADO.NET**

  Added an important note recommending configurable retry logic in Microsoft.Data.SqlClient 3.0+ over custom loops for new apps. Clarified how to distinguish transient from persistent errors and improved sample setup and run instructions, with minor SQL text cleanup.

  https://learn.microsoft.com/en-us/sql/connect/ado-net/step-4-connect-resiliently-sql-ado-net?view=sql-server-ver17

- **Stop System-Versioning on a System-Versioned Temporal Table**

  Moved and renamed the article into the temporal subfolder and clarified behavior when turning SYSTEM_VERSIONING OFF while keeping the SYSTEM_TIME period. Added an optional step to drop the period to revert to a non-temporal table, updated transaction examples, and clarified requirements when re-enabling versioning.

  https://learn.microsoft.com/en-us/sql/relational-databases/tables/temporal/stop-system-versioning?view=sql-server-ver17

- **Use transparent network IP resolution with the ODBC driver**

  Streamlined content to position TransparentNetworkIPResolution as legacy and clarified it has no effect when MultiSubnetFailover=Yes is used (recommended for Azure SQL and HA). Simplified behavior to enabled vs disabled cases, updated keyword/attribute tables, retitled the article, and added related links.

  https://learn.microsoft.com/en-us/sql/connect/odbc/using-transparent-network-ip-resolution?view=sql-server-ver17