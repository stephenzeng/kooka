# SQL Server
**Date created:** 2026-09-03 UTC  
**Tags:** Best Practices, Configuration, Get Started, Guidance, Identity, Performance, Security, Troubleshooting  

## Major Changes

- **Use mssql-python with Apache Arrow**

  Expanded Arrow integration guidance for Python, detailing how arrow_reader() streams results and blocks the connection until the reader is released, with recommended context manager usage and explicit close behaviors. Introduced end-to-end instructions for loading Arrow data into SQL Server via cursor.bulkcopy_arrow(), including accepted Arrow sources and streaming directly from a reader. Clarified type compatibility (for example, use decimal128 for money/decimal) and added options for column mapping and bulk copy settings, with a TypeError note when passing Arrow objects to bulkcopy().

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/arrow-integration?view=sql-server-ver17

- **Use Bulk Copy with mssql-python Driver**

  Prioritized a new bulkcopy_arrow() workflow for columnar ingestion to improve throughput and reduce Python object materialization. Added a comprehensive pandas example converting to Arrow with explicit schema casting (including decimal128) and clarified that NaN maps to SQL NULL on this path. Documented accepted Arrow sources, performance guidance to start from columnar data, and updated behavior so the internal bulk copy connection inherits Connection.timeout set before cursor creation; updated the method comparison to show bulkcopy_arrow() as the fastest for columnar datasets.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/bulk-copy?view=sql-server-ver17

- **Choose a Data Loading and Movement Pattern with mssql-python**

  Recommended bulkcopy_arrow() for DataFrames, Arrow, and Parquet to avoid row-by-row Python conversion and increase throughput. Reworked examples for pandas and Polars to use Arrow with proper decimal casting, added Arrow streaming via RecordBatch/RecordBatchReader, and updated Parquet staging to pass Arrow data directly. Clarified that bulkcopy_arrow() opens its own connection and to commit DDL before calling, and that passing Arrow objects to bulkcopy() raises TypeError.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/data-loading-movement-patterns?view=sql-server-ver17

- **Microsoft Entra Authentication with mssql-python**

  Introduced credential-object authentication via token_provider, with examples using azure-identity (DefaultAzureCredential and others) requesting the database scope. Clarified behavior across operations (fresh token for bulk copy), pooling by identity, and conflicts when combining token_provider with Authentication or raw access tokens, including warnings and errors. Updated access token guidance to prefer token_provider for azure-identity and noted automatic encoding and pooled token refresh.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/entra-authentication?view=sql-server-ver17

- **Use mssql-python with pandas**

  Added guidance to fetch query results into pandas via Arrow using cursor.arrow() and cursor.arrow_reader() to avoid per-value Python objects and enable streaming. Recommended bulk inserts through Arrow with cursor.bulkcopy_arrow(), including explicit schema casting (for example, decimal128) and using Table.cast() to avoid inference issues; positioned traditional bulkcopy() as a fallback for object-heavy DataFrames. Provided multiple Arrow-based code samples for querying, streaming, and loading at scale.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/pandas-integration?view=sql-server-ver17

- **Use mssql-python with Polars**

  Strengthened streaming patterns by using arrow_reader() as a context manager to ensure server-side resources are released on exceptions. Added a full example for bulk insertion via Arrow memory using cursor.bulkcopy_arrow and explained Arrow-to-SQL type compatibility (for example, use decimal128 for money/decimal), with a link to the Arrow integration.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/polars-integration?view=sql-server-ver17

## Moderate Changes

- **mssql-django configuration reference**

  Clarified that with Azure SQL Database serverless auto-pause, the first connection attempt can fail with error 40613 during resume and applications should retry. Retained the recommendation to set connection_timeout to at least 60 seconds and linked to auto-pause/auto-resume guidance.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-django/configuration-reference?view=sql-server-ver17

- **Connect to an Azure SQL database**

  Updated guidance on loginTimeout: keep 30s as a baseline, but increase it for serverless auto-pause scenarios to allow driver retries during resume. Added a reference to connection resiliency for auto-paused databases.

  https://learn.microsoft.com/en-us/sql/connect/jdbc/connecting-to-an-azure-sql-database?view=sql-server-ver17

- **Manage Connections with mssql-python**

  Clarified that the first connection to Azure SQL Database serverless may trigger resume, and short timeouts can expire before it completes. Noted that error 40613 can occur during resume and recommended implementing retries, reinforcing the 60-second timeout recommendation for auto-pause scenarios.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/connection-management?view=sql-server-ver17

- **Connection Pooling with mssql-python**

  Added identity isolation details for connection pools, mapping authentication methods to pool keys and explaining how pools are separated by identity or token hash. Clarified token acquisition behavior, idle pool reclamation, and token-refresh checks before reusing pooled connections.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/connection-pooling?view=sql-server-ver17

- **Connection resiliency (JDBC)**

  Clarified retry timing: the first retry is immediate, subsequent retries follow connectRetryInterval, and the overall sequence is bounded by loginTimeout. Added guidance for connecting to auto-paused serverless databases with recommended settings and sample JDBC URL, warned about replacing (not extending) the transient error list when retryConn lacks a leading plus sign, and refined keepalive wording.

  https://learn.microsoft.com/en-us/sql/connect/jdbc/connection-resiliency?view=sql-server-ver17

