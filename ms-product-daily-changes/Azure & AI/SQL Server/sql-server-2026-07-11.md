# SQL Server
**Date created:** 2026-07-11 UTC  
**Tags:** Administration, Monitoring, Programming, Security  

## New Articles

- **go-mssqldb Always Encrypted**

  Introduced a how-to for using Always Encrypted with the go-mssqldb driver, including enabling via columnencryption and configuring CMK providers (PFX, Windows cert store, Azure Key Vault). Shows Go samples for transparent decryption and parameter encryption with guidance on strict type mapping using driver-specific types. Documents limitations and Azure authentication using DefaultAzureCredential.

  https://learn.microsoft.com/en-us/sql/connect/golang/always-encrypted?view=sql-server-ver17

- **go-mssqldb SQL Server and Windows Authentication**

  Added a driver-focused guide to SQL authentication, Windows integrated auth, NTLM, and Kerberos for Go. Provides decision guidance, connection string formats (URL and ADO), and working examples including Linux/macOS Kerberos prerequisites and options. Links to related topics for Entra ID, encryption, and platform setup.

  https://learn.microsoft.com/en-us/sql/connect/golang/authentication?view=sql-server-ver17

- **go-mssqldb with Azure SQL Database**

  Added an Azure-focused guide for connecting Go apps to Azure SQL, Managed Instance, and Fabric. Covers mandatory TLS settings, passwordless Microsoft Entra ID flows (Default, Managed Identity, Service Principal), firewall and connection limit guidance, and throttling error handling with retries. Includes performance tips, resilience settings, and a troubleshooting checklist.

  https://learn.microsoft.com/en-us/sql/connect/golang/azure-sql?view=sql-server-ver17

- **go-mssqldb Bulk Operations**

  Added step-by-step guidance for high-throughput bulk inserts using mssql.CopyIn, with examples for batching and options (constraints, triggers, tablock). Explains error-handling patterns, CSV streaming, type mapping considerations, and performance best practices. Notes limitations such as lack of support on Azure SQL and Always Encrypted columns.

  https://learn.microsoft.com/en-us/sql/connect/golang/bulk-operations?view=sql-server-ver17

- **go-mssqldb Concurrent Programming**

  Published best practices for safe concurrency with database/sql using go-mssqldb. Explains goroutine-safe types, worker pool patterns, and controlled parallelism to reduce latency and manage throughput. Covers graceful shutdown, pool sizing, and pitfalls like sharing rows or leaving resources open.

  https://learn.microsoft.com/en-us/sql/connect/golang/concurrent-programming?view=sql-server-ver17

- **go-mssqldb Connection Options**

  Introduced a full reference of connection parameters for the driver, including security, failover, performance, diagnostics, and protocol selection. Details encryption/TLS choices, Always Encrypted enablement, and logging flags with bitmasks. Adds examples and links to related connection string and troubleshooting content.

  https://learn.microsoft.com/en-us/sql/connect/golang/connection-options?view=sql-server-ver17

- **go-mssqldb Connection Pooling**

  Added a deep dive into configuring and monitoring the Go database/sql connection pool for SQL Server. Provides recommended settings by scenario, health checks, and strategies to avoid pool exhaustion and stale connections. Introduces SessionInitSQL for per-connection setup and includes metrics/Prometheus examples.

  https://learn.microsoft.com/en-us/sql/connect/golang/connection-pooling?view=sql-server-ver17

- **go-mssqldb Connection Strings**

  Published a consolidated reference for URL, ADO, and ODBC connection string formats with secure configuration guidance. Includes numerous examples, special character handling, and safe construction using net/url and msdsn.Config. Helps teams standardize connection practices and avoid parsing errors.

  https://learn.microsoft.com/en-us/sql/connect/golang/connection-strings?view=sql-server-ver17

