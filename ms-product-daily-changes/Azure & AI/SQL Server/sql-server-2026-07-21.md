# SQL Server
**Date created:** 2026-07-21 UTC  
**Tags:** AI, Administration, Analytics, Monitoring, Other, Programming, Security  

## New Articles

- **SQL Server 2016: Hardware and Software Requirements**

  Introduced a comprehensive requirements guide for SQL Server 2016, covering supported Windows versions, .NET prerequisites, and detailed hardware guidance for CPU, memory, storage, and disk sector sizes. Added OS compatibility matrices, Server Core and WOW64 considerations, and feature-level drive space requirements. Included guidance for installations on domain controllers and supported storage scenarios, plus links to planning and security resources to streamline deployment decisions.

  https://learn.microsoft.com/en-us/sql/sql-server/install/hardware-and-software-requirements-for-installing-sql-server-2016?view=sql-server-ver17

## Major Changes

- **SQL Server 2017: Hardware and Software Requirements**

  Retargeted the article to SQL Server 2017 only, updating the title and description for clarity. Removed SQL Server 2016-specific matrices and sections, including OS support and Server Core details, to prevent misapplication. Adjusted headings to reflect 2017-only coverage so readers reference current prerequisites and supported platforms.

  https://learn.microsoft.com/en-us/sql/sql-server/install/hardware-and-software-requirements-for-installing-sql-server-2017?view=sql-server-ver17

- **Install SQL Server from the Installation Wizard (Setup)**

  Narrowed scope to SQL Server 2017 and later by updating moniker ranges and converting version-selector blocks to 2017 only. Removed SQL Server 2016 references in headings and navigation, and revised the patch requirement section to apply solely to SQL Server 2017 (not applicable to 2019+). This improves accuracy and reduces confusion when following setup steps for supported versions.

  https://learn.microsoft.com/en-us/sql/database-engine/install-windows/install-sql-server-from-the-installation-wizard-setup?view=sql-server-ver17

## Moderate Changes

- **Add and Remove Publishers from Replication Monitor**

  Updated applicability to SQL Server 2017 and later, removing SQL Server 2016 from support. No procedural or conceptual guidance was changed.

  https://learn.microsoft.com/en-us/sql/relational-databases/replication/monitor/add-and-remove-publishers-from-replication-monitor?view=sql-server-ver17

- **A Guide to Query Processing for Memory-Optimized Tables**

  Raised the minimum supported version to SQL Server 2017 and normalized operator spacing. The guidance remains unchanged.

  https://learn.microsoft.com/en-us/sql/relational-databases/in-memory-oltp/a-guide-to-query-processing-for-memory-optimized-tables?view=sql-server-ver17

- **Audit Database Management Event Class**

  Updated applicability to start at SQL Server 2017 while keeping Azure SQL Database and Azure SQL Managed Instance coverage. Clarified version targeting without altering event semantics.

  https://learn.microsoft.com/en-us/sql/relational-databases/event-classes/audit-database-management-event-class?view=sql-server-ver17

- **Change the database compatibility level and use the Query Store**

  Raised the minimum supported version to SQL Server 2017, removing SQL Server 2016 from scope. Instructions and recommendations are unchanged.

  https://learn.microsoft.com/en-us/sql/database-engine/install-windows/change-the-database-compatibility-mode-and-use-the-query-store?view=sql-server-ver17

- **Collation and Unicode support**

  Updated version applicability to SQL Server 2017 and later. Content remains the same.

  https://learn.microsoft.com/en-us/sql/relational-databases/collations/collation-and-unicode-support?view=sql-server-ver17

- **Troubleshoot issues with Launchpad service executing Python and R scripts in SQL Server Machine Learning Services**

  Updated all moniker ranges to require SQL Server 2017 and later, aligning scoped notes and sections accordingly. No changes to troubleshooting steps or guidance.

  https://learn.microsoft.com/en-us/sql/machine-learning/troubleshooting/common-issues-external-script-execution?view=sql-server-ver17

- **Configure SQL Server Agent mail to use Database Mail**

  Set minimum version to SQL Server 2017 for applicability, maintaining Linux and Azure SQL MI targets. Steps and configuration guidance are unchanged.

  https://learn.microsoft.com/en-us/sql/relational-databases/database-mail/configure-sql-server-agent-mail-to-use-database-mail?view=sql-server-ver17

- **Connect to an Instance of SQL Server**

  Raised the minimum supported version to SQL Server 2017. The connection steps and examples are unchanged.

  https://learn.microsoft.com/en-us/sql/relational-databases/server-management-objects-smo/create-program/connecting-to-an-instance-of-sql-server?view=sql-server-ver17

