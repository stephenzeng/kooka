# SQL Server
**Date created:** 2026-07-18 UTC  
**Tags:** AI, Administration, Analytics, Other, Programming, Security  

## Major Changes

- **CREATE EXTERNAL DATA SOURCE (Transact-SQL)**
  Removed all SQL Server 2016-scoped content, including overview, syntax, permissions, and examples for Hadoop and Azure Storage (wasb/wasbs). Guidance now applies to supported versions without legacy 2016 specifics, reducing confusion. This streamlines external data source documentation for current deployments.
  https://learn.microsoft.com/en-us/sql/t-sql/statements/create-external-data-source-transact-sql?view=sql-server-ver17

- **Database Engine events and errors (1000 to 1999)**
  Eliminated SQL Server 2016 moniker content, links, and includes; coverage now starts with SQL Server 2017 and later. This reduces outdated references and aligns error documentation with supported versions. Navigation and includes were cleaned up accordingly.
  https://learn.microsoft.com/en-us/sql/relational-databases/errors-events/database-engine-events-and-errors-1000-to-1999?view=sql-server-ver17

- **Database Engine events and errors (14000 to 14999)**
  Removed all SQL Server 2016-specific content, includes, and version links. The page now targets SQL Server 2017 and later only, simplifying version guidance and ensuring readers use supported references. Error listings for newer versions are unchanged.
  https://learn.microsoft.com/en-us/sql/relational-databases/errors-events/database-engine-events-and-errors-14000-to-14999?view=sql-server-ver17

- **Database Engine events and errors (28000 to 30999)**
  Deleted all SQL Server 2016 moniker sections, includes, and references. Content now focuses on SQL Server 2017 and later, clarifying supported coverage. Version navigation was updated to reflect this scope.
  https://learn.microsoft.com/en-us/sql/relational-databases/errors-events/database-engine-events-and-errors-28000-to-30999?view=sql-server-ver17

- **Database Engine events and errors (41400 to 49999)**
  Removed SQL Server 2016 moniker content, includes, and links. The page now documents errors for SQL Server 2017 and later, improving accuracy for supported environments. Core error data remains intact for current versions.
  https://learn.microsoft.com/en-us/sql/relational-databases/errors-events/database-engine-events-and-errors-41400-to-49999?view=sql-server-ver17

- **Install Machine Learning Server (Standalone) or R Server (Standalone) using SQL Server Setup**
  Removed SQL Server 2016-specific guidance, including R Server (Standalone) steps, VC++ 2013 patch requirements, and associated imagery. The article now focuses on Machine Learning Server (Standalone) for SQL Server 2017 and later. This helps administrators follow current installation paths without legacy dependencies.
  https://learn.microsoft.com/en-us/sql/machine-learning/install/sql-machine-learning-standalone-windows-install?view=sql-server-ver15

- **CAB downloads for offline installation of cumulative updates for SQL Server Machine Learning Services**
  Removed all SQL Server 2016 R Services content, including monikered sections, CAB tables, GDR notes, and prerequisites. Standardized GDR headers for remaining versions and refocused on SQL Server 2017 and 2019. This consolidates offline servicing guidance to supported versions.
  https://learn.microsoft.com/en-us/sql/machine-learning/install/sql-ml-cab-downloads?view=sql-server-ver17

- **Start Microsoft Report Builder**
  Removed SharePoint integrated mode content and the note about integration being unavailable after SQL Server 2016, along with the SharePoint start procedure. The article now centers on launching Report Builder from the SSRS web portal. This reflects current, supported management workflows.
  https://learn.microsoft.com/en-us/sql/reporting-services/report-builder/start-report-builder?view=sql-server-ver17

