# SQL Server
**Date created:** 2026-08-14 UTC  
**Tags:** Best Practices, Configuration, Deprecation, Guidance, Security  

## New Articles

- **Latest Updates and Version History for SQL Server on Linux**

  Introduced a consolidated Linux-focused hub for SQL Server 2025, 2022, 2019, and 2017 that maps builds to update types, KBs, and release dates. Added a quick-reference matrix of the latest CUs and GDRs with links to installation guidance and the master build-version workbook. Highlighted platform support milestones across distributions and versions, plus related links to release notes, known issues, and version discovery.

  https://learn.microsoft.com/en-us/troubleshoot/sql/releases/linux/download-and-install-latest-updates-linux

- **PolyBase EES Encryption on Linux**

  Documented that starting with SQL Server 2025 CU8, PolyBase External Execution Service (EES) communications are encrypted by default using a regenerated self‑signed certificate. Provided certificate details and steps to use a custom CA by placing ca.crt under /var/opt/mssql/polybase-ees and restarting EES. Included operational guidance to restart the service and explained the fallback to unencrypted communication if the certificate is missing or invalid.

  https://learn.microsoft.com/en-us/sql/linux/sql-server-linux-polybase-ees-encryption?view=sql-server-ver17

- **Release Notes for SQL Server on Linux**

  Added per-version release notes (2025, 2022, 2019, 2017) covering supported platforms, tooling, and container tags, noting that SLES is not supported starting with SQL Server 2025. Published a “Latest releases” table with current CU/GDR versions, builds, dates, and KB links, and called out that SQL Server 2019 and 2017 have reached their final CUs. Included installation guidance by version and repository, and linked to full history, known issues, and related quickstarts.

  https://learn.microsoft.com/en-us/sql/linux/sql-server-linux-release-notes?view=sql-server-ver17

## Major Changes

- **Deprecation of AMQP protocol for change event streaming**

  Expanded and clarified AMQP deprecation with platform-specific destination_type requirements and timelines. Specified AzureEventHubs for Azure SQL Database and Microsoft Fabric, and AzureEventHubsApacheKafka for Azure SQL Managed Instance and SQL Server 2025, advising against AzureEventHubsAMQP for new groups. Updated rollout schedules and corrected migration procedures, including the sys.sp_create_event_stream_group family of stored procedures, to streamline transitions.

  https://learn.microsoft.com/en-us/sql/relational-databases/track-changes/change-event-streaming/amqp-deprecation?view=sql-server-ver17

- **Configure change event streaming (preview) to Azure Event Hubs**

  Overhauled configuration guidance by removing SAS token workflows, simplifying setup with shared access policy keys, and strongly recommending Microsoft Entra authentication. Reorganized examples by platform with clear destination_type and endpoint patterns, and added a new limitation for table names containing a period. Clarified TLS requirements for AMQP on Azure SQL MI/SQL Server 2025 (minimum TLS 1.2; not compatible with TLS 1.3) to improve reliability and security.

  https://learn.microsoft.com/en-us/sql/relational-databases/track-changes/change-event-streaming/configure?view=sql-server-ver17

- **sys.sp_create_event_stream_group (Transact-SQL)**

  Extended procedure coverage to Azure SQL Database, Azure SQL Managed Instance, and Microsoft Fabric SQL DB and added an important AMQP deprecation notice. Introduced a platform-specific destination_type matrix recommending AzureEventHubs for Azure SQL Database/Fabric and AzureEventHubsApacheKafka for MI/SQL Server 2025, marking AMQP as deprecated. Updated examples to align with these recommendations and endpoint formats.

  https://learn.microsoft.com/en-us/sql/relational-databases/system-stored-procedures/sys-sp-create-event-stream-group-transact-sql?view=sql-server-ver17

## Moderate Changes

- **SQL Server 2025 build versions (KB5005684)**

  Updated the build table to add CU8 as the latest release with version 17.0.4075.5 (2025.170.4075.5), KB5104822, dated August 13, 2026. Adjusted CU7 so it is no longer marked as Latest.

  https://learn.microsoft.com/en-us/troubleshoot/sql/releases/sqlserver-2025/build-versions

- **dbo.sysjobs (Transact-SQL)**

  Added a Security section clarifying that owner_sid identifies the login that runs T‑SQL job steps and advising minimal, need‑to‑know SELECT access. Updated the owner_sid column description to reinforce this guidance.

  https://learn.microsoft.com/en-us/sql/relational-databases/system-tables/dbo-sysjobs-transact-sql?view=sql-server-ver17

- **sp_add_job (Transact-SQL)**

  Inserted reusable guidance on SQL Server Agent job ownership in the @owner_login_name parameter and Permissions sections. Clarified that only members of the sysadmin fixed server role can set or change @owner_login_name.

  https://learn.microsoft.com/en-us/sql/relational-databases/system-stored-procedures/sp-add-job-transact-sql?view=sql-server-ver17

- **sp_update_job (Transact-SQL)**

  Added ownership and permissions guidance to clarify job ownership requirements after the @owner_login_name parameter and in the Permissions section, improving administrative clarity.

  https://learn.microsoft.com/en-us/sql/relational-databases/system-stored-procedures/sp-update-job-transact-sql?view=sql-server-ver17

- **TRUSTWORTHY Database Property**

  Refined security guidance with clear recommendations to keep TRUSTWORTHY OFF and a warning that db_owner elevation to sysadmin requires both TRUSTWORTHY ON and a sysadmin owner. Updated examples and queries to assess database state and ownership, and streamlined best practices for safer configurations.

  https://learn.microsoft.com/en-us/sql/relational-databases/security/trustworthy-database-property?view=sql-server-ver17