- **Create an application role**

  Updated monikers to start at SQL Server 2017 and equivalent cloud offerings, removing SQL Server 2016. The process to create and use application roles is unchanged.

  https://learn.microsoft.com/en-us/sql/relational-databases/security/authentication-access/create-an-application-role?view=sql-server-ver17

- **Create check constraints**

  Adjusted applicability to begin at SQL Server 2017. The constraint creation guidance remains the same.

  https://learn.microsoft.com/en-us/sql/relational-databases/tables/create-check-constraints?view=sql-server-ver17

- **Database Engine events and errors (13000 to 13999)**

  Set applicability to SQL Server 2017 and later. Error reference content is unchanged.

  https://learn.microsoft.com/en-us/sql/relational-databases/errors-events/database-engine-events-and-errors-13000-to-13999?view=sql-server-ver17

- **DATEFROMPARTS (Transact-SQL)**

  Updated support to SQL Server 2017 and later. Function behavior and examples are unchanged.

  https://learn.microsoft.com/en-us/sql/t-sql/functions/datefromparts-transact-sql?view=sql-server-ver17

- **EDIT_DISTANCE_SIMILARITY (Transact-SQL) preview**

  Raised the minimum on-premises version to SQL Server 2017 while keeping Azure and Fabric targets. No functional description changes.

  https://learn.microsoft.com/en-us/sql/t-sql/functions/edit-distance-similarity-transact-sql?view=sql-server-ver17

- **Exception Event Class**

  Set applicability to SQL Server 2017 and later, retaining Azure SQL targets. Event class guidance is unchanged.

  https://learn.microsoft.com/en-us/sql/relational-databases/event-classes/exception-event-class?view=sql-server-ver17

- **Executing Template Files by Using the CommandStream Property**

  Updated monikers to require SQL Server 2017 and later. The how-to content is unchanged.

  https://learn.microsoft.com/en-us/sql/relational-databases/sqlxml-annotated-xsd-schemas-xpath-queries/net-framework-classes/executing-template-files-by-using-the-commandstream-property?view=sql-server-ver17

- **Executing XPath Queries (SQLXML Managed Classes)**

  Raised the minimum supported version to SQL Server 2017, retaining Azure targets. Query execution guidance is unchanged.

  https://learn.microsoft.com/en-us/sql/relational-databases/sqlxml-annotated-xsd-schemas-xpath-queries/net-framework-classes/executing-xpath-queries-sqlxml-managed-classes?view=sql-server-ver17

- **Execution Related Dynamic Management Views and Functions (Transact-SQL)**

  Adjusted version applicability to SQL Server 2017 and later across page-level and scoped directives. DMV coverage and usage remain the same.

  https://learn.microsoft.com/en-us/sql/relational-databases/system-dynamic-management-objects/execution-related-dynamic-management-views-and-functions-transact-sql?view=sql-server-ver17

- **GENERATE_SERIES (Transact-SQL)**

  Updated support to start at SQL Server 2017 and aligned moniker directives across sections. Function details and examples were not changed.

  https://learn.microsoft.com/en-us/sql/t-sql/functions/generate-series-transact-sql?view=sql-server-ver17

- **SQL Server installation guide**

  Replaced the combined 2016/2017 requirements entry with a 2017-specific reference, effectively dropping SQL Server 2016 from that list. Installation guidance remains current for supported versions.

  https://learn.microsoft.com/en-us/sql/database-engine/install-windows/install-sql-server?view=sql-server-ver17

- **LEAD (Transact-SQL)**

  Raised the minimum supported version to SQL Server 2017. Function syntax and examples are unchanged.

  https://learn.microsoft.com/en-us/sql/t-sql/functions/lead-transact-sql?view=sql-server-ver17

- **Manage trigger security**

  Updated an in-page moniker block to require SQL Server 2017 and later. Security guidance applicability now aligns with supported versions.

  https://learn.microsoft.com/en-us/sql/relational-databases/triggers/manage-trigger-security?view=sql-server-ver17

- **Modify R/Python code to run in SQL Server (In-Database) instances**

  Updated all relevant moniker directives to SQL Server 2017 and later, aligning guidance with supported versions and platforms. The underlying performance and security recommendations are unchanged.

  https://learn.microsoft.com/en-us/sql/machine-learning/deploy/modify-r-python-code-to-run-in-sql-server?view=sql-server-ver17

- **Monitor Performance with Replication Monitor**

  Adjusted applicability to SQL Server 2017 and later while retaining Azure SQL MI coverage. Monitoring steps and concepts are unchanged.

  https://learn.microsoft.com/en-us/sql/relational-databases/replication/monitor/monitor-performance-with-replication-monitor?view=sql-server-ver17

