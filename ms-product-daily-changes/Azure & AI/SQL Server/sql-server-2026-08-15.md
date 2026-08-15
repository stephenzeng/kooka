# SQL Server
**Date created:** 2026-08-15 UTC  
**Tags:** Best Practices, Configuration, Get Started, Guidance, Performance  

## New Articles

- **High Availability and Disaster Recovery**

  Introduced a comprehensive guide to configure Master Data Services for high availability and disaster recovery using SQL Server Always On availability groups. Covers architecture choices, prerequisites, and detailed steps to set up WSFC, enable AGs, create and validate an availability group, and configure a listener. Provides instructions to connect MDS to the AG listener, validate configuration, and perform failover testing. Highlights design considerations such as synchronous vs. asynchronous replicas and clarifies scope limitations.

  https://learn.microsoft.com/en-us/sql/master-data-services/install-mds-availability-group-environment?view=sql-server-ver16

## Major Changes

- **bcp utility**

  Reorganized the article with platform-specific guidance using moniker sections, separating SQL Server/Azure SQL from Microsoft Fabric Data Warehouse content. Split the Syntax section into engine-specific variants and added Fabric-specific syntax to avoid ambiguity. Expanded the options matrix with a “Supported in Fabric” column and clarified support by platform, with scoped notes for options like -z (vector) and -h (hints). Unified terminology and updated option descriptions for consistency, and clarified native file compatibility and preview status in Fabric to set correct expectations.

  https://learn.microsoft.com/en-us/sql/tools/bcp/bcp-utility?view=sql-server-ver17

## Moderate Changes

- **Microsoft.Data.SqlClient for SQL Server**

  Updated connection guidance to recommend MultiSubnetFailover for TCP endpoints and broadened applicability to Entra-authenticated SQL endpoints across Azure SQL, Managed Instance, Fabric SQL, and SQL Server 2022+ on Azure VMs/Arc. Clarified MultiSubnetFailover behavior (parallel connects) and documented unsupported scenarios, steering users toward Always On availability groups. Enhanced serverless guidance with timeout recommendations, retriable vs. non-retriable errors, and links for auto-pause/resume.

  https://learn.microsoft.com/en-us/sql/connect/ado-net/microsoft-ado-net-sql-server?view=sql-server-ver17

- **Access External Data: Hadoop - PolyBase**

  Strengthened configuration steps, including explicit sp_configure commands, service restarts, and improved pushdown setup with classpath guidance for CDH 5.x. Clarified external table essentials—master key, scoped credentials (Kerberos), and parameter details for external data sources and file formats—and reformatted T-SQL examples for ad hoc queries, import, and export.

  https://learn.microsoft.com/en-us/sql/relational-databases/polybase/polybase-configure-hadoop?view=sql-server-ver15

- **Install from a Command Prompt**

  Expanded command-line installation guidance for SQL Server Machine Learning Services with clearer switches, version-specific feature flags, and consistent example syntax. Reorganized sections for in-database installs, silent setups, and post-install steps, and clarified that SQL Server 2022 no longer installs R/Python/Java runtimes via Setup with updated links for platform-specific guidance.

  https://learn.microsoft.com/en-us/sql/machine-learning/install/sql-ml-component-commandline-install?view=sql-server-ver17

- **Upgrade Integration Services Packages**

  Rewrote and restructured upgrade guidance to clarify methods, expected outcomes, and performance considerations when using dtexec. Added explicit notes for Script components requiring manual reference updates and detailed binding redirect instructions for SSIS designer and custom apps. Organized results content to explain connection provider name changes and recommended alternatives for ADODB-dependent scripts.

  https://learn.microsoft.com/en-us/sql/integration-services/install-windows/upgrade-integration-services-packages?view=sql-server-ver17

- **R Tutorial: Develop a Predictive Model in SQL Server**

  Retitled and refocused the tutorial on SQL Server 2017 with updated prerequisites and clearer client/server setup guidance. Directed package installation through sqlmlutils and standardized code blocks, anchors, and section naming for a smoother learning experience.

  https://learn.microsoft.com/en-us/sql/machine-learning/tutorials/walkthrough-data-science-end-to-end-walkthrough?view=sql-server-ver17