- **Troubleshoot a Reporting Services installation**
  Removed the full SQL Server 2016 SharePoint mode troubleshooting section, including issues with Configuration Manager, Central Administration, PowerShell cmdlets, URL configuration, setup, and Report Builder in SharePoint. Native mode troubleshooting remains. This aligns content with supported deployment modes and reduces legacy noise.
  https://learn.microsoft.com/en-us/sql/reporting-services/install-windows/troubleshoot-a-reporting-services-installation?view=sql-server-ver17

- **Verify a Reporting Services Installation**
  Removed the SQL Server 2016 SharePoint verification steps, including checks for services, service applications, site features, content types, and sample reports. The article now focuses on verifying Native Mode installations. This simplifies validation for current SSRS deployments.
  https://learn.microsoft.com/en-us/sql/reporting-services/install-windows/verify-a-reporting-services-installation?view=sql-server-ver17

- **Upgrade Python and R runtime with binding in SQL Server Machine Learning Services**
  Scoped guidance to SQL Server 2017 by removing all SQL Server 2016 sections, including 2016 binding considerations and version map. The remaining content focuses on the 2017 version map and procedures. This clarifies upgrade paths for supported versions.
  https://learn.microsoft.com/en-us/sql/machine-learning/install/upgrade-r-and-python?view=sql-server-2017

- **What's new in SQL Server Reporting Services (SSRS)**
  Removed the entire SQL Server 2016 section, including features such as KPIs, mobile reports, SharePoint mode support, rendering improvements, and subscription enhancements. The page now highlights updates relevant to supported versions only. This provides a current, focused view of SSRS advancements.
  https://learn.microsoft.com/en-us/sql/reporting-services/what-s-new-in-sql-server-reporting-services-ssrs?view=sql-server-ver17

## Moderate Changes

- **Access report server items by using URL access**
  Removed SharePoint mode (SQL Server 2016) sections and examples; content now focuses on Native mode URL access. Guidance is streamlined while retaining the XML example.
  https://learn.microsoft.com/en-us/sql/reporting-services/access-report-server-items-using-url-access?view=sql-server-ver17

- **Add a snapshot to report history**
  Dropped SQL Server 2016 Report Manager instructions; the page now targets SQL Server 2017+ web portal workflows. This clarifies snapshot creation for supported versions.
  https://learn.microsoft.com/en-us/sql/reporting-services/report-server/add-a-snapshot-to-report-history-report-manager?view=sql-server-ver17

- **ALTER AVAILABILITY GROUP (Transact-SQL)**
  Corrected manual failover guidance: for two-instance availability groups, run failover on the secondary replica; for Managed Instance link, run on the primary. This prevents operational mistakes during failover.
  https://learn.microsoft.com/en-us/sql/t-sql/statements/alter-availability-group-transact-sql?view=sql-server-ver17

- **ALTER EXTERNAL RESOURCE POOL (Transact-SQL)**
  Removed SQL Server 2016 content and retargeted monikers to 2017+. Syntax and options reflect supported versions without legacy references.
  https://learn.microsoft.com/en-us/sql/t-sql/statements/alter-external-resource-pool-transact-sql?view=sql-server-ver17

- **Author custom code analysis rules**
  Updated prerequisites to require .NET 10 SDK, replacing .NET 8. This ensures compatibility with current tooling for custom rule authoring.
  https://learn.microsoft.com/en-us/sql/tools/sql-database-projects/howto/author-custom-code-analysis-rules?view=sql-server-ver17

- **Backup and restore operations for Reporting Services**
  Removed SQL Server 2016 SharePoint mode content and related links; focus is now Native mode. This clarifies databases and procedures relevant to supported deployments.
  https://learn.microsoft.com/en-us/sql/reporting-services/install-windows/backup-and-restore-operations-for-reporting-services?view=sql-server-ver17

- **Configure Execution Properties for a Report**
  Removed 2016-specific Report Manager steps and links; page now targets SQL Server 2017+. This centers execution property guidance on the current web portal experience.
  https://learn.microsoft.com/en-us/sql/reporting-services/reports/configure-execution-properties-for-a-report-report-manager?view=sql-server-ver17