- **MSSQL_REPL-2147200953**

  Raised the minimum supported version to SQL Server 2017 and normalized moniker formatting. Error reference content is unchanged.

  https://learn.microsoft.com/en-us/sql/relational-databases/replication/mssql-repl-2147200953?view=sql-server-ver17

- **OPENROWSET BULK (Transact-SQL)**

  Updated all moniker ranges to start at SQL Server 2017, aligning syntax, notes, and examples with supported versions. No changes to semantics or examples.

  https://learn.microsoft.com/en-us/sql/t-sql/functions/openrowset-bulk-transact-sql?view=sql-server-ver17

- **Point**

  Updated applicability to SQL Server 2017 and later. Spatial type content is unchanged.

  https://learn.microsoft.com/en-us/sql/relational-databases/spatial/point?view=sql-server-ver17

- **Install PolyBase on Windows**

  Retargeted PolyBase installation guidance to SQL Server 2017 only, removing 2016. Clarifies supported version scope for setup.

  https://learn.microsoft.com/en-us/sql/relational-databases/polybase/polybase-installation?view=sql-server-ver17

- **Reduce the Production Server Tuning Load**

  Raised the minimum supported version to SQL Server 2017 while maintaining Azure SQL targets. Optimization guidance is unchanged.

  https://learn.microsoft.com/en-us/sql/relational-databases/performance/reduce-the-production-server-tuning-load?view=sql-server-ver17

- **R tutorials for SQL machine learning**

  Updated moniker ranges to require SQL Server 2017 and later at both page and section level. Tutorial descriptions and steps are unchanged.

  https://learn.microsoft.com/en-us/sql/machine-learning/tutorials/r-tutorials?view=sql-server-ver17

- **Security Audit Event Category (SQL Server Profiler)**

  Raised applicability to SQL Server 2017 and later, with minor formatting normalization. No changes to profiler event details.

  https://learn.microsoft.com/en-us/sql/relational-databases/event-classes/security-audit-event-category-sql-server-profiler?view=sql-server-ver17

- **Specify Synchronization Schedules**

  Updated support to SQL Server 2017 and later, retaining Azure SQL MI applicability. Replication scheduling guidance is unchanged.

  https://learn.microsoft.com/en-us/sql/relational-databases/replication/specify-synchronization-schedules?view=sql-server-ver17

- **Statistics for Memory-Optimized Tables**

  Set the minimum supported version to SQL Server 2017, keeping Azure SQL targets. The statistical guidance remains the same.

  https://learn.microsoft.com/en-us/sql/relational-databases/in-memory-oltp/statistics-for-memory-optimized-tables?view=sql-server-ver17

- **Subscriber Properties**

  Adjusted applicability to SQL Server 2017 and later. Property details and usage are unchanged.

  https://learn.microsoft.com/en-us/sql/relational-databases/replication/subscriber-properties?view=sql-server-ver17

- **Subscribers**

  Updated support to begin at SQL Server 2017 and retained Azure SQL coverage. Replication subscriber guidance is unchanged.

  https://learn.microsoft.com/en-us/sql/relational-databases/replication/subscribers?view=sql-server-ver17

- **Subscription Expiration and Deactivation**

  Raised the minimum version to SQL Server 2017 and kept Azure SQL MI applicability. Conceptual guidance is unchanged.

  https://learn.microsoft.com/en-us/sql/relational-databases/replication/subscription-expiration-and-deactivation?view=sql-server-ver17

- **sys.all_sql_modules (Transact-SQL)**

  Updated monikers to start at SQL Server 2017. DMV description and usage remain unchanged.

  https://learn.microsoft.com/en-us/sql/relational-databases/system-catalog-views/sys-all-sql-modules-transact-sql?view=sql-server-ver17

- **sys.assembly_modules (Transact-SQL)**

  Adjusted applicability to SQL Server 2017 and later. No changes to content.

  https://learn.microsoft.com/en-us/sql/relational-databases/system-catalog-views/sys-assembly-modules-transact-sql?view=sql-server-ver17

- **sys.column_encryption_key_values (Transact-SQL)**

  Raised the minimum supported version to SQL Server 2017 and normalized formatting. The encryption key metadata guidance is unchanged.

  https://learn.microsoft.com/en-us/sql/relational-databases/system-catalog-views/sys-column-encryption-key-values-transact-sql?view=sql-server-ver17

- **sys.cryptographic_providers (Transact-SQL)**

  Updated applicability to SQL Server 2017 and later while retaining Azure targets. Content remains unchanged.

  https://learn.microsoft.com/en-us/sql/relational-databases/system-catalog-views/sys-cryptographic-providers-transact-sql?view=sql-server-ver17

