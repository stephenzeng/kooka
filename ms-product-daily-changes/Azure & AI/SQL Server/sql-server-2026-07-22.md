# SQL Server
**Date created:** 2026-07-22 UTC  
**Tags:** Administration, Analytics, Other, Programming, Security  

## New Articles

- **Use mssql-python with Apache Arrow**

  Introduced Arrow-based fetch methods (arrow, arrow_batch, arrow_reader) to retrieve columnar data efficiently from SQL Server into Python. Added end-to-end examples for integrating with pandas, Polars, and DuckDB, streaming large results to Parquet/CSV/IPC, and tuning memory and batch sizes. Documented SQL-to-Arrow type mappings and notes like datetimeoffset UTC normalization and unsupported sql_variant.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/arrow-integration?view=sql-server-ver17

- **Async Patterns with mssql-python**

  Provided practical async patterns using ThreadPoolExecutor and asyncio to wrap the synchronous driver. Included templates for connection pooling wrappers, FastAPI integration, background tasks, and concurrent query execution. Covered streaming pagination, executor sizing, graceful shutdown, and resilient retry guidance.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/asynchronous-patterns?view=sql-server-ver17

- **Use Read-Only Routing and Availability Groups with mssql-python**

  Added guidance for connecting via an availability group listener with ApplicationIntent and MultiSubnetFailover for fast failovers. Showed patterns for separate read/write connections, read-after-write with replication lag, and retry logic on role changes. Included code examples to validate routing and offload read workloads.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/availability-groups?view=sql-server-ver17

- **Work with Binary Data Using mssql-python**

  Explained how to insert, retrieve, and stream large binary data, including files and images, with best practices for types and FILESTREAM. Demonstrated bulk loading, hashing/validation, and format-specific operations (e.g., PDF checks, Pillow image handling, gzip). Provided patterns for exporting rows to disk and safe NULL handling.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/binary-data?view=sql-server-ver17

- **Build Connection Strings Programmatically with mssql-python**

  Presented multiple approaches to compose secure, flexible connection strings (builder pattern, environment files, JSON/YAML configs, Key Vault). Covered Entra authentication, encryption settings, and escaping rules for special characters. Included a helper for validating strings by running a lightweight query.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/build-connection-strings?view=sql-server-ver17

- **Use Bulk Copy with mssql-python Driver**

  Introduced cursor.bulkcopy for high-throughput data loads with options for batching, identity handling, constraints, and transactions. Showed mappings by name/index, generators for CSV ingestion, and DataFrame to table loading. Covered auth paths (Managed Identity, Service Principal) for the bulk channel and performance tips versus executemany.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/bulk-copy?view=sql-server-ver17

- **Manage Connections with mssql-python**

  Detailed connection lifecycle patterns, including context managers, autocommit configuration, and runtime attribute changes (timeouts, isolation, packet size). Explained retrieving driver/server metadata and safe LIKE escaping. Provided best practices for pooling, timeouts, and thread safety.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/connection-management?view=sql-server-ver17

- **Connection Pooling with mssql-python**

  Described default pooling behavior, configuration/disable options, and lifecycle (acquire/release, health checks). Shared guidance for pool sizing, avoiding exhaustion, and app patterns (Flask/ASGI). Listed current limitations and tuning tips for cloud limits and idle cleanup.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/connection-pooling?view=sql-server-ver17

- **Connection Strings for mssql-python**

  Provided a comprehensive keyword reference with examples for SQL and Entra auth, encryption/TLS (including strict/TDS 8.0), and HA/failover. Clarified keyword vs parameter overrides and escaping rules. Included timeout/autocommit, ODBC attribute injection, and parser error handling.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/connection-strings?view=sql-server-ver17

- **Container and Local Development with mssql-python**

  Offered step-by-step setup for local SQL (go-sqlcmd, VS Code, Docker) and Python environments with needed system libraries. Showed Dockerfile/devcontainer patterns, CI orchestration, and secrets management. Included Azure SQL auth options and troubleshooting for platform dependencies.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/container-local-development?view=sql-server-ver17

- **Manage Cursors and Result Sets in mssql-python**

  Explained cursor creation, reuse, and concurrency without MARS using multiple connections. Covered fetch strategies, handling multiple result sets, and memory-efficient processing via batching. Included metadata access, rowcount behavior, and practical lifecycle best practices.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/cursor-management?view=sql-server-ver17

