# SQL Server
**Date created:** 2026-08-13 UTC  
**Tags:** Best Practices, Billing, Configuration, Deprecation, Get Started, Guidance, Licensing, Monitoring, Performance, Security, Troubleshooting  

## Major Changes

- **AppContext switches in SqlClient**

  Overhauled guidance on Transparent Network IP Resolution (TNIR) and MultiSubnetFailover, replacing legacy tables with a clearer behavior matrix. Clarifies that on .NET 5+ the TransparentNetworkIPResolution keyword isn’t supported and throws ArgumentException; MultiSubnetFailover is the supported path. Strongly recommends enabling MultiSubnetFailover=True to avoid sequential retry delays, with expanded mitigation steps for long connect scenarios. Adds AppContext details for disabling TNIR by default and notes process-wide options to default-enable MultiSubnetFailover.

  https://learn.microsoft.com/en-us/sql/connect/ado-net/appcontext-switches?view=sql-server-ver17

- **JSON message format - change event streaming**

  Reworked CloudEvents guidance to state the entire event can be serialized as native JSON or Avro, with the data attribute defined as a byte array requiring format-aware deserialization. Updates examples and schema: adopts segmentindex/finalsegment, adds a transaction object (commitlsn, beginlsn, sequencenumber, finalevent, committime), and includes finalevent in the Avro schema. Documents a known issue where committime may incorrectly include a UTC suffix (Z) on non-UTC systems and refines attribute naming and casing.

  https://learn.microsoft.com/en-us/sql/relational-databases/track-changes/change-event-streaming/message-format?view=sql-server-ver17

- **SqlClient support for high availability, disaster recovery**

  Rewrites HADR configuration guidance to recommend MultiSubnetFailover for Microsoft SQL family TCP endpoints (AG listeners, FCIs, Azure SQL Database, Azure SQL Managed Instance, and Fabric SQL), noting it’s safe for single-IP targets and unsupported for named instances or non-TCP. Explains parallel connection attempts across multiple IPs and faster TCP retries for quicker failovers. Consolidates troubleshooting for long connect delays and clarifies when to adjust or disable TNIR, removing prior cautions that could discourage enabling MultiSubnetFailover.

  https://learn.microsoft.com/en-us/sql/connect/ado-net/sql/sqlclient-support-high-availability-disaster-recovery?view=sql-server-ver17

## Moderate Changes

- **Always On failover cluster instances (SQL Server)**

  Updated supported version references for maximum node counts, adding SQL Server 2025 and retaining 2022. Cleaned up older version links and removed references to deprecated versions to keep guidance current.

  https://learn.microsoft.com/en-us/sql/sql-server/failover-clusters/windows/always-on-failover-cluster-instances-sql-server?view=sql-server-ver17

- **Configure change event streaming (preview) to Azure Event Hubs**

  Added a platform-specific known issue where committime in messages may include a UTC suffix (Z) on non-UTC servers, with a fix pending. Reclassified the 4,096 stream group limit (each up to 40,000 tables) as a database-level limit for clearer capacity planning.

  https://learn.microsoft.com/en-us/sql/relational-databases/track-changes/change-event-streaming/configure?view=sql-server-ver17

- **Manage Connections with mssql-python**

  Recommends a connection timeout of at least 60 seconds for Azure SQL Database serverless with auto-pause to allow resume. Advises enabling MultiSubnetFailover=yes for Azure SQL Database, Azure SQL Managed Instance, Microsoft Fabric SQL, AG listeners, and FCIs, noting it’s safe for single-IP targets.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/connection-management?view=sql-server-ver17

- **Connection Strings for mssql-python**

  Clarifies that high availability and failover keywords apply to Always On, Azure SQL targets, and idle connection resiliency. Recommends enabling MultiSubnetFailover across Microsoft SQL family TCP endpoints and setting at least a 60-second timeout for Azure SQL Database serverless scenarios to accommodate resume time.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/connection-strings?view=sql-server-ver17

- **CREATE SERVER AUDIT (Transact-SQL)**

  Expands applicability to Microsoft Fabric (SQL analytics endpoint and Fabric Data Warehouse). Notes that Fabric Data Warehouse supports audit predicates and links to examples and configuration guidance for SQL Audit Logs.

  https://learn.microsoft.com/en-us/sql/t-sql/statements/create-server-audit-transact-sql?view=sql-server-ver17

- **Walkthrough for the Security Features of SQL Server on Linux**

  Updates samples to AdventureWorks2025 and corrects GRANT targets for custom roles. Clarifies least-privilege steps, row-level security behavior, and TDE/backup procedures with consistent terminology and aligned examples.

  https://learn.microsoft.com/en-us/sql/linux/security/get-started?view=sql-server-ver17