- **sys.dm_db_task_space_usage (Transact-SQL)**

  Set the minimum supported version to SQL Server 2017. DMV behavior and examples are unchanged.

  https://learn.microsoft.com/en-us/sql/relational-databases/system-dynamic-management-objects/sys-dm-db-task-space-usage-transact-sql?view=sql-server-ver17

- **sys.dm_os_process_memory (Transact-SQL)**

  Raised applicability to SQL Server 2017 and later with minor formatting updates. Reference details are unchanged.

  https://learn.microsoft.com/en-us/sql/relational-databases/system-dynamic-management-objects/sys-dm-os-process-memory-transact-sql?view=sql-server-ver17

- **sys.dm_os_ring_buffers (Transact-SQL)**

  Updated support to start at SQL Server 2017, retaining Azure targets. DMV usage guidance is unchanged.

  https://learn.microsoft.com/en-us/sql/relational-databases/system-dynamic-management-objects/sys-dm-os-ring-buffers-transact-sql?view=sql-server-ver17

- **sys.dm_tran_active_transactions (Transact-SQL)**

  Set applicability to SQL Server 2017 and later. Reference content is unchanged.

  https://learn.microsoft.com/en-us/sql/relational-databases/system-dynamic-management-objects/sys-dm-tran-active-transactions-transact-sql?view=sql-server-ver17

- **sys.dm_tran_version_store_space_usage (Transact-SQL)**

  Raised the minimum supported version to SQL Server 2017. No changes to DMV details.

  https://learn.microsoft.com/en-us/sql/relational-databases/system-dynamic-management-objects/sys-dm-tran-version-store-space-usage?view=sql-server-ver17

- **sys.dm_tran_version_store (Transact-SQL)**

  Updated applicability to SQL Server 2017 and later. Content remains unchanged.

  https://learn.microsoft.com/en-us/sql/relational-databases/system-dynamic-management-objects/sys-dm-tran-version-store-transact-sql?view=sql-server-ver17

- **sys.fn_helpcollations (Transact-SQL)**

  Set support to start at SQL Server 2017. Function reference and outputs are unchanged.

  https://learn.microsoft.com/en-us/sql/relational-databases/system-functions/sys-fn-helpcollations-transact-sql?view=sql-server-ver17

- **System-versioned temporal tables with memory-optimized tables**

  Raised the minimum version to SQL Server 2017 for applicability. Guidance and examples are unchanged.

  https://learn.microsoft.com/en-us/sql/relational-databases/tables/system-versioned-temporal-tables-with-memory-optimized-tables?view=sql-server-ver17

- **Tips for using R packages**

  Updated moniker ranges to require SQL Server 2017 and later across the page and scoped blocks. Best practices content remains the same.

  https://learn.microsoft.com/en-us/sql/machine-learning/package-management/tips-for-using-r-packages?view=sql-server-ver17

- **TSQL Event Category**

  Set applicability to SQL Server 2017 and later. Event category descriptions are unchanged.

  https://learn.microsoft.com/en-us/sql/relational-databases/event-classes/tsql-event-category?view=sql-server-ver17

- **Unsupported SQL Server Features for In-Memory OLTP**

  Raised the minimum on-premises version to SQL Server 2017 while retaining Azure targets. The unsupported feature list is unchanged.

  https://learn.microsoft.com/en-us/sql/relational-databases/in-memory-oltp/unsupported-sql-server-features-for-in-memory-oltp?view=sql-server-ver17

- **Use Unicode Native Format to Import or Export Data (SQL Server)**

  Updated applicability to SQL Server 2017 and later. Import/export steps and examples are unchanged.

  https://learn.microsoft.com/en-us/sql/relational-databases/import-export/use-unicode-native-format-to-import-or-export-data-sql-server?view=sql-server-ver17

- **Web application requirements (Master Data Services)**

  Refreshed prerequisites to list SQL Server 2022 and 2019 explicitly and separated SQL Server 2017 into its own item. This clarifies current support and removes the prior combined 2016/2017 reference.

  https://learn.microsoft.com/en-us/sql/master-data-services/install-windows/web-application-requirements-master-data-services?view=sql-server-ver16

- **What's new in SQL Server Machine Learning Services?**

  Updated version applicability to require SQL Server 2017 and later across page-level and in-page moniker blocks. No changes to feature descriptions.

  https://learn.microsoft.com/en-us/sql/machine-learning/what-s-new-in-sql-server-machine-learning-services?view=sql-server-ver17

## Minor Changes