- **go-mssqldb Connection Strings**
  Added explicit TLS configuration guidance (including TrustServerCertificate) and updated examples. Advised using NewConnectorWithProcessQueryText for scenarios relying on deprecated driver behavior that rewrites '?' placeholders. This improves connection security and forwards compatibility.
  https://learn.microsoft.com/en-us/sql/connect/golang/connection-strings?view=sql-server-ver17

- **Convert an original SQL project to an SDK-style project**
  Updated prerequisites to .NET 10 SDK and added SSMS Database DevOps as a supported tool. Clarified what not to remove during conversion (Pre/PostDeploy, Build items for external .sql files, and non-.sql artifacts). This reduces migration errors and broadens tool support.
  https://learn.microsoft.com/en-us/sql/tools/sql-database-projects/howto/convert-original-sql-project?view=sql-server-ver17

- **Create a local R package repository using miniCRAN**
  Removed SQL Server 2016-specific paths and examples; guidance now targets SQL Server 2017. This aligns package management steps with supported versions.
  https://learn.microsoft.com/en-us/sql/machine-learning/package-management/create-a-local-package-repository-using-minicran?view=sql-server-ver17

- **Create, delete, or modify a folder - Reporting Services**
  Removed 2016 Report Manager procedures; content now covers SQL Server 2017+ web portal steps. This keeps folder management instructions current.
  https://learn.microsoft.com/en-us/sql/reporting-services/report-server/create-delete-or-modify-a-folder-web-portal?view=sql-server-ver17

- **What is SQL Server Reporting Services (SSRS)?**
  Removed the 2016 SharePoint integrated mode section and link. The overview now reflects supported Native mode capabilities.
  https://learn.microsoft.com/en-us/sql/reporting-services/create-deploy-and-manage-mobile-and-paginated-reports?view=sql-server-ver17

- **Tutorial: Create and deploy a SQL project**
  Updated prerequisites to .NET 10 SDK across all pivots. This ensures setup consistency for current SDK-style projects.
  https://learn.microsoft.com/en-us/sql/tools/sql-database-projects/tutorials/create-deploy-sql-project?view=sql-server-ver17

- **CREATE EXTERNAL RESOURCE POOL (Transact-SQL)**
  Removed SQL Server 2016 moniker notes and retargeted syntax/options to SQL Server 2017+. This removes outdated governed-process references.
  https://learn.microsoft.com/en-us/sql/t-sql/statements/create-external-resource-pool-transact-sql?view=sql-server-ver17

- **CREATE EXTERNAL TABLE (Transact-SQL)**
  Adjusted applicability by removing SQL Server 2016 from a behavior section; now scoped to SQL Server 2017–2019 and Linux equivalents. No functional guidance changes.
  https://learn.microsoft.com/en-us/sql/t-sql/statements/create-external-table-transact-sql?view=sql-server-ver17

- **Database Engine events and errors**
  Removed SQL Server 2016 sections and links; page now targets 2017 and later (including Azure variants). This clarifies supported error/event coverage.
  https://learn.microsoft.com/en-us/sql/relational-databases/errors-events/database-engine-events-and-errors?view=sql-server-ver17

- **Database Engine events and errors (0 to 999)**
  Removed SQL Server 2016 moniker sections, links, and includes; page now targets 2017+. Version navigation and includes were aligned accordingly.
  https://learn.microsoft.com/en-us/sql/relational-databases/errors-events/database-engine-events-and-errors-0-to-999?view=sql-server-ver17

- **Database Engine events and errors (10000 to 10999)**
  Removed SQL Server 2016 moniker sections, links, and includes. Version lists now reflect 2017 and later only.
  https://learn.microsoft.com/en-us/sql/relational-databases/errors-events/database-engine-events-and-errors-10000-to-10999?view=sql-server-ver17