- **Manage licensing and billing of SQL Server enabled by Azure Arc**

  Adds pay-as-you-go networking requirements and steps to maintain Azure connectivity for accurate usage uploads. Provides troubleshooting actions if the Azure portal hasn’t received usage for over 24 hours and highlights that blocking outbound connectivity can affect billing accuracy.

  https://learn.microsoft.com/en-us/sql/sql-server/azure-arc/manage-license-billing?view=sql-server-ver17

- **Microsoft JDBC Driver for SQL Server support matrix**

  Moves Microsoft JDBC Driver 9.4 to the “no longer supported” section and records end of mainstream support as July 30, 2026. Helps teams plan upgrades and avoid unsupported client stacks.

  https://learn.microsoft.com/en-us/sql/connect/jdbc/microsoft-jdbc-driver-for-sql-server-support-matrix?view=sql-server-ver17

- **Configure Persistent Memory (PMEM) on Linux**

  Expands guidance on PMEM-aware filesystems and direct access with SQLPAL, recommending -map=mem for performance and -map=dev for very large NVDIMMs. Clarifies that data/tempdb can use fsdax but logs should not unless BTT is configured, and advises validating performance versus NVMe SSDs with updated examples.

  https://learn.microsoft.com/en-us/sql/linux/configure/persistent-memory?view=sql-server-ver17

- **Configure SMB Storage FCI for SQL Server on Linux**

  Fixes multiple command examples and step instructions (e.g., mount/umount usage, rm -f), and clarifies verification steps and user context. Refines SMB/CIFS guidance and references to streamline setup accuracy.

  https://learn.microsoft.com/en-us/sql/linux/business-continuity/failover-cluster-instance/shared-disk-cluster-configure-server-message-block?view=sql-server-ver17

- **Specify a merge article resolver**

  Reorganizes content with clear steps for SSMS and Transact-SQL to register, specify, change, and unregister merge article resolvers. Improves examples, adds anchors and notes (paths and registration commands), and streamlines cross-references.

  https://learn.microsoft.com/en-us/sql/relational-databases/replication/publish/specify-a-merge-article-resolver?view=sql-server-ver17

- **SqlClient troubleshooting guide**

  Adds troubleshooting for long connection delays when DNS returns multiple IPs and sequential retries occur. Recommends setting MultiSubnetFailover=True to enable parallel attempts and links to guidance for disabling TNIR when appropriate.

  https://learn.microsoft.com/en-us/sql/connect/ado-net/sqlclient-troubleshooting-guide?view=sql-server-ver17

- **SQL Server 2025 Known Issues**

  Documents a known issue where committime in change event streaming includes a UTC suffix (Z) on non-UTC systems, even though the value is local time. Notes alignment when the database uses UTC and that a fix is planned.

  https://learn.microsoft.com/en-us/sql/sql-server/sql-server-2025-known-issues?view=sql-server-ver17

- **Troubleshoot Timeout Expired Errors in SQL Server**

  Refocuses on connection timeout errors with guidance to differentiate from query timeouts and to test by increasing connection timeout. Organizes causes into service/port/protocol and name resolution/network issues, adds links for port configuration and pooling, and provides a streamlined troubleshooting path.

  https://learn.microsoft.com/en-us/troubleshoot/sql/database-engine/connect/timeout-expired-error

- **Troubleshoot Query Timeout Errors in SQL Server**

  Centers on identifying and fixing query timeouts, including correlating attention events with completed batches to pinpoint the failing statement. Expands instructions for setting command timeout across client libraries and outlines a clear workflow that prioritizes tuning the slow query.

  https://learn.microsoft.com/en-us/troubleshoot/sql/database-engine/performance/troubleshoot-query-timeouts

- **Troubleshoot Slow-Running Queries in SQL Server**

  Emphasizes a method to distinguish waiting from running time and to find top contributors to elapsed time, with guidance to use Query Store for comparison over time. Refines actions for CPU-bound scenarios and updates structure and references to improve findability and execution.

  https://learn.microsoft.com/en-us/troubleshoot/sql/database-engine/performance/troubleshoot-slow-running-queries

- **Upgrade and migrate Reporting Services**

  Generalizes upgrade guidance to cover upgrades from older versions and updates references to current, version-agnostic procedures. Adjusts the pre-upgrade checklist and points hardware/software requirements to archived documentation for context.

  https://learn.microsoft.com/en-us/sql/reporting-services/install-windows/upgrade-and-migrate-reporting-services?view=sql-server-ver17

- **Tutorial: SQL development for R data scientists**

  Updates prerequisites by removing SQL Server 2016 R Services, standardizing on SQL Server Machine Learning Services with R. Helps align setups with supported components.

  https://learn.microsoft.com/en-us/sql/machine-learning/tutorials/walkthrough-data-science-end-to-end-walkthrough?view=sql-server-ver17