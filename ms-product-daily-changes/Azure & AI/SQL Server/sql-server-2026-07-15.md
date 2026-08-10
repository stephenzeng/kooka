# SQL Server
**Date created:** 2026-07-15 UTC  
**Tags:** Administration, Automation, Other, Programming, Security  

## Major Changes

- **<a id="release-history"></a> Release history for SQL Server 2019 on Linux**
  Added a new CU 32 GDR (July 2026) entry and detailed section for version 15.0.4480.2 as a security update that incorporates CU 32 and links to KB 5102335. The update is identified as the final cumulative update for SQL Server 2019, with comprehensive package details and download links for RHEL, SLES, and Ubuntu. This helps administrators plan final patching for SQL Server 2019 and retrieve exact packages for offline or manual installation.
  https://learn.microsoft.com/en-us/troubleshoot/sql/releases/linux/release-history-2019

- **Deploy availability groups on Kubernetes with DH2i DxOperator on Azure Kubernetes Service**
  Overhauled the deployment to use a new DxOperator manifest and a new DxSqlAg custom resource with restructured specs, updated sample YAML, and the SQL Server container image set to 2025-latest. Listener configuration is now defined within the custom resource, and service setup requires an additional active-vhost selector label. Commands, options, and verification steps were updated to match the new operator model. These changes streamline AKS deployments and align guidance with the latest DxOperator capabilities.
  https://learn.microsoft.com/en-us/sql/linux/business-continuity/containers/tutorial-kubernetes-dxoperator?view=sql-server-ver17

## Moderate Changes

- **KB5005684 - SQL Server 2025 build versions**
  Added July 14, 2026 GDR and CU+GDR entries across SQL Server 2016, 2017, 2019, 2022, and 2025 build tables, with associated build numbers and KB references. This consolidates the latest security servicing information so administrators can validate current patch levels across supported versions.
  https://learn.microsoft.com/en-us/troubleshoot/sql/releases/sqlserver-2025/build-versions

- **DBCC CHECKDB (Transact-SQL)**
  Added a limitation noting DBCC CHECKDB and DBCC CHECKFILEGROUP aren’t supported in Azure SQL Database Hyperscale and recommending DBCC CHECKTABLE('TableName') WITH TABLOCK as an alternative. Consolidated guidance on memory-optimized tables in Remarks for clearer reference.
  https://learn.microsoft.com/en-us/sql/t-sql/database-console-commands/dbcc-checkdb-transact-sql?view=sql-server-ver17

- **DBCC CHECKFILEGROUP (Transact-SQL)**
  Documented that DBCC CHECKDB and DBCC CHECKFILEGROUP aren’t supported in Azure SQL Database Hyperscale and advised using DBCC CHECKTABLE('TableName') WITH TABLOCK, with links to related integrity and DBCC documentation. This helps teams select supported checks for Hyperscale workloads.
  https://learn.microsoft.com/en-us/sql/t-sql/database-console-commands/dbcc-checkfilegroup-transact-sql?view=sql-server-ver17

- **Download and install the latest updates for SQL Server**
  Added July 2026 GDR and CU+GDR releases for SQL Server 2016–2025, including build numbers and release dates, and appended entries to each version’s history. Centralizing this data simplifies patch selection and compliance checks.
  https://learn.microsoft.com/en-us/troubleshoot/sql/releases/download-and-install-latest-updates

- **Download the Microsoft Drivers for PHP for SQL Server**
  Clarified driver capabilities and supported targets, covering Azure SQL Database, SQL database in Fabric, Azure SQL Managed Instance, and all supported SQL Server versions/editions. Added references to support matrices and engine docs, and noted PHP streams for large objects to guide application design.
  https://learn.microsoft.com/en-us/sql/connect/php/download-drivers-php-sql-server?view=sql-server-ver17

- **Install SQL Server on Server Core**
  Updated applicability to SQL Server 2017 and later and added Windows Server 2025 support while noting SQL Server 2025 doesn’t support Windows Server 2016. Refreshed links to version-specific requirements, updated .NET prerequisites to 4.7.2 (with a note for SQL Server 2017), and generalized upgrade guidance with links to supported paths. These changes help ensure accurate planning for new installs and upgrades on Server Core.
  https://learn.microsoft.com/en-us/sql/database-engine/install-windows/install-sql-server-on-server-core?view=sql-server-ver17