- **Connection Strings for mssql-python**

  Enhanced high availability guidance for MultiSubnetFailover, including parallel IP attempts, limits (TCP-only, up to 64 IPs), and mirroring incompatibility. Updated timeout recommendations for serverless auto-pause (first attempt triggers resume, possible 40613, implement retries) and introduced using azure-identity credentials via token_provider, including conflict rules and Entra authentication pointers.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/connection-strings?view=sql-server-ver17

- **Custom Type Converters with mssql-python**

  Extended add_output_converter() to accept Python type keys or integer ODBC SQL type codes, with guidance on when to use each for column selection. Documented converter resolution order and refined the converter function signature details, with examples for DECIMAL/NUMERIC/MONEY behavior.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/custom-type-converters?view=sql-server-ver17

- **Data Type Mappings for mssql-python**

  Removed the version qualifier from the sql_variant mapping entry while keeping the streaming fetch note. Simplified unsupported types guidance by removing prior workarounds and stating they lack native Python mappings.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/data-type-mappings?view=sql-server-ver17

- **JDBC driver support for High Availability, disaster recovery**

  Broadened multiSubnetFailover guidance to include Azure SQL Database, Azure SQL Managed Instance, and SQL database in Microsoft Fabric, and explained behavior with multiple resolved IPs and TNIR. Clarified use with instanceName, limits (>64 IPs fail), incompatibility with mirroring, and recommended increasing loginTimeout for serverless auto-pause scenarios.

  https://learn.microsoft.com/en-us/sql/connect/jdbc/jdbc-driver-support-for-high-availability-disaster-recovery?view=sql-server-ver17

- **Microsoft JDBC Driver for SQL Server**

  Clarified that loginTimeout bounds the full retry sequence and that multiSubnetFailover attempts connections in parallel to all resolved IPs and is safe for single-IP targets. Expanded when to enable multiSubnetFailover, explained retryConn list replacement semantics, and added a section aligning loginTimeout/connectRetry* as a single retry budget that covers serverless resume (40613).

  https://learn.microsoft.com/en-us/sql/connect/jdbc/microsoft-jdbc-driver-for-sql-server?view=sql-server-ver17

- **High availability and disaster recovery**

  Specified that ODBC login timeout must be configured via SQLSetConnectAttr with SQL_ATTR_LOGIN_TIMEOUT before connecting (no connection string keyword). Other edits refined wording for clarity.

  https://learn.microsoft.com/en-us/sql/connect/odbc/odbc-driver-support-for-high-availability-disaster-recovery?view=sql-server-ver17

- **Performance Tuning for mssql-python Applications**

  Added bulkcopy_arrow() as a fourth insert method for columnar sources and provided a pyarrow example emphasizing decimal casting and Table.cast(). Recommended using cursor.arrow() for DataFrame destinations and noted that passing Arrow tables to bulkcopy() raises TypeError.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/performance-tuning?view=sql-server-ver17

- **Quickstart: Apache Arrow with the mssql-python driver for Python**

  Raised the minimum dependency to mssql-python>=1.14.0 and updated the Arrow reader example to iterate streaming results, handle empty streams, and close resources explicitly. Emphasized streaming usage of cursor.arrow_reader() and clarified its behavior versus arrow_batch(), with pointers to deeper Arrow integration content.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/python-sql-driver-mssql-python-arrow-quickstart?view=sql-server-ver17

- **Quickstart: Bulk copy with the mssql-python driver for Python**

  Switched the quickstart to use bulkcopy_arrow for high-performance uploads of Arrow record batches (for example, from Parquet) without converting to Python objects. Updated code and narrative and raised the minimum dependency to mssql-python>=1.14.0.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/python-sql-driver-mssql-python-bulk-copy-quickstart?view=sql-server-ver17

- **Set the connection properties**

  Clarified that loginTimeout bounds the total retry budget (including connectRetryInterval) and should be sized for auto-paused serverless resumes. Expanded multiSubnetFailover guidance across Azure SQL offerings and explained parallel connection attempts to all resolved IPs, with single-IP targets resulting in a single attempt.

  https://learn.microsoft.com/en-us/sql/connect/jdbc/setting-the-connection-properties?view=sql-server-ver17

- **SqlClient support for high availability, disaster recovery**

  Clarified how MultiSubnetFailover opens parallel connections to multiple IPs, why sequential attempts can cause timeouts, and that it does not change failover duration or harm single-IP targets. Updated guidelines to set MultiSubnetFailover=True, use the AG listener, note protocol and IP-count limits, and document incompatibility with mirroring along with upgrade guidance.

  https://learn.microsoft.com/en-us/sql/connect/ado-net/sql/sqlclient-support-high-availability-disaster-recovery?view=sql-server-ver17

- **Understanding timeout properties in the JDBC driver**

  Explained default loginTimeout behavior by driver version and that it bounds overall connection retries, which affects connections to auto-paused Azure SQL Database serverless. Added a cross-reference to guidance for connecting to auto-paused serverless databases.

  https://learn.microsoft.com/en-us/sql/connect/jdbc/understand-timeouts?view=sql-server-ver17