- **Database Engine events and errors (11000 to 12999)**
  Removed SQL Server 2016 content, links, and includes; remaining coverage targets 2017+. This reduces outdated references.
  https://learn.microsoft.com/en-us/sql/relational-databases/errors-events/database-engine-events-and-errors-11000-to-12999?view=sql-server-ver17

- **Database Engine events and errors (13000 to 13999)**
  Deleted 2016 moniker sections, links, and includes, aligning the page to 2017+ versions. Core references remain the same for newer versions.
  https://learn.microsoft.com/en-us/sql/relational-databases/errors-events/database-engine-events-and-errors-13000-to-13999?view=sql-server-ver17

- **Database Engine events and errors (15000 to 15999)**
  Removed all 2016-specific content and includes; version navigation now reflects 2017 and later. Error data for supported versions is unchanged.
  https://learn.microsoft.com/en-us/sql/relational-databases/errors-events/database-engine-events-and-errors-15000-to-15999?view=sql-server-ver17

- **Database Engine events and errors (16000 to 17999)**
  Removed SQL Server 2016 sections, links, and includes; the page now targets 2017+ and Azure variants. Version lists were updated accordingly.
  https://learn.microsoft.com/en-us/sql/relational-databases/errors-events/database-engine-events-and-errors-16000-to-17999?view=sql-server-ver17

- **Database Engine events and errors (18000 to 18999)**
  Removed 2016 moniker blocks and references; coverage now focuses on 2017+ (including Linux and Azure variants). Navigation cleaned up to supported versions.
  https://learn.microsoft.com/en-us/sql/relational-databases/errors-events/database-engine-events-and-errors-18000-to-18999?view=sql-server-ver17

- **Database Engine events and errors (19000 to 20999)**
  Eliminated SQL Server 2016 sections and includes; page targets 2017 and later. No changes to the supported error listings themselves.
  https://learn.microsoft.com/en-us/sql/relational-databases/errors-events/database-engine-events-and-errors-19000-to-20999?view=sql-server-ver17

- **Database Engine events and errors (2000 to 2999)**
  Removed SQL Server 2016 moniker section, links, and include; version navigation now lists 2017+ only. This aligns references with supported releases.
  https://learn.microsoft.com/en-us/sql/relational-databases/errors-events/database-engine-events-and-errors-2000-to-2999?view=sql-server-ver17

- **Database Engine events and errors (21000 to 21999)**
  Removed 2016-specific sections, links, and includes; content now targets 2017+ and Azure variants. Version lists were updated to match.
  https://learn.microsoft.com/en-us/sql/relational-databases/errors-events/database-engine-events-and-errors-21000-to-21999?view=sql-server-ver17

- **Database Engine events and errors (22000 to 22999)**
  Removed SQL Server 2016 moniker content, links, and includes; the page now covers 2017+ only. This simplifies version targeting.
  https://learn.microsoft.com/en-us/sql/relational-databases/errors-events/database-engine-events-and-errors-22000-to-22999?view=sql-server-ver17

- **Database Engine events and errors (23000 to 25999)**
  Removed 2016 block, links, and includes; documentation now focuses on 2017+ and Azure variants. Navigation was aligned accordingly.
  https://learn.microsoft.com/en-us/sql/relational-databases/errors-events/database-engine-events-and-errors-23000-to-25999?view=sql-server-ver17

- **Database Engine events and errors (26000 to 27999)**
  Removed SQL Server 2016 moniker sections, links, and includes; page targets 2017+ versions. This reduces outdated content.
  https://learn.microsoft.com/en-us/sql/relational-databases/errors-events/database-engine-events-and-errors-26000-to-27999?view=sql-server-ver17

- **Database Engine events and errors (3000 to 3999)**
  Removed 2016 sections, links, and includes; coverage now starts at 2017+. References and navigation were cleaned up.
  https://learn.microsoft.com/en-us/sql/relational-databases/errors-events/database-engine-events-and-errors-3000-to-3999?view=sql-server-ver17