- **go-mssqldb Data Type Mappings**

  Documented Go-to-SQL Server type mappings and result scanning behaviors for the driver, including driver-specific types. Provides guidance for precise decimal handling, date/time best practices, NULL semantics, and GUID usage. Includes examples and a quick checklist for reliable data access.

  https://learn.microsoft.com/en-us/sql/connect/golang/data-type-mappings?view=sql-server-ver17

- **Disable SQL Authentication**

  New Azure Arc on Windows guide for SQL Server 2025 explains how to disable SQL authentication to enforce Microsoft Entra and Windows authentication. Details prerequisites, permissions, a migration plan for replacing SQL logins, and portal steps to enable/disable the setting. Includes verification via SERVERPROPERTY and notes on scope and limitations.

  https://learn.microsoft.com/en-us/sql/sql-server/azure-arc/disable-sql-authentication?view=sql-server-ver17

- **go-mssqldb Encryption and Certificates**

  Added TLS configuration guidance including strict/TDS 8.0, mandatory/optional modes, and when to disable in controlled scenarios. Documents certificate validation, CA chains, serverCertificate pinning, and hostname overrides with security cautions. Explains tlsmin and provides robust connection examples.

  https://learn.microsoft.com/en-us/sql/connect/golang/encryption-certificates?view=sql-server-ver17

- **go-mssqldb Microsoft Entra ID Authentication**

  Introduced a comprehensive Entra ID authentication guide for go-mssqldb using azuread and azuresql drivers. Covers all supported flows with connection examples, from Managed Identity and Service Principal to Interactive and On-Behalf-Of. Includes patterns for custom token providers to fit advanced workflows.

  https://learn.microsoft.com/en-us/sql/connect/golang/entra-authentication?view=sql-server-ver17

- **go-mssqldb Error Handling and Retry Patterns**

  Added actionable guidance to classify transient vs. permanent errors and implement resilient retries with backoff and jitter. Explains driver error structures, deadlock handling, and pool monitoring via db.Stats to prevent cascading failures. Provides patterns for common constraint and permission errors and an upsert example with MERGE.

  https://learn.microsoft.com/en-us/sql/connect/golang/error-handling?view=sql-server-ver17

- **Install the go-mssqldb Driver**

  Created an end-to-end installation guide with prerequisites, go get steps, and optional packages for Entra ID and Always Encrypted. Includes a verification program and OS-specific auth notes. Provides upgrade guidance and links to quickstart and related references.

  https://learn.microsoft.com/en-us/sql/connect/golang/installation?view=sql-server-ver17

- **go-mssqldb JSON and XML Data**

  Added patterns for producing and consuming JSON/XML using SQL Server features with Go. Covers FOR JSON/FOR XML streaming, deserialization/unmarshalling, parameter passing, and indexed computed columns for queryable JSON properties. Helps teams choose JSON vs. XML and implement efficient ingestion patterns.

  https://learn.microsoft.com/en-us/sql/connect/golang/json-xml-data?view=sql-server-ver17

- **go-mssqldb Limitations**

  Published a clear inventory of driver limitations with practical workarounds. Covers LastInsertId, MARS, temp table scoping with pooling, Always Encrypted constraints, TLS compatibility nuances, driver naming, and GUID handling. Highlights precision caveats for decimals and platform-specific protocol considerations.

  https://learn.microsoft.com/en-us/sql/connect/golang/known-limitations?view=sql-server-ver17

- **go-mssqldb on Linux and macOS**

  Added cross-platform guidance for authentication options (SQL, NTLM, Kerberos) and clarifies SSPI unavailability on non-Windows. Explains krb5 setup, parameters, and TLS trust store handling with steps to import custom CAs. Provides alternatives including Entra ID via azuresql and links to related topics.

  https://learn.microsoft.com/en-us/sql/connect/golang/linux-macos?view=sql-server-ver17

- **go-mssqldb Logging and Diagnostics**

  Introduced logging controls with flag bitmasks and examples, including SetLogger and context-aware logging. Shows integrations with slog, zerolog, and zap, and how to propagate correlation IDs. Provides production logging recommendations and cautions to protect sensitive data.

  https://learn.microsoft.com/en-us/sql/connect/golang/logging-diagnostics?view=sql-server-ver17

