# SQL Server
**Date created:** 2026-09-02 UTC  
**Tags:** Automation, Compliance, Configuration, Guidance, Identity, Performance, Security, Troubleshooting  

## Major Changes

- **Cannot Connect to WMI Provider Error in SQL Server**

  Reorganized and expanded troubleshooting for the “Cannot connect to WMI provider” error in SQL Server Configuration Manager. Added clear guidance for identifying common error codes, locating the correct MOF file by version (including SQL Server 2025), and enumerating MOF files. Provided two explicit remediation paths—recompiling the provider with mofcomp or repairing the installation—along with when to choose each, and refined commands, steps, and related links.

  https://learn.microsoft.com/en-us/troubleshoot/sql/tools/error-message-when-you-open-configuration-manager

## Moderate Changes

- **What is Microsoft Copilot in SSMA for Oracle (OracleToSQL)?**

  Updated to reflect general availability of the Microsoft-managed endpoint with Microsoft Entra ID authentication in SSMA v10.6 and removed preview labels. Added a Limits section detailing token caps for scripts and prompts and service rate/volume limits to help plan usage and avoid throttling.

  https://learn.microsoft.com/en-us/sql/ssma/oracle/copilot-in-ssma-overview?view=sql-server-ver17

- **How to create In-Memory OLTP App Control and managed installer policies**

  Clarified how HkDllGen works with App Control for Business and AppLocker Managed Installer, noting generated DLLs aren’t Authenticode-signed and are trusted via origin claims. Updated steps to designate hkdllgen.exe as a managed installer, improved PowerShell examples, and added verification methods (including fsutil) to confirm origin claims. Refined wizard guidance, emphasized enabling Managed Installer and audit mode, and updated terminology and references.

  https://learn.microsoft.com/en-us/sql/relational-databases/in-memory-oltp/create-in-memory-oltp-app-control-managed-installer?view=sql-server-ver17

- **Intelligent Query Processing**

  Updated availability to note that Optimized plan forcing with Query Store is available on Azure SQL Managed Instance with SQL Server 2025 or Always-up-to-date update policy, and remains unavailable for the SQL Server 2022 policy. Helps teams plan adoption timing and compatibility.

  https://learn.microsoft.com/en-us/sql/relational-databases/performance/intelligent-query-processing?view=sql-server-ver17

- **What's new in SSMA for Access (AccessToSQL)**

  Added an SSMA v10.6 section highlighting important security, compliance, UX, and accessibility fixes. Helps administrators assess upgrade value and plan deployments.

  https://learn.microsoft.com/en-us/sql/ssma/access/what-s-new-in-ssma-for-access-accesstosql?view=sql-server-ver17

- **What's new in SSMA for Db2 (Db2ToSQL)**

  Added an SSMA v10.6 section summarizing security, compliance, UX, and accessibility improvements. Enables teams to track fixes relevant to regulated and enterprise environments.

  https://learn.microsoft.com/en-us/sql/ssma/db2/what-s-new-in-ssma-for-db2-db2tosql?view=sql-server-ver17

- **What's new in SSMA for MySQL (MySQLToSQL)**

  Added an SSMA v10.6 section noting security, compliance, UX, and accessibility fixes. Encourages updating to benefit from quality and governance improvements.

  https://learn.microsoft.com/en-us/sql/ssma/mysql/what-s-new-in-ssma-for-mysql-mysqltosql?view=sql-server-ver17

- **What's new in SSMA for Oracle (OracleToSQL)**

  Added an SSMA v10.6 section that improves Code conversion Copilot quality, announces general availability of the managed endpoint for SQL Code Conversion Copilot, and fixes DMS auth issues with duplicate subscription names. Also captures security, compliance, UX, and accessibility updates to support reliable migrations.

  https://learn.microsoft.com/en-us/sql/ssma/oracle/what-s-new-in-ssma-for-oracle-oracletosql?view=sql-server-ver17

- **What's new in SSMA for SAP ASE (SybaseToSQL)**

  Added an SSMA v10.6 section announcing GA for AI-assisted code conversion with Copilot in SSMA for SAP ASE and GA for the managed endpoint for SQL Code Conversion Copilot. Also highlighted key security, compliance, UX, and accessibility fixes to strengthen migration workflows.

  https://learn.microsoft.com/en-us/sql/ssma/sybase/what-s-new-in-ssma-for-sybase-sybasetosql?view=sql-server-ver17