- **Custom Type Converters with mssql-python**

  Documented registering/removing custom output converters and expected function signatures based on cursor.description. Provided examples for money/decimal, JSON parsing, datetime formatting, and spatial integration. Included security and performance considerations and converter scoping.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/custom-type-converters?view=sql-server-ver17

- **Choose a Data Access and Analytics Pattern with mssql-python**

  Compared cursor fetch methods, Arrow extraction, and DataFrame integrations (pandas/Polars/DuckDB) with code examples. Offered guidance for streaming large results and pushing computation server-side. Linked SQL features (columnstore, IQP, Query Store) to pattern choices and pitfalls.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/data-access-analytics-patterns?view=sql-server-ver17

- **Choose a Data Loading and Movement Pattern with mssql-python**

  Outlined patterns from single inserts and executemany batching to high-throughput bulkcopy. Provided MERGE upsert designs, staging table workflows, and DataFrame/Parquet loading paths. Clarified validation/transaction considerations, including bulkcopy’s transaction behavior.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/data-loading-movement-patterns?view=sql-server-ver17

- **Data Type Mappings for mssql-python**

  Mapped Python↔SQL types, MAX type handling, and streaming for large values. Covered setinputsizes overrides, decimal locale, UUID/native_uuid, datetimeoffset, spatial as WKT/bytes, and unsupported types. Provided precision and NumPy/pandas conversion recommendations.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/data-type-mappings?view=sql-server-ver17

- **Work with Datetime Values in mssql-python**

  Showed reliable handling of SQL date/time types, including timezone-aware values and conversions. Demonstrated date arithmetic, parsing/formatting, range queries, and audit patterns. Included special scenarios (pre-1753 dates, business days) with Python and SQL examples.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/datetime-handling?view=sql-server-ver17

- **Handle Decimal and Money Values in mssql-python**

  Established Decimal as the standard for precise financial calculations and described rounding/formatting. Provided patterns for totals, averages, currency conversion, and transactional balance updates. Included output converters, bulk insert tips, and best-practice checklists.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/decimal-money?view=sql-server-ver17

- **Use mssql-python with DuckDB**

  Demonstrated querying SQL Server results via Arrow directly in DuckDB for analytics. Covered joins with local files, exporting to Parquet/CSV, and streaming large results with arrow_reader. Emphasized server-side filtering and Arrow for efficient data transfer.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/duck-db-integration?view=sql-server-ver17

- **Encryption and TLS with mssql-python**

  Explained Encrypt options (including strict/TDS 8.0), TrustServerCertificate risks, and certificate hostname validation. Provided recommended configurations for Azure SQL, on-prem production, and dev scenarios. Included troubleshooting for common TLS errors.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/encryption-certificates?view=sql-server-ver17

- **Microsoft Entra Authentication with mssql-python**

  Detailed authentication modes (Default, Interactive, DeviceCode, MSI, Service Principal, Integrated) with connection examples. Clarified token acquisition, DefaultAzureCredential behavior, and SQL access token injection. Offered scenario guidance and troubleshooting for common identity issues.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/entra-authentication?view=sql-server-ver17

- **Error Handling and SQLSTATE Codes for mssql-python**

  Documented DB-API exception classes, SQLSTATE-driven categorization, and exception attributes. Provided mappings for common errors, retry guidance for transient faults, and logging/rollback best practices. Included symptom-to-exception references for rapid diagnosis.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/error-handling?view=sql-server-ver17

- **Execute Queries with mssql-python**

  Covered parameterized execution styles, DML with transactions, and batch execution methods. Explained prepared statement behavior, stored procedure calling via EXECUTE/{CALL}, and explicit typing with setinputsizes (including known decimal caveat). Included structured error handling and performance guidance.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/executing-queries?view=sql-server-ver17

- **Use mssql-python with FastAPI**

  Provided an end-to-end FastAPI app with parameterized CRUD endpoints, pagination, and health checks. Demonstrated dependency-managed connections, pooling, and centralized error handling. Included JWT auth middleware, testing patterns, and configuration via environment variables.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/fast-api-integration?view=sql-server-ver17

- **Use mssql-python with Flask**

  Showed request-scoped connection/cursor management and blueprint-based route organization. Delivered CRUD and health endpoints with parameterized queries and pooling. Included pytest-based testing, Entra auth options, and performance considerations.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/flask-integration?view=sql-server-ver17