- **Migrate to go-mssqldb from Other Drivers**

  Added a migration guide for teams moving from Postgres/MySQL drivers to go-mssqldb. Maps placeholders to named parameters, covers SQL differences (identity, pagination, JSON access, MERGE), and shows patterns for inserted IDs and bulk operations. Includes an actionable checklist to de-risk migrations.

  https://learn.microsoft.com/en-us/sql/connect/golang/migration-guide?view=sql-server-ver17

- **go-mssqldb Performance Tuning**

  Published a comprehensive optimization guide spanning pool configuration, packet size, prepared statements, and bulk ingestion. Recommends patterns to reduce round trips and implicit conversions, with testing and benchmarking advice. Includes DMV and tooling tips for plan analysis and memory-efficient result processing.

  https://learn.microsoft.com/en-us/sql/connect/golang/performance-tuning?view=sql-server-ver17

- **go-mssqldb Protocols**

  Added reference guidance for selecting and configuring TCP/IP, named pipes, shared memory, and DAC. Explains connection string parameters, naming formats, and platform limitations. Helps choose the right protocol per scenario with examples and related links.

  https://learn.microsoft.com/en-us/sql/connect/golang/protocols?view=sql-server-ver17

- **go-mssqldb Queries and Statements**

  Introduced end-to-end usage patterns with database/sql for querying, DML, batching, and pagination. Details parameterization (positional and named), multiple result sets, and retrieving identity values correctly. Includes transaction and prepared statement guidance with context-based timeouts.

  https://learn.microsoft.com/en-us/sql/connect/golang/queries-statements?view=sql-server-ver17

- **Quickstart: Connect and Query with go-mssqldb**

  Added a quickstart that gets developers connected and querying fast. Provides a complete sample, notes on identity retrieval, and secure connection string guidance. Includes Entra ID authentication with azuresql and links to deeper topics.

  https://learn.microsoft.com/en-us/sql/connect/golang/quickstart?view=sql-server-ver17

- **go-mssqldb Security Best Practices**

  Published prescriptive guidance on parameterization, least privilege, and secret management to reduce risk. Recommends secure TLS settings, TDS 8.0 strict mode, and protecting Always Encrypted keys. Covers safe logging practices and a security checklist to operationalize controls.

  https://learn.microsoft.com/en-us/sql/connect/golang/security-best-practices?view=sql-server-ver17

- **go-mssqldb Stored Procedures**

  Added how-to for calling stored procedures with named parameters, output values, and return status handling. Explains result-set processing order and temp table scope considerations requiring single-connection or transaction usage. Includes examples and guidance for logging PRINT/RAISERROR messages.

  https://learn.microsoft.com/en-us/sql/connect/golang/stored-procedures?view=sql-server-ver17

- **go-mssqldb Support and Lifecycle**

  Introduced a support policy and compatibility matrix for Go versions, SQL platforms, and OSes. Describes support channels for bugs, features, and security, plus TLS compatibility notes for older servers. Helps teams plan platform alignment and upgrades.

  https://learn.microsoft.com/en-us/sql/connect/golang/support-lifecycle?view=sql-server-ver17

- **go-mssqldb Table-Valued Parameters**

  Added a practical guide for using TVPs to pass sets of rows efficiently. Shows SQL types/procedures, Go struct mapping, and how to send empty TVPs with correct schema qualification. Compares TVPs with bulk copy and JSON/XML based on data shape and throughput.

  https://learn.microsoft.com/en-us/sql/connect/golang/table-valued-parameters?view=sql-server-ver17

- **go-mssqldb Test Patterns**

  Added patterns for unit and integration testing with containers, go-sqlmock, and testcontainers-go. Covers environment configuration, isolation with transactions, CI/CD workflows, and retry testing for transient errors. Notes TLS certificate considerations with recent Go versions for SQL Server containers.

  https://learn.microsoft.com/en-us/sql/connect/golang/testing?view=sql-server-ver17