- **Database Engine events and errors (31000 to 41399)**
  Eliminated SQL Server 2016 moniker content and includes; version lists updated to 2017+. This aligns error references with supported releases.
  https://learn.microsoft.com/en-us/sql/relational-databases/errors-events/database-engine-events-and-errors-31000-to-41399?view=sql-server-ver17

- **Database Engine events and errors (4000 to 4999)**
  Removed SQL Server 2016 moniker section, links, and include; page now focuses on 2017+ and Azure variants. No changes to newer error data.
  https://learn.microsoft.com/en-us/sql/relational-databases/errors-events/database-engine-events-and-errors-4000-to-4999?view=sql-server-ver17

- **Database Engine events and errors (5000 to 5999)**
  Deleted 2016 moniker section, links, and include; content now targets 2017+ versions. This simplifies troubleshooting for supported environments.
  https://learn.microsoft.com/en-us/sql/relational-databases/errors-events/database-engine-events-and-errors-5000-to-5999?view=sql-server-ver17

- **Database Engine events and errors (6000 to 6999)**
  Removed SQL Server 2016 sections, links, and include; page targets 2017+ and Azure variants. Navigation was updated accordingly.
  https://learn.microsoft.com/en-us/sql/relational-databases/errors-events/database-engine-events-and-errors-6000-to-6999?view=sql-server-ver17

- **Database Engine events and errors (7000 to 7999)**
  Removed SQL Server 2016 moniker sections, links, and includes; references now focus on 2017+ versions. Core error content is unchanged for supported versions.
  https://learn.microsoft.com/en-us/sql/relational-databases/errors-events/database-engine-events-and-errors-7000-to-7999?view=sql-server-ver17

- **Database Engine events and errors (8000 to 8999)**
  Removed 2016 moniker content and includes; page now covers 2017+ only. Version navigation cleaned accordingly.
  https://learn.microsoft.com/en-us/sql/relational-databases/errors-events/database-engine-events-and-errors-8000-to-8999?view=sql-server-ver17

- **Database Engine events and errors (9000 to 9999)**
  Removed SQL Server 2016 moniker section, links, and include; documentation now targets 2017+ and Azure variants. This clarifies supported error references.
  https://learn.microsoft.com/en-us/sql/relational-databases/errors-events/database-engine-events-and-errors-9000-to-9999?view=sql-server-ver17

- **Set trace flags with DBCC TRACEON (Transact-SQL)**
  Corrected trace flag descriptions: 8286 now enforces FORCESEEK and 8287 enforces FORCE ORDER. Pairing guidance and applicability remain unchanged.
  https://learn.microsoft.com/en-us/sql/t-sql/database-console-commands/dbcc-traceon-trace-flags-transact-sql?view=sql-server-ver17

- **Export a report by using URL access**
  Removed SQL Server 2016 SharePoint integrated mode export steps and example URL. Export guidance for supported modes remains the same.
  https://learn.microsoft.com/en-us/sql/reporting-services/export-a-report-using-url-access?view=sql-server-ver17

- **R language extension in SQL Server Machine Learning Services**
  Removed SQL Server 2016 from applicability; guidance now targets SQL Server 2017–2019. Content remains otherwise unchanged.
  https://learn.microsoft.com/en-us/sql/machine-learning/concepts/extension-r?view=sql-server-ver17

- **Files-only installation (Reporting Services)**
  Removed SQL Server 2016 SharePoint mode installation link and content. The page now references Native mode setup and configuration.
  https://learn.microsoft.com/en-us/sql/reporting-services/install-windows/files-only-installation-reporting-services?view=sql-server-ver17

- **Install the go-mssqldb Driver**
  Increased the minimum supported Go version to 1.25 and updated terminology to “Microsoft SQL platform.” This clarifies requirements and platform scope.
  https://learn.microsoft.com/en-us/sql/connect/golang/installation?view=sql-server-ver17