- **Install mssql-python**

  Provided cross-platform install steps (pip, pinning, verification) with system dependencies for Linux/macOS. Explained virtual environment usage, developer installs, and resolving common install/import issues. Linked to quickstarts and reference articles.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/installation?view=sql-server-ver17

- **Use JSON Data with mssql-python**

  Explained storing, validating, querying, and modifying JSON with SQL functions. Showed indexing patterns via computed columns and when to process JSON server-side vs client-side. Included Python repository patterns and handling large FOR JSON outputs.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/json-data?view=sql-server-ver17

- **Migrate from PostgreSQL to Microsoft SQL with mssql-python**

  Mapped key SQL and driver differences (types, pagination, upserts, RETURNING vs OUTPUT, auth). Provided code rewrites, transaction guidance, and bulk loading strategies. Included a schema/data migration script with dependency ordering and revalidation.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/migrate-from-postgresql?view=sql-server-ver17

- **Migrate from pymssql to mssql-python**

  Outlined driver and API differences, including parameter styles, pooling, and multi-cursor support. Demonstrated stored procedure approaches without callproc and bulk copy migration. Included before/after code examples and a migration checklist.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/migrate-from-pymssql?view=sql-server-ver17

- **Migrate from pyodbc to mssql-python**

  Described moving off external ODBC dependencies to the first-party driver with qmark/pyformat support. Covered connection string updates, stored procedure execution, and equivalent exceptions. Provided performance guidance and full before/after examples.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/migrate-from-pyodbc?view=sql-server-ver17

- **Migrate from SQLite to Microsoft SQL with mssql-python**

  Compared SQL features and data types and provided translation examples for schema, pagination, and upserts. Included code for returning inserted IDs and a bulk migration script. Offered guidance for sizing text/LOBs and mapping types safely.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/migrate-from-sql-lite?view=sql-server-ver17

- **Configure mssql-python Module Settings**

  Documented global Settings (column name casing, decimal separator) and connection-level overrides. Explained native_uuid behavior for UNIQUEIDENTIFIER, DB-API constants, and version checks. Recommended configuring settings at startup for consistency.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/module-configuration?view=sql-server-ver17

- **Handle NULL Values with mssql-python**

  Clarified mapping of SQL NULL to Python None and correct checks and SQL predicates. Showed NULL-safe patterns for CRUD, aggregations, and serialization (JSON/dataclasses). Covered bulk operations, DataFrame handling, and practical examples.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/null-handling?view=sql-server-ver17

- **Implement Pagination with mssql-python**

  Presented OFFSET-FETCH, keyset/seek, cursor-based, and ROW_NUMBER strategies with validation for sorting and filters. Included a reusable PagedResult helper and generator-based iteration. Provided indexing and performance tips to avoid deep OFFSET penalties.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/pagination?view=sql-server-ver17

- **Use mssql-python with pandas**

  Demonstrated reading with Arrow and chunking, and writing via parameterized inserts and bulkcopy. Showed analytics patterns (resampling, pivots) and ETL workflows with incremental loads. Included performance tips to push computation server-side.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/pandas-integration?view=sql-server-ver17

- **Build Parameterized Queries with mssql-python**

  Provided secure patterns for parameters across types, dynamic IN lists, and validated sorting/columns. Included CRUD examples with executemany batching and OUTPUT for identity keys. Emphasized plan reuse, preparation, and injection prevention.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/parameterized-queries?view=sql-server-ver17

- **Performance Tuning for mssql-python Applications**

  Covered pooling strategies, fetch and insertion patterns (execute, executemany, bulkcopy), and network round-trip reduction. Included memory management, query/index tuning, and monitoring with Python/SQL tools. Concluded with a performance checklist.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/performance-tuning?view=sql-server-ver17

- **Use mssql-python with Polars**

  Recommended Arrow for fast reads into Polars and demonstrated batch streaming. Showed bulkcopy for efficient writes and safe quoting for generated SQL. Included ETL and analysis patterns with performance best practices.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/polars-integration?view=sql-server-ver17

- **Quickstart: Apache Arrow with the mssql-python Driver**

  Provided a ready-to-run project that fetches SQL data via Arrow full-table, batch, and reader patterns. Demonstrated saving to Parquet and rendering results. Included environment setup with uv, .env configuration, and Azure CLI auth notes.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/python-sql-driver-mssql-python-arrow-quickstart?view=sql-server-ver17

