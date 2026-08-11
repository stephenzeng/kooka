# SQL Server
**Date created:** 2026-07-31 UTC  
**Tags:** Administration, Analytics, Monitoring, Programming, Security  

## Major Changes

- **Configure Change Event Streaming to Azure Event Hubs**

  Clarified message sizing by documenting 1 MB per-column truncation before event formation and how @max_message_size_kb controls message splitting; added guidance to configure max text repl size. Tightened security and networking guidance by removing Kafka SAS token authentication (not supported) and noting AMQP requires Azure Event Hubs minimum TLS 1.2. Expanded platform coverage and destination options, including configuration for Fabric Eventstream custom input endpoints, with reorganized, platform-specific limitations and updated terminology (“stream group”). Clarified Microsoft Entra authentication requirements and availability by platform, and refined parameter guidance for @partition_key_scheme and @max_message_size_kb. Updated DMV references to the system-dynamic-management-objects path.

  https://learn.microsoft.com/en-us/sql/relational-databases/track-changes/change-event-streaming/configure?view=sql-server-ver17

- **What is change event streaming (preview)?**

  Expanded destination support to include Fabric Eventstream and broadened applicability to SQL database in Microsoft Fabric alongside SQL Server 2025, Azure SQL Database, and Azure SQL Managed Instance. Added platform supportability details, including preview feature requirements for SQL Server 2025, Microsoft Entra authentication availability starting with CU3 for Arc-enabled or Azure VM instances, and Managed Instance update policy needs, plus Fabric limitations such as no xEvent debugging or Entra auth. Introduced guidance for consuming events from Fabric Eventstream and standardized terminology from “streaming group” to “stream group.”

  https://learn.microsoft.com/en-us/sql/relational-databases/track-changes/change-event-streaming/overview?view=sql-server-ver17

## Moderate Changes

- **Troubleshoot Intermittent SQL Server Connectivity Issues**

  Added a Summary outlining a data-driven approach using SQLCHECK, SQLTRACE, and SQL Network Analyzer (SQLNA). Refined error and cause sections and expanded diagnostics with concrete steps for collecting client/server traces, interpreting TCP resets, and leveraging NETSTAT outputs. Updated guidance on ephemeral port ranges, TcpTimedWaitDelay, firewall auditing, and impacts from antivirus or network filter drivers, and added related troubleshooting links.

  https://learn.microsoft.com/en-us/troubleshoot/sql/database-engine/connect/intermittent-periodic-network-issue

- **JSON message format - change event streaming**

  Extended applicability to Azure SQL Database, Azure SQL Managed Instance, and SQL database in Microsoft Fabric, and clarified that events can stream to Azure Event Hubs or Fabric Eventstream. Clarified 1 MB truncation per column prior to splitting and how max_message_size_kb governs segmenting and ordering; corrected the data example to use eventrow and renamed JSON schema headings to AVRO schema. Improved CloudEvents attribute explanations, including uniqueness of source+id and extension attribute terminology.

  https://learn.microsoft.com/en-us/sql/relational-databases/track-changes/change-event-streaming/message-format?view=sql-server-ver17

- **Prerequisites and Checklist for Resolving Connectivity Errors**

  Introduced a Summary describing a two-part approach—diagnostic prerequisites and a quick checklist—to streamline troubleshooting. Reorganized steps to prioritize reviewing SQLCHECK output and provided clearer, actionable checks for logs, connection strings, services/listeners, TCP/IP, aliases, TLS/DH, SPNs, Kerberos, and permissions. Added related links to deep-dive connectivity topics.

  https://learn.microsoft.com/en-us/troubleshoot/sql/database-engine/connect/resolve-connectivity-errors-checklist

- **Secure reports and resources**

  Added an IMPORTANT note clarifying that a report is not a security boundary and that data access must be enforced at the data source (for example, RLS/OLS or database permissions). Clarified that folder permissions, role assignments, and hidden parameters govern access to the report artifact but not the underlying data returned.

  https://learn.microsoft.com/en-us/sql/reporting-services/security/secure-reports-and-resources?view=sql-server-ver17

- **Credentials and connections for report data sources**

  Added guidance that when stored credentials are used, all users run under the same identity, preventing per-user data access enforcement. Recommended Windows Integrated Security with data source–level controls for user-specific authorization and reiterated that a report is not a security boundary.

  https://learn.microsoft.com/en-us/sql/reporting-services/report-data/specify-credential-and-connection-information-for-report-data-sources?view=sql-server-ver17

- **sys.dm_change_feed_errors (Transact-SQL)**

  Expanded applicability to Azure SQL Managed Instance and SQL database in Microsoft Fabric. Updated behavior to store up to the 64 most recently logged errors, with clarification that multiple errors can occur per session. Documented that rows appear only when change feed features are configured and have logged errors, and that entries rotate and clear on engine restart or when the change feed is disabled.

  https://learn.microsoft.com/en-us/sql/relational-databases/system-dynamic-management-objects/sys-dm-change-feed-errors?view=sql-server-ver17

- **What's new in SQL Server 2025**

  Clarified that Change event streaming captures row-level DML changes on tracked tables and publishes to Azure Event Hubs or Fabric Eventstream. Noted that each change is emitted as a CloudEvent containing current schema, previous values, and new values in JSON or Avro, and that Microsoft Entra authentication is available for Arc-enabled or Azure VM instances starting with CU3.

  https://learn.microsoft.com/en-us/sql/sql-server/what-s-new-in-sql-server-2025?view=sql-server-ver17