- **Install Microsoft Report Builder**
  Removed SQL Server 2016 SharePoint-related installation guidance; starting Report Builder from SSRS or SharePoint-integrated sites remains noted. Focus is on supported scenarios.
  https://learn.microsoft.com/en-us/sql/reporting-services/install-windows/install-report-builder?view=sql-server-ver17

- **Install packages with R tools**
  Removed SQL Server 2016-specific guidance and paths; content now focuses on SQL Server 2017. This streamlines package installation instructions.
  https://learn.microsoft.com/en-us/sql/machine-learning/package-management/install-r-packages-standard-tools?view=sql-server-2017

- **Install SQL Server Database Engine**
  Removed SQL Server 2016-only “R Services (In-Database)” from optional components. The list now reflects supported features like Machine Learning Services.
  https://learn.microsoft.com/en-us/sql/database-engine/install-windows/install-sql-server-database-engine?view=sql-server-ver17

- **Integrate Reporting Services by using SOAP - Web application**
  Removed SQL Server 2016 Report Manager content; focus is now SQL Server 2017+ using the web portal for management and examples for listing reports. This aligns with supported management patterns.
  https://learn.microsoft.com/en-us/sql/reporting-services/application-integration/integrating-reporting-services-using-soap-web-application?view=sql-server-ver17

- **Limit Report History - Reporting Services**
  Removed 2016-specific configuration steps and links; page now covers SQL Server 2017+ behavior. This simplifies history configuration guidance.
  https://learn.microsoft.com/en-us/sql/reporting-services/reports/limit-report-history-report-manager?view=sql-server-ver17

- **Microsoft go-mssqldb Driver for SQL Server**
  Expanded supported targets to include SQL database in Microsoft Fabric and Fabric Data Warehouse. This clarifies connectivity options for new platforms.
  https://learn.microsoft.com/en-us/sql/connect/golang/microsoft-go-mssqldb-driver?view=sql-server-ver17

- **Migrate a Reporting Services Installation (Native Mode)**
  Removed 2016-specific version lists and SharePoint mode migration link; deduplicated version includes. Core migration guidance remains, focused on supported versions.
  https://learn.microsoft.com/en-us/sql/reporting-services/install-windows/migrate-a-reporting-services-installation-native-mode?view=sql-server-ver17

- **Plan for report design and report deployment**
  Removed 2016 SharePoint mode deployment steps; Native mode and programmatic publishing remain. This aligns deployment guidance with supported scenarios.
  https://learn.microsoft.com/en-us/sql/reporting-services/plan-for-report-design-and-report-deployment-reporting-services?view=sql-server-ver17

- **go-mssqldb Queries and Statements**
  Emphasized always calling rows.Close() when stopping iteration early and handling potential server-side errors during token draining. Added a code example demonstrating proper closure and error checks. This reduces resource leaks and hidden errors.
  https://learn.microsoft.com/en-us/sql/connect/golang/queries-statements?view=sql-server-ver17

- **Quickstart: Connect and Query with go-mssqldb**
  Updated prerequisite to Go 1.25 or later. This keeps setup aligned with driver support.
  https://learn.microsoft.com/en-us/sql/connect/golang/quickstart?view=sql-server-ver17

- **Quickstart: Run simple R scripts with SQL machine learning**
  Removed SQL Server 2016 R Services references and scoped to SQL Server 2017+ and Azure SQL Managed Instance ML Services. This modernizes the quickstart for supported ML environments.
  https://learn.microsoft.com/en-us/sql/machine-learning/tutorials/quickstart-r-create-script?view=sql-server-ver17

- **Quickstart: Data structures, data types, and objects using R with SQL machine learning**
  Removed 2016 (R Services) content; page now focuses on SQL Server 2017+ ML Services and Azure SQL Managed Instance. This improves applicability.
  https://learn.microsoft.com/en-us/sql/machine-learning/tutorials/quickstart-r-data-types-and-objects?view=sql-server-ver17