- **Retrieve Data with mssql-python**

  Explained fetch methods, row access patterns, and metadata usage. Covered navigation, batching, multiple result sets, and large-result strategies. Shared best practices for cleanup and efficient iteration.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/retrieving-data?view=sql-server-ver17

- **Retry Logic and Connection Resiliency with mssql-python**

  Identified transient errors using SQLSTATE and engine codes, with guidance on what to retry. Included decorators, a ResilientConnection wrapper, and policies for backoff, deadlocks, and throttling. Offered circuit breaker examples and troubleshooting tips.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/retry-logic?view=sql-server-ver17

- **Row Objects in mssql-python**

  Clarified row access by attribute, string key, and index, plus tuples, dict conversion, and slicing. Showed metadata-driven transformations and dataclass mapping. Included JSON serialization patterns and naming/casing considerations.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/row-objects?view=sql-server-ver17

- **Schema Discovery with mssql-python**

  Documented nine metadata methods for tables, columns, procedures, keys, indexes, and data types. Provided filters and end-to-end examples to build schema reports. Included security notes for exposing metadata.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/schema-discovery?view=sql-server-ver17

- **Security Best Practices for mssql-python Applications**

  Recommended Entra/managed identities, secret hygiene, and enforced encryption/certificate validation. Showed parameterized queries, identifier validation, and least privilege role patterns. Added auditing, safe error handling, and a comprehensive checklist.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/security-best-practices?view=sql-server-ver17

- **Use Sparse Columns and Column Sets with mssql-python**

  Explained sparse column benefits and column set XML techniques for flexible attributes. Provided insert/update/query patterns, dynamic attribute validation, and bulkcopy strategies. Included storage/Index guidance and monitoring NULL sparsity.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/sparse-columns?view=sql-server-ver17

- **Use Spatial Data with mssql-python**

  Demonstrated inserting/querying geometry/geography, spatial operations, and distance/area calculations. Integrated Shapely/GeoPandas for WKT/GeoJSON workflows and indexing for performance. Covered CRS/SRID handling, validation, and MakeValid.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/spatial-data?view=sql-server-ver17

- **Use mssql-python with SQLAlchemy**

  Introduced the mssql-python SQLAlchemy dialect with connection URLs for SQL/Entra auth. Provided ORM/Core examples, pooling settings, and web app integration patterns. Included Alembic migration setup, differences vs pyodbc, and troubleshooting.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/sql-alchemy-integration?view=sql-server-ver17

- **Call Stored Procedures with mssql-python**

  Showed executing procedures via EXECUTE and ODBC {CALL}, capturing output parameters and return codes. Covered handling multiple result sets and transaction patterns. Included best practices and alternatives for unsupported features.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/stored-procedures?view=sql-server-ver17

- **Handle Strings and Unicode with mssql-python**

  Explained string type choices, Unicode handling, and encoding behavior across nvarchar/varchar. Provided safe LIKE escaping, collation effects, and large text handling. Included JSON-in-nvarchar patterns and truncation-avoidance tips.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/string-unicode?view=sql-server-ver17

- **Support Lifecycle for mssql-python Driver**

  Documented supported Python/OS/SQL platforms, feature matrix, and limitations. Provided version history, upgrade policy, and compatibility notes. Included migration guidance from other drivers and support channels.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/support-lifecycle?view=sql-server-ver17

- **Transaction Management with mssql-python**

  Clarified autocommit vs explicit transactions, isolation levels, and savepoints. Provided deadlock retry patterns and lock hints to prevent lost updates. Included temp table scope considerations and DDL requirements.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/transaction-management?view=sql-server-ver17

- **Troubleshoot mssql-python**

  Centralized fixes for install, connection, query, datatype, performance, transaction, and bulk copy issues. Provided environment checks, logging, and diagnostics, plus platform-specific remedies. Included quick reference error mapping and related links.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/troubleshooting?view=sql-server-ver17

- **What's New in mssql-python Driver**

  Added release notes from 1.0.0 to 1.11.0 highlighting bulkcopy, Arrow, sql_variant, native UUID, and pooling enhancements. Summarized bug fixes and performance improvements across versions. Included upgrade guidance and roadmap links.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/whats-new?view=sql-server-ver17