- **go-mssqldb Transactions**

  Published a transactions guide covering isolation levels, error handling, savepoints, and deadlock retries. Explains connection pinning, concurrency guidance, and unsupported distributed transactions with alternatives. Includes read-only routing notes and a practical checklist.

  https://learn.microsoft.com/en-us/sql/connect/golang/transactions?view=sql-server-ver17

- **go-mssqldb Troubleshooting**

  Added a comprehensive troubleshooting playbook for connectivity, auth, pool exhaustion, and performance slowdowns. Provides targeted fixes for Azure SQL scenarios, certificate validation issues, and encoding/collation pitfalls. Includes logging guidance and cross-references to error handling, pooling, and security content.

  https://learn.microsoft.com/en-us/sql/connect/golang/troubleshooting?view=sql-server-ver17

- **Use GORM with go-mssqldb**

  Introduced guidance for using GORM with SQL Server via go-mssqldb, including setup, CRUD, and migrations. Highlights batch insert sizing to respect SQL Server’s parameter limits and shows transaction patterns. Explains pooling configuration and when to mix in raw SQL.

  https://learn.microsoft.com/en-us/sql/connect/golang/use-go-orm-library-with-go-mssqldb?view=sql-server-ver17

- **Use sqlx with go-mssqldb**

  Added a practical guide for sqlx, covering struct scanning, named parameters, IN expansion, and transaction helpers. Provides examples for complex scans and advice on choosing sqlx vs. database/sql vs. GORM. Helps teams adopt ergonomic query patterns without losing control.

  https://learn.microsoft.com/en-us/sql/connect/golang/use-go-sql-extensions-library-with-go-mssqldb?view=sql-server-ver17

- **What's new in go-mssqldb**

  Introduced a release history for the Microsoft fork detailing new parameters, authentication flows, TDS 8.0/strict, Always Encrypted support, and protocol updates. Summarizes fixes and enhancements across performance, TLS/cert handling, and error reporting. Helps teams evaluate upgrades and plan adoption.

  https://learn.microsoft.com/en-us/sql/connect/golang/whats-new?view=sql-server-ver17

## Major Changes

- **Driver Feature Support Matrix**

  Expanded the matrix to fully document go-mssqldb capabilities and renamed the column to “go-mssqldb (Go).” Added support details and version notes for key features including Always Encrypted, multiple Microsoft Entra auth flows, Windows Integrated auth, Bulk Copy, spatial types, TVPs, network resiliency options, and TDS 8.0/TLS 1.3. This helps teams accurately plan feature usage and version alignment for Go workloads.

  https://learn.microsoft.com/en-us/sql/connect/driver-feature-matrix?view=sql-server-ver17

- **Microsoft go-mssqldb Driver for SQL Server**

  Comprehensive rewrite that restructures the driver documentation and adds extensive production guidance, samples, and references. Covers secure connection patterns, Entra/Windows auth, encryption and TDS 8.0, pooling, retries, performance tuning, operations, and troubleshooting. Positions the driver as the official option and centralizes best practices for Go developers targeting SQL Server and Azure SQL.

  https://learn.microsoft.com/en-us/sql/connect/golang/microsoft-go-mssqldb-driver?view=sql-server-ver17

## Moderate Changes

- **Release notes - SQL Server enabled by Azure Arc**

  Added a GA entry for disabling SQL authentication via the Azure portal for Arc-enabled SQL Server. Updates March 2026 notes so admins can adopt external-auth-only configurations confidently.

  https://learn.microsoft.com/en-us/sql/sql-server/azure-arc/release-notes?view=sql-server-ver17

- **SERVERPROPERTY (Transact-SQL)**

  Documented a new SQL Server 2025-specific property, IsExternalAuthenticationOnly, indicating whether SQL authentication is disabled. Helps administrators verify external-auth-only status and align with security guidance.

  https://learn.microsoft.com/en-us/sql/t-sql/functions/serverproperty-transact-sql?view=sql-server-ver17