- **Quickstart: R functions with SQL machine learning**
  Removed 2016 R Services references; retained guidance for SQL Server 2017 ML Services and Azure SQL Managed Instance. Ensures relevance for supported offerings.
  https://learn.microsoft.com/en-us/sql/machine-learning/tutorials/quickstart-r-functions?view=sql-server-ver17

- **Quickstart: Create and score a predictive model in R with SQL machine learning**
  Removed 2016 R Services references; content now aligns with SQL Server 2017 ML Services and Azure SQL Managed Instance. This keeps examples consistent with supported runtimes.
  https://learn.microsoft.com/en-us/sql/machine-learning/tutorials/quickstart-r-train-score-model?view=sql-server-ver17

- **Release history for SQL Server 2022 on Linux**
  Added CU 26 (16.0.4265.3, 2026-07-16) with detailed package versions for RHEL 9, SLES 15, and Ubuntu 22.04 and navigation updates. This enables planning and offline installs for the latest CU.
  https://learn.microsoft.com/en-us/troubleshoot/sql/releases/linux/release-history-2022

- **Release history for SQL Server 2025 on Linux**
  Added CU 7 (17.0.4065.4, 2026-07-16) with package details for RHEL 10 and Ubuntu 24.04 and updated release lists/anchors. This supports administrators targeting the newest CU.
  https://learn.microsoft.com/en-us/troubleshoot/sql/releases/linux/release-history-2025

- **SQL Server Reporting Services tools**
  Removed the SQL Server 2016 SharePoint integrated mode section, including Central Administration and PowerShell cmdlet details. Tools guidance now reflects supported SSRS modes.
  https://learn.microsoft.com/en-us/sql/reporting-services/tools/reporting-services-tools?view=sql-server-ver17

- **Paginated report parameters in Report Builder**
  Removed SQL Server 2016 moniker content; applicability now starts with SQL Server 2017. This clarifies supported parameter features.
  https://learn.microsoft.com/en-us/sql/reporting-services/report-design/report-parameters-report-builder-and-report-designer?view=sql-server-ver17

- **Get R package information**
  Removed 2016-specific paths, package lists, and upgrade notes; monikers updated to 2017+. This aligns package references with supported ML Services versions.
  https://learn.microsoft.com/en-us/sql/machine-learning/package-management/r-package-information?view=sql-server-ver17

- **R tutorial: Predict NYC taxi fares with binary classification**
  Removed 2016 R Services content; guidance now targets SQL Server 2017+ and Azure SQL Managed Instance. This modernizes the tutorial’s pre-reqs and context.
  https://learn.microsoft.com/en-us/sql/machine-learning/tutorials/r-taxi-classification-introduction?view=sql-server-ver17

- **R tutorials for SQL machine learning**
  Removed the SQL Server 2016 R Services section; remaining content focuses on SQL Server 2017 and Azure SQL Managed Instance. This simplifies navigation to supported tutorials.
  https://learn.microsoft.com/en-us/sql/machine-learning/tutorials/r-tutorials?view=sql-server-ver17

- **Security architecture for the extensibility framework in SQL Server Machine Learning Services**
  Removed SQL Server 2016 from multiple sections’ moniker ranges, limiting applicability to 2017. This clarifies service identities and processing details for current versions.
  https://learn.microsoft.com/en-us/sql/machine-learning/concepts/security?view=sql-server-ver17

- **sp_execute_external_script (Transact-SQL)**
  Removed SQL Server 2016 R Services language constraints and updated moniker ranges to cover 2017 appropriately. Clarified supported languages (Python and R) for SQL Server 2017 and Azure SQL Managed Instance.
  https://learn.microsoft.com/en-us/sql/relational-databases/system-stored-procedures/sp-execute-external-script-transact-sql?view=sql-server-ver17