- **Use XML Data with mssql-python**

  Covered inserting/validating XML, querying with XQuery methods, and modifying documents in-place. Demonstrated shredding via nodes(), XML indexing for performance, and namespace handling. Included Python parsing, streaming, and best practices for choosing XML vs JSON.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/xml-data?view=sql-server-ver17

## Major Changes

- **Full-Text Search**

  Updated applicability to SQL Server 2017+ and refined component behavior and process descriptions for clarity. Corrected supported data types for full-text indexes (limiting binary support to varbinary(max), image, and xml and requiring a type column) and clarified indexing behaviors. Expanded details on indexing pipelines and storage paths to improve accuracy and troubleshooting.

  https://learn.microsoft.com/en-us/sql/relational-databases/search/full-text-search?view=sql-server-ver17

- **Microsoft Python Driver for SQL Server - mssql-python**

  Overhauled the page into an overview and task hub with comprehensive samples and best practices for production. Added sections covering connection/authentication, resiliency, data access patterns, bulk copy, data types, integrations, and migration guidance from other drivers. Emphasized secure defaults (encryption, Entra auth), robust error handling, and performance-focused patterns across the driver’s feature set.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/python-sql-driver-mssql-python?view=sql-server-ver17

- **Quickstart: Python SQL Driver - mssql-python Bulk Copy with the Python Driver**

  Revamped the bulk copy quickstart to use Arrow streaming for faster, lower-overhead data movement and improved type fidelity. Simplified setup, updated dependency requirements, and strengthened validation by verifying destination row counts. Added clear next steps for advanced performance tuning and data movement scenarios.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/python-sql-driver-mssql-python-bulk-copy-quickstart?view=sql-server-ver17

- **Query with Full-Text Search**

  Expanded examples and reorganized guidance to clarify when to use predicates versus rowset-valued functions. Added targeted scenarios (prefix, inflectional, thesaurus synonyms, NEAR, ISABOUT/WEIGHT) with ranking and filtering patterns. Strengthened cross-references to setup, analysis tools, and related search features for quicker adoption.

  https://learn.microsoft.com/en-us/sql/relational-databases/search/query-with-full-text-search?view=sql-server-ver17

## Moderate Changes

- **ALTER ASYMMETRIC KEY (Transact-SQL)**

  Updated applicability to require SQL Server 2017 or later, removing SQL Server 2016 from scope. This clarifies supported versions without changing syntax or behavior.

  https://learn.microsoft.com/en-us/sql/t-sql/statements/alter-asymmetric-key-transact-sql?view=sql-server-ver17

- **ALTER CREDENTIAL (Transact-SQL)**

  Adjusted version applicability to SQL Server 2017+, aligning front matter and in-page monikers. This narrows supported on-prem targets while retaining Azure offerings.

  https://learn.microsoft.com/en-us/sql/t-sql/statements/alter-credential-transact-sql?view=sql-server-ver17

- **ALTER DATABASE SCOPED CONFIGURATION (Transact-SQL)**

  Raised the minimum supported version to SQL Server 2017 to match current support. No operational guidance changed; only applicability was updated.

  https://learn.microsoft.com/en-us/sql/t-sql/statements/alter-database-scoped-configuration-transact-sql?view=sql-server-ver17

- **ALTER DATABASE (Transact-SQL)**

  Updated version scope to SQL Server 2017 and later, removing 2016 from applicability. The change helps readers target current platforms without altering procedures.

  https://learn.microsoft.com/en-us/sql/t-sql/statements/alter-database-transact-sql?view=sql-server-ver17

- **ALTER DATABASE (Transact-SQL) File and Filegroup Options**

  Revised monikers to start at SQL Server 2017 across page-level and content blocks. This ensures version accuracy for file and filegroup configuration topics.

  https://learn.microsoft.com/en-us/sql/t-sql/statements/alter-database-transact-sql-file-and-filegroup-options?view=sql-server-ver17

- **ALTER DATABASE SET options (Transact-SQL)**

  Limited a content block’s applicability to SQL Server 2017+, removing 2016 from that section. The update avoids confusion about supported behaviors on older versions.

  https://learn.microsoft.com/en-us/sql/t-sql/statements/alter-database-transact-sql-set-options?view=sql-server-ver17

