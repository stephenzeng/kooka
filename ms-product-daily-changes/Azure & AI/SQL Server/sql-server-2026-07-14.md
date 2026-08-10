# SQL Server
**Date created:** 2026-07-14 UTC  
**Tags:** Administration, Other  

## New Articles

- **Deprecated Full-Text Search Features in SQL Server**

  Introduced a comprehensive reference documenting deprecated full-text search features across SQL Server, Azure SQL Database, and Azure SQL Managed Instance. Provides guidance to monitor deprecated feature usage via performance counters and trace events, helping teams assess impact and plan remediation. Includes tables mapping removed or deprecated features to replacements with feature IDs, covering items like FULLTEXTCATALOGPROPERTY LogSize, FULLTEXTSERVICEPROPERTY timeouts, sp_fulltext_* procedures, dm_fts_* columns, and sys.fulltext_catalogs columns. Details features slated for future removal, such as the generic NEAR operator, certain CREATE FULLTEXT CATALOG options (IN PATH, ON FILEGROUP), DATABASEPROPERTYEX('IsFullTextEnabled'), sp_detach_db @keepfulltextindexfile, and sp_fulltext_service @action=resource_usage, to support forward planning.

  https://learn.microsoft.com/en-us/sql/relational-databases/search/deprecated-full-text-search-features-in-sql-server?view=sql-server-ver17

## Major Changes

- **Fuzzy String Match**

  Clarified platform scope and collation support for fuzzy string matching functions, specifying availability for Azure SQL Database, SQL database in Microsoft Fabric, and Azure SQL Managed Instance with Always-up-to-date policy. Updated guidance confirms Windows and binary (BIN/BIN2) collations are supported, while non-binary SQL_* collations are not. Advises using the COLLATE clause to apply a supported Windows collation when changing database or column collation isn’t feasible, improving accuracy and deployment decisions.

  https://learn.microsoft.com/en-us/sql/relational-databases/fuzzy-string-match/overview?view=fabric-sqldb

## Moderate Changes

- **Start Microsoft Report Builder**

  Narrowed version targeting so that notes on Reporting Services SharePoint integration deprecation and the SharePoint integrated mode startup steps apply only to SQL Server 2016. This refinement ensures version-accurate guidance and reduces confusion for later releases.

  https://learn.microsoft.com/en-us/sql/reporting-services/report-builder/start-report-builder?view=sql-server-ver17