- **Install pretrained machine learning models on SQL Server**
  Removed SQL Server 2016-specific guidance (MicrosoftML and component upgrade notes). The article now focuses on SQL Server 2017 and later.
  https://learn.microsoft.com/en-us/sql/machine-learning/install/sql-pretrained-models-install?view=sql-server-ver15

- **SQL projects tools**
  Updated comparison table to mark “Object renaming and refactoring” and “Intellisense from project model” as supported. This reflects current tool capabilities for project development.
  https://learn.microsoft.com/en-us/sql/tools/sql-database-projects/sql-projects-tools?view=sql-server-ver17

- **Release notes for SQL Server 2022 on Linux**
  Updated latest release to CU 26 (16.0.4265.3) with refreshed package versions/links and release history entry. SSIS package versions remain unchanged. This guides administrators to the latest fixes.
  https://learn.microsoft.com/en-us/sql/linux/sql-server-linux-release-notes-2022?view=sql-server-ver17

- **Release notes for SQL Server 2025 on Linux**
  Updated latest release to CU 7 (17.0.4065.4) with new package versions/links for RHEL 10 and Ubuntu 24.04 and a release history update. This ensures accurate update planning.
  https://learn.microsoft.com/en-us/sql/linux/sql-server-linux-release-notes-2025?view=sql-server-ver17

- **Back up and restore SQL Server Reporting Services (SSRS) encryption keys**
  Removed the 2016 SharePoint mode backup section; core prerequisites remain. The page now focuses on supported SSRS modes.
  https://learn.microsoft.com/en-us/sql/reporting-services/install-windows/ssrs-encryption-keys-back-up-and-restore-encryption-keys?view=sql-server-ver17

- **Create a report server database, Report Server Configuration Manager**
  Removed 2016 SharePoint mode content (data alerting database, install-only steps, and SharePoint service application creation). The focus is on supported Native mode configurations.
  https://learn.microsoft.com/en-us/sql/reporting-services/install-windows/ssrs-report-server-create-a-report-server-database?view=sql-server-ver17

- **Tutorial: start from an existing database**
  Updated prerequisites to .NET 10 SDK across all pivots. This keeps project tooling up to date for SDK-style workflows.
  https://learn.microsoft.com/en-us/sql/tools/sql-database-projects/tutorials/start-from-existing-database?view=sql-server-ver17

- **Store Credentials in a Reporting Services Data Source**
  Removed SQL Server 2016 monikered applicability; the page now targets SQL Server 2017+. This clarifies supported credential storage options.
  https://learn.microsoft.com/en-us/sql/reporting-services/report-data/store-credentials-in-a-reporting-services-data-source?view=sql-server-ver17

- **Tutorial: Store the database schema in Git**
  Updated prerequisites to .NET 10 SDK across Visual Studio, VS Code, and CLI. This standardizes environment setup for source control workflows.
  https://learn.microsoft.com/en-us/sql/tools/sql-database-projects/tutorials/store-database-schema-git?view=sql-server-ver17

- **sys.database_scoped_credentials (Transact-SQL)**
  Removed SQL Server 2016-specific column definitions; documentation now targets SQL Server 2017+ and Azure/Fabric. This eliminates duplicate legacy details.
  https://learn.microsoft.com/en-us/sql/relational-databases/system-catalog-views/sys-database-scoped-credentials-transact-sql?view=sql-server-ver17

- **Temporal table considerations and limitations**
  Removed 2016-specific foreign key cascade limitation notes and workarounds. Remaining considerations reflect supported versions.
  https://learn.microsoft.com/en-us/sql/relational-databases/tables/temporal-table-considerations-and-limitations?view=sql-server-ver17

- **go-mssqldb Transactions**
  Added guidance for SET XACT_ABORT ON: treat any statement error as terminal, roll back immediately, and do not attempt further statements or commit. Documented driver behavior to surface server-aborted transactions, preventing silent partial commits.
  https://learn.microsoft.com/en-us/sql/connect/golang/transactions?view=sql-server-ver17