- **ALTER LOGIN (Transact-SQL)**

  Updated monikers to require SQL Server 2017+, aligning the page metadata and in-page directive. This change clarifies supported environments for login management.

  https://learn.microsoft.com/en-us/sql/t-sql/statements/alter-login-transact-sql?view=sql-server-ver17

- **ALTER TABLE (Transact-SQL)**

  Raised applicability to SQL Server 2017+, updating top-level metadata and in-article moniker blocks. The article now targets current releases without altering syntax guidance.

  https://learn.microsoft.com/en-us/sql/t-sql/statements/alter-table-transact-sql?view=sql-server-ver17

- **ALTER USER (Transact-SQL)**

  Updated version monikers to start at SQL Server 2017 for on-prem environments. No syntax or procedural changes were made.

  https://learn.microsoft.com/en-us/sql/t-sql/statements/alter-user-transact-sql?view=sql-server-ver17

- **ALTER WORKLOAD GROUP (Transact-SQL)**

  Adjusted applicability to SQL Server 2017+ (Windows/Linux) at both metadata and directive levels. This ensures guidance maps to supported versions.

  https://learn.microsoft.com/en-us/sql/t-sql/statements/alter-workload-group-transact-sql?view=sql-server-ver17

- **BACKUP (Transact-SQL)**

  Set minimum supported on-prem version to SQL Server 2017, aligning moniker directives. This clarifies version eligibility without changing backup syntax.

  https://learn.microsoft.com/en-us/sql/t-sql/statements/backup-transact-sql?view=sql-server-ver17

- **BULK INSERT (Transact-SQL)**

  Updated monikers to 2017+ and clarified applicability across syntax and options sections. No functional changes; the revision narrows version scope across platforms.

  https://learn.microsoft.com/en-us/sql/t-sql/statements/bulk-insert-transact-sql?view=sql-server-ver17

- **Choose a Language When Creating a Full-Text Index**

  Broadened applies-to to include Azure SQL Managed Instance and clarified security guidance for verifying signed external components. Refined language behavior explanations to help administrators configure safe, predictable full-text processing.

  https://learn.microsoft.com/en-us/sql/relational-databases/search/choose-a-language-when-creating-a-full-text-index?view=sql-server-ver17

- **CLOSE SYMMETRIC KEY (Transact-SQL)**

  Narrowed on-premises applicability to SQL Server 2017 or later. This avoids implying support for 2016 without altering usage guidance.

  https://learn.microsoft.com/en-us/sql/t-sql/statements/close-symmetric-key-transact-sql?view=sql-server-ver17

- **Configure and Manage Stopwords and Stoplists for Full-Text Search**

  Reorganized and expanded content with clearer definitions, step-by-step procedures in T-SQL/SSMS, and concise task-method tables. Clarified behaviors (e.g., positional handling) and upgrade guidance, improving operational accuracy and troubleshooting.

  https://learn.microsoft.com/en-us/sql/relational-databases/search/configure-and-manage-stopwords-and-stoplists-for-full-text-search?view=sql-server-ver17

- **Configure and Manage Word Breakers and Stemmers**

  Updated version applicability to SQL Server 2017+ while retaining Azure services. Editorial refinements improve clarity without changing procedures.

  https://learn.microsoft.com/en-us/sql/relational-databases/search/configure-and-manage-word-breakers-and-stemmers-for-search?view=sql-server-ver17

- **Create and Manage Full-Text Indexes**

  Expanded conceptual explanations, refined procedures, and updated examples for modern samples. Removed SQL Server 2016 from supported monikers, aligning the article with current releases and Azure.

  https://learn.microsoft.com/en-us/sql/relational-databases/search/create-and-manage-full-text-indexes?view=sql-server-ver17

- **CREATE DATABASE**

  Updated in-page monikers to start at SQL Server 2017 for Windows and Linux. The change aligns version labeling without altering syntax.

  https://learn.microsoft.com/en-us/sql/t-sql/statements/create-database-transact-sql?view=sql-server-ver17

- **CREATE EXTERNAL DATA SOURCE (Transact-SQL)**

  Raised minimum version support to SQL Server 2017 across metadata and directives. This ensures readers target currently supported platforms.

  https://learn.microsoft.com/en-us/sql/t-sql/statements/create-external-data-source-transact-sql?view=sql-server-ver17