- **Microsoft JDBC Driver for SQL Server**
  Refined the overview to explicitly state support for connecting to the Microsoft SQL Database Engine across Azure SQL services and all supported SQL Server versions/editions. The clarification improves compatibility expectations while maintaining standard JDBC API and app server support guidance.
  https://learn.microsoft.com/en-us/sql/connect/jdbc/microsoft-jdbc-driver-for-sql-server?view=sql-server-ver17

- **Microsoft Drivers for PHP for SQL Server**
  Updated the overview to emphasize accessing the Microsoft SQL Database Engine across Azure SQL services and all supported SQL Server versions/editions. The wording highlights read/write usage and retains guidance on using PHP streams for large objects to inform application development.
  https://learn.microsoft.com/en-us/sql/connect/php/microsoft-php-driver-for-sql-server?view=sql-server-ver17

- **<a id="release-history"></a> Release history for SQL Server 2017 on Linux**
  Added CU 31 GDR (July 2026) to the release history and introduced a detailed section with package details and download links; removed an outdated Azure Connect Pack note from May 2026. This enables precise patching and reduces confusion about prior notes.
  https://learn.microsoft.com/en-us/troubleshoot/sql/releases/linux/release-history-2017

- **<a id="release-history"></a> Release history for SQL Server 2022 on Linux**
  Added a CU 25 GDR (July 2026) entry and a dedicated section summarizing the 16.0.4262.2 security update, with package details and links for manual/offline installs on RHEL, SLES, and Ubuntu. This streamlines retrieval of correct packages for secure updates.
  https://learn.microsoft.com/en-us/troubleshoot/sql/releases/linux/release-history-2022

- **<a id="release-history"></a> Release history for SQL Server 2025 on Linux**
  Added a CU 6 GDR (July 2026) entry and detailed section for version 17.0.4060.2, including KB 5101346 and download links for RHEL 10 and Ubuntu 24.04 packages. The guidance supports fast, accurate patching across key 2025 components.
  https://learn.microsoft.com/en-us/troubleshoot/sql/releases/linux/release-history-2025

- **Release notes for SQL Server 2017 on Linux**
  Updated latest release info to CU 31 GDR (2026-07-14), with build 14.0.3540.1 and refreshed package versions and links for RHEL 8, SLES 12, and Ubuntu 18.04. Added the new entry to the history table to aid version tracking.
  https://learn.microsoft.com/en-us/sql/linux/sql-server-linux-release-notes-2017?view=sql-server-ver17

- **Release notes for SQL Server 2019 on Linux**
  Updated the latest release to CU 32 GDR (Jul 2026) with build 15.0.4480.2 and refreshed package versions for RHEL, SLES, and Ubuntu components. Added the new entry to the release history for complete traceability.
  https://learn.microsoft.com/en-us/sql/linux/sql-server-linux-release-notes-2019?view=sql-server-ver17

- **Release notes for SQL Server 2022 on Linux**
  Reflected CU 25 GDR (Jul 2026) as the latest release and updated package builds to 16.0.4262.2-1 across RHEL 9, SLES 15, and Ubuntu 22.04 (SSIS unchanged). Added the entry to release history to support auditing and servicing workflows.
  https://learn.microsoft.com/en-us/sql/linux/sql-server-linux-release-notes-2022?view=sql-server-ver17

- **Release notes for SQL Server 2025 on Linux**
  Updated “Latest versions for all packages” to CU 6 GDR (Jul 2026), build 17.0.4060.2 with KB 5101346, and refreshed package versions/links for RHEL 10 and Ubuntu 24.04. Added the history entry to document the release.
  https://learn.microsoft.com/en-us/sql/linux/sql-server-linux-release-notes-2025?view=sql-server-ver17

- **Store JSON documents**
  Removed the statement that JSON isn’t a built-in data type, aligning the article with current support for a json data type in storage options. This clarifies architecture choices for developers storing JSON in SQL Server.
  https://learn.microsoft.com/en-us/sql/relational-databases/json/store-json-documents-in-sql-tables?view=sql-server-ver17

- **TDS 8.0**
  Corrected the TLS negotiation matrix: with Encrypt=Optional and clients supporting TLS 1.2 and 1.3 on Windows 11/Windows Server 2022, the negotiated protocol is TLS 1.2 and TDS 8.0 isn’t triggered. This avoids misconfiguration by setting accurate expectations for secure connection behavior.
  https://learn.microsoft.com/en-us/sql/relational-databases/security/networking/tds-8?view=sql-server-ver17