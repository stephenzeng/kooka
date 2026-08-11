# SQL Server
**Date created:** 2026-08-06 UTC  
**Tags:** Administration, Monitoring, Programming  

## New Articles

- **Performance Tuning for the Microsoft Drivers for PHP for SQL Server**

  Introduced comprehensive performance guidance for PHP apps using SQLSRV and PDO_SQLSRV across SQL Server, Azure SQL, and Fabric SQL. Covers connection management and pooling configuration, discourages PDO persistent connections, and recommends per-request connection reuse. Details query and insert best practices, including pagination, efficient fetch modes, prepared batches, TVPs for large loads, and bulk options for massive imports. Explains reducing round trips, managing multiple result sets and MARS trade-offs, tuning prepared statements, and optimizing cursors and LOB streaming. Provides timeout recommendations, read-only routing tips, observability with Query Store and Extended Events, and a deployment checklist.

  https://learn.microsoft.com/en-us/sql/connect/php/performance-tuning-php-sql-driver?view=sql-server-ver17

- **Troubleshoot the Microsoft Drivers for PHP for SQL Server**

  Added a new troubleshooting guide that helps diagnose installation issues, connection and authentication problems, TLS validation, and common PDO/SQLSRV execution errors. Explains handling of data types (UTF-8, datetime, decimal/money), transaction patterns with deadlock retries, and connection resiliency behaviors and limits. Includes steps for enabling driver diagnostics, resolving container/CI runtime dependencies, and sample DSNs and code snippets to accelerate resolution.

  https://learn.microsoft.com/en-us/sql/connect/php/troubleshooting-php-sql-driver?view=sql-server-ver17

## Major Changes

- **Microsoft Drivers for PHP for SQL Server**

  Overhauled the article into a full getting-started hub that clearly distinguishes SQLSRV and PDO_SQLSRV and how they use the Microsoft ODBC Driver. Added a quick-connect example and a production-ready PDO sample with managed identity authentication, TLS settings, retry logic for transient errors, idle connection resiliency, diagnostics, and failover/sovereign cloud guidance. Reorganized content into task-oriented sections and expanded feature notes such as MultiSubnetFailover, ApplicationIntent, HostNameInCertificate, and user-assigned identities. Consolidated links to deeper guidance for performance, troubleshooting, and reference to streamline navigation.

  https://learn.microsoft.com/en-us/sql/connect/php/microsoft-php-driver-for-sql-server?view=sql-server-ver17

- **Troubleshoot High CPU Usage Issues in SQL Server**

  Added a structured Summary with root causes and a prioritized troubleshooting approach, plus clearer steps to confirm SQL Server is the CPU source. Improved guidance on statistics maintenance, identifying CPU-heavy queries, and tracing with Extended Events. Introduced targeted mitigations for SOS_BLOCKALLOCPARTIALLIST spinlock contention on large-memory servers, including verification steps and use of DBCC DROPCLEANBUFFERS and trace flags 8142/8145 with restart considerations, and clarified T174 usage. Updated related resources to include performance monitoring and Query Store best practices.

  https://learn.microsoft.com/en-us/troubleshoot/sql/database-engine/performance/troubleshoot-high-cpu-usage-issues

## Moderate Changes

- **Troubleshoot Slow SQL Server Performance Caused by I/O Issues**

  Added a step-by-step methodology to diagnose I/O bottlenecks using wait types, DMVs, and Windows Performance Monitor counters, with refined terminology and thresholds. Clarified how to distinguish SQL Server from OS-level causes and strengthened guidance on assessing storage capacity and primary drivers of I/O. The article now presents a more prescriptive workflow with renamed sections and links to related topics for deeper follow-up.

  https://learn.microsoft.com/en-us/troubleshoot/sql/database-engine/performance/troubleshoot-sql-io-performance

- **Version Requirements for SQL Server in Windows Operating System**

  Expanded guidance with a Summary and a “How to use this article” section to locate minimum servicing levels and full hardware/software requirements. Clarified cumulative update support across servicing releases and provided direction for cases where a Windows version isn’t listed, including end-of-support planning. Added related links to installation and requirements resources for faster decision-making.

  https://learn.microsoft.com/en-us/troubleshoot/sql/database-engine/install/windows/use-sql-server-in-windows