- **CREATE EXTERNAL TABLE (Transact-SQL)**

  Updated monikers to SQL Server 2017+, adjusting applicability for all sections. No functional changes, only version alignment.

  https://learn.microsoft.com/en-us/sql/t-sql/statements/create-external-table-transact-sql?view=sql-server-ver17

- **CREATE LOGIN (Transact-SQL)**

  Set minimum version to SQL Server 2017 and normalized directive formatting. Applies to on-prem Windows/Linux with no semantic changes.

  https://learn.microsoft.com/en-us/sql/t-sql/statements/create-login-transact-sql?view=sql-server-ver17

- **CREATE TABLE (Transact-SQL) IDENTITY (Property)**

  Limited on-prem applicability to SQL Server 2017+ across syntax and example sections. This clarifies supported environments without changing identity semantics.

  https://learn.microsoft.com/en-us/sql/t-sql/statements/create-table-transact-sql-identity-property?view=sql-server-ver17

- **CREATE WORKLOAD GROUP (Transact-SQL)**

  Updated version scope to SQL Server 2017+, aligning monikers in metadata and body. No other content changes.

  https://learn.microsoft.com/en-us/sql/t-sql/statements/create-workload-group-transact-sql?view=sql-server-ver17

- **Customize behavior of word breakers with a dictionary file**

  Narrowed scope to SQL Server 2017+ (Windows/Linux), removing Azure and 2016 applicability. Cleaned formatting and clarified operational steps for dictionary placement and service restart.

  https://learn.microsoft.com/en-us/sql/relational-databases/search/customize-the-behavior-of-word-breakers-with-a-custom-dictionary?view=sql-server-ver17

- **Driver Feature Support Matrix**

  Refreshed Python driver capabilities, adding Bulk Copy support (v1.4.0+) and clarifying MultiSubnetFailover and Transparent Network IP Resolution. This helps developers select features based on accurate, current support.

  https://learn.microsoft.com/en-us/sql/connect/driver-feature-matrix?view=sql-server-ver17

- **DROP WORKLOAD GROUP (Transact-SQL)**

  Adjusted monikers to SQL Server 2017+ (including Linux) with directive alignment. This update reflects current support without behavior changes.

  https://learn.microsoft.com/en-us/sql/t-sql/statements/drop-workload-group-transact-sql?view=sql-server-ver17

- **Find property set GUIDs and property integer IDs for search properties**

  Expanded applicability to Azure SQL Managed Instance and updated version scope to SQL Server 2017+. Clarified supported types and reorganized sections for easier navigation.

  https://learn.microsoft.com/en-us/sql/relational-databases/search/find-property-set-guids-and-property-integer-ids-for-search-properties?view=sql-server-ver17

- **Improve the performance of full-text indexes**

  Reworked structure and clarified resource bottlenecks, batching, and crawl behaviors for better tuning. Expanded memory estimation examples, CPU troubleshooting, and index maintenance guidance, and updated applicability to SQL Server 2017+ and Azure services.

  https://learn.microsoft.com/en-us/sql/relational-databases/search/improve-the-performance-of-full-text-indexes?view=sql-server-ver17

- **Improve the performance of full-text queries**

  Updated monikers to 2017+ and streamlined related resources. Minor reorganizations help readers find performance guidance faster.

  https://learn.microsoft.com/en-us/sql/relational-databases/search/improve-the-performance-of-full-text-queries?view=sql-server-ver17

- **Limit Search Results with RANK**

  Limited applicability to SQL Server 2017+, removing SQL Server 2016. This ensures examples and guidance map to current versions.

  https://learn.microsoft.com/en-us/sql/relational-databases/search/limit-search-results-with-rank?view=sql-server-ver17

- **MERGE (Transact-SQL)**

  Adjusted monikers to require SQL Server 2017+, with normalized spacing. No syntax/content changes; the update clarifies version applicability across platforms.

  https://learn.microsoft.com/en-us/sql/t-sql/statements/merge-transact-sql?view=sql-server-ver17

- **Quickstart: Connect to a SQL database from a Jupyter Notebook**

  Updated prerequisites to Python 3.10+, corrected package names, and introduced reproducible devcontainer/Codespaces setup. Simplified database creation via shared includes and expanded next steps for connections and DataFrame/Arrow integrations.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/python-sql-driver-mssql-python-connect-jupyter-notebook?view=sql-server-ver17

- **Quickstart: Python SQL Driver - mssql-python**

  Emphasized secure, passwordless auth for Azure SQL with updated prerequisites and setup includes. Revised connection guidance, expanded .env examples, and streamlined next steps to connection and troubleshooting content.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/python-sql-driver-mssql-python-quickstart?view=sql-server-ver17

- **Quickstart: Python SQL Driver - mssql-python Rapid Prototyping with the Python Driver for SQL Server**

  Centered the quickstart on building a Streamlit prototype with simplified prerequisites. Improved project setup clarity and added next steps for deployment and query execution.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/python-sql-driver-mssql-python-rapid-prototyping-quickstart?view=sql-server-ver17

- **Quickstart: Python SQL Driver - mssql-python Repeatable Deployments with the Python Driver for SQL Server**

  Modernized prerequisites (Python 3.10+), introduced reusable includes, and strengthened configuration and security practices (lockfiles, secret stores). Clarified deployment steps and added next steps for connection and execution topics.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/python-sql-driver-mssql-python-repeatable-deployments-quickstart?view=sql-server-ver17

- **RESTORE Statements (Transact-SQL)**

  Updated monikers to start at SQL Server 2017 with consistent directive spacing. This aligns version targeting without changing restore procedures.

  https://learn.microsoft.com/en-us/sql/t-sql/statements/restore-statements-transact-sql?view=sql-server-ver17

- **Search document properties with search property lists**

  Expanded conceptual and procedural guidance with step-by-step SSMS/T-SQL instructions and images. Clarified behaviors (IDs, repopulation, index size) and updated to SQL Server 2017+ applicability.

  https://learn.microsoft.com/en-us/sql/relational-databases/search/search-document-properties-with-search-property-lists?view=sql-server-ver17

- **Set the service account for the full-text Filter Daemon Launcher**

  Limited scope to SQL Server 2017+ and updated images/formatting for clarity. The article now focuses on on-premises scenarios with consistent syntax.

  https://learn.microsoft.com/en-us/sql/relational-databases/search/set-the-service-account-for-the-full-text-filter-daemon-launcher?view=sql-server-ver17

- **sys.sp_fulltext_database (Transact-SQL)**

  Set minimum version to SQL Server 2017 while retaining Azure applicability. No procedural changes were introduced.

  https://learn.microsoft.com/en-us/sql/relational-databases/system-stored-procedures/sp-fulltext-database-transact-sql?view=sql-server-ver17

- **sp_help_jobhistory (Transact-SQL)**

  Adjusted applicability to SQL Server 2017+ (Windows/Linux). The procedure’s usage and semantics remain unchanged.

  https://learn.microsoft.com/en-us/sql/relational-databases/system-stored-procedures/sp-help-jobhistory-transact-sql?view=sql-server-ver17

- **sys.sp_helprole (Transact-SQL)**

  Updated monikers to require SQL Server 2017+. This ensures version accuracy without altering procedure details.

  https://learn.microsoft.com/en-us/sql/relational-databases/system-stored-procedures/sp-helprole-transact-sql?view=sql-server-ver17

- **sys.sp_helptrigger (Transact-SQL)**

  Removed SQL Server 2016 from applicability by setting minimum to 2017. Content remains functionally consistent.

  https://learn.microsoft.com/en-us/sql/relational-databases/system-stored-procedures/sp-helptrigger-transact-sql?view=sql-server-ver17

- **Troubleshoot full-text indexing**

  Updated applicability to SQL Server 2017+ and standardized terminology and structure. Reorganized guidance helps pinpoint indexing failures and cross-reference related topics faster.

  https://learn.microsoft.com/en-us/sql/relational-databases/search/troubleshoot-full-text-indexing?view=sql-server-ver17

- **Upgrade Full-Text Search (SQL Server Search)**

  Narrowed scope to SQL Server 2017+ with SQL Server-only applicability and clearer import vs rebuild trade-offs. Clarified CPU usage, consistency considerations, and improved examples for realistic upgrade operations.

  https://learn.microsoft.com/en-us/sql/relational-databases/search/upgrade-full-text-search?view=sql-server-ver17

- **Customize Filters and Word Breakers**

  Updated monikers to SQL Server 2017+, removing 2016 references. This keeps configuration guidance aligned with supported releases.

  https://learn.microsoft.com/en-us/sql/relational-databases/search/view-or-change-registered-filters-and-word-breakers?view=sql-server-ver17