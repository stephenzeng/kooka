# SQL Server
**Date created:** 2026-08-28 UTC  
**Tags:** Automation, Best Practices, Configuration, Deprecation, Guidance, Monitoring, Performance, Security, Troubleshooting  

## Major Changes

- **Create a differential database backup (SQL Server)**

  Expanded and reorganized the article with clearer prerequisites, recommendations, and limitations to help teams plan differential backup strategies. Added end-to-end PowerShell guidance using Backup-SqlDatabase, including module requirements and examples, alongside a refined SSMS walkthrough with notes on recovery models, copy-only constraints, URL backups, media handling, reliability options, and compression defaults. Updated T-SQL guidance with improved syntax explanations and a new AdventureWorks2025 example, and added remarks on tape backups with deprecation context and broader cross-references.

  https://learn.microsoft.com/en-us/sql/relational-databases/backup-restore/create-a-differential-database-backup-sql-server?view=sql-server-ver17

- **Untrusted Certificate Authority Error When You Connect to SQL Server**

  Overhauled troubleshooting for TLS trust failures to clarify root causes such as untrusted CAs and fallback self-signed certificates, and how Schannel evaluates trust. Explained why errors may appear after upgrading drivers/tools by detailing default encryption changes across OLE DB 19, ODBC 18, Microsoft.Data.SqlClient 4.0, and SSMS 20. Organized solutions into three actionable paths: install the issuing CA on clients, connect without certificate validation via documented keywords/UI (with security cautions), or reconfigure encryption by deploying a trusted server certificate and adjusting client/server settings.

  https://learn.microsoft.com/en-us/troubleshoot/sql/database-engine/connect/error-message-when-you-connect

## Moderate Changes

- **Back up and restore SQL Server databases**

  Refined and reorganized guidance for clarity, including updated best practices, standardized code samples, modernized images, and streamlined headings and notes. The glossary was refreshed with clearer definitions, and recommendations now highlight consistent file extensions and adding antivirus exclusions.

  https://learn.microsoft.com/en-us/sql/relational-databases/backup-restore/back-up-and-restore-of-sql-server-databases?view=sql-server-ver17

- **Create a Full Database Backup**

  Reworked recommendations and limitations, adding practical tips like using differential backups for large databases, sizing with sp_spaceused, and suppressing routine backup log entries with trace flag 3226. Clarified version-compatibility limits for restores and expanded device options to include URL targets for Azure Blob or S3-compatible storage, with streamlined SSMS steps and refreshed examples.

  https://learn.microsoft.com/en-us/sql/relational-databases/backup-restore/create-a-full-database-backup-sql-server?view=sql-server-ver17

- **Initialization and authorization properties**

  Clarified that SSPROP_INIT_TNIR controls legacy TransparentNetworkIPResolution fallback and does not affect connection sequencing when MULTISUBNETFAILOVER is enabled. Added recommendations to use MULTISUBNETFAILOVER for Azure SQL, Azure SQL Managed Instance, Microsoft Fabric SQL databases, availability group listeners, and failover cluster instances.

  https://learn.microsoft.com/en-us/sql/connect/oledb/ole-db-data-source-objects/initialization-and-authorization-properties?view=sql-server-ver17

- **OLE DB Driver for SQL Server Support for High Availability, Disaster Recovery**

  Substantially revised guidance for MultiSubnetFailover and ApplicationIntent, expanding coverage to Azure SQL and Microsoft Fabric SQL scenarios. Clarified parallel connection behavior, safety for single-IP targets, unsupported distributed transactions, failure cases without read-only routing, and detailed timeout recommendations—especially for Azure SQL Database serverless with auto-pause. Added programmatic configuration details and modernization notes for migrations from mirroring.

  https://learn.microsoft.com/en-us/sql/connect/oledb/features/oledb-driver-for-sql-server-support-for-high-availability-disaster-recovery?view=sql-server-ver17

- **Release notes - SQL Server enabled by Azure Arc**

  Added a “Current auto-upgrade target version” section (1.1.3518.465) and updated version availability across May–August 2026, marking several prior builds as no longer available. Documented August 2026 changes: least-privilege enabled by default via NT SERVICE\SqlServerExtension and a fix for an authentication token access issue.

  https://learn.microsoft.com/en-us/sql/sql-server/azure-arc/release-notes?view=sql-server-ver17

- **Using connection string keywords with OLE DB Driver for SQL Server**

  Strengthened guidance to enable MultiSubnetFailover for Azure and HA/DR targets and clarified its parallel-IP behavior and safety for single-IP endpoints. Updated timeout recommendations for Azure SQL Database serverless (minimum 60 seconds with retry) and positioned TransparentNetworkIPResolution as a legacy fallback with no effect when MultiSubnetFailover is enabled.

  https://learn.microsoft.com/en-us/sql/connect/oledb/applications/using-connection-string-keywords-with-oledb-driver-for-sql-server?view=sql-server-ver17

- **Using Transparent Network IP Resolution**

  Marked TransparentNetworkIPResolution as legacy and recommended MultiSubnetFailover=Yes for Azure and HA/DR scenarios, noting TNIR has no effect when MultiSubnetFailover is enabled. Simplified the behavioral explanation with a concise table and focused guidance for when MultiSubnetFailover is not used.

  https://learn.microsoft.com/en-us/sql/connect/oledb/features/using-transparent-network-ip-resolution?view=sql-server-ver17