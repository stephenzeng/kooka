# SQL Server
**Date created:** 2026-09-05 UTC  
**Tags:** Automation, Best Practices, Billing, Compliance, Configuration, Deprecation, Get Started, Governance, Guidance, Licensing, Performance, Security, Troubleshooting  

## New Articles

- **Automate the Transition to Pay-as-you-go SQL Licensing at Scale**
  
  Introduces a scripted and policy-based approach to preview, apply, and enforce transitions to pay-as-you-go licensing across Azure Arc–enabled SQL Server, SQL Server on Azure VMs, Azure SQL Database, Azure SQL Managed Instance, and Azure-SSIS IR. Provides a PowerShell tool (manage-payg-transition.ps1) with options for scoping, dry runs, scheduling via Azure Automation, and detailed reporting. Explains required permissions, validations, and safeguards to avoid disruptive changes, and links policy packages for continuous compliance and remediation.
  
  https://learn.microsoft.com/en-us/sql/sql-server/manage-license-type-at-scale?view=sql-server-ver17

## Major Changes

- **AppContext Switches in SqlClient**
  
  Added guidance that SqlClient reads AppContext switches on first use and they must be set at application startup. Introduced several switches to control behaviors: enforce Connection Idle Timeout, enable an experimental V2 connection pool, count pool wait time toward Connect Timeout, revert to legacy failover alternation on login SQL errors, and honor zero scale for vartime parameters. These controls help tune connection reliability, performance, and compatibility in production environments.
  
  https://learn.microsoft.com/en-us/sql/connect/ado-net/appcontext-switches?view=sql-server-ver17

- **Linux and macOS Installation Tutorial for the Microsoft Drivers for PHP for SQL Server**
  
  Designates PIE (PHP Installer for Extensions) as the official replacement for deprecated PECL and adds end-to-end installation steps using PIE. Includes optional attestation, platform-specific guidance for Apple silicon, required build tools, and how PIE handles elevation and dependencies. Updates all platform steps to position PECL as an alternative and streamlines related setup instructions.
  
  https://learn.microsoft.com/en-us/sql/connect/php/installation-tutorial-linux-mac?view=sql-server-ver17

- **Support Lifecycle for mssql-python Driver**
  
  Updates current GA to 1.14.0 and revises version history, noting performance and behavior improvements such as a native parameter binding pipeline and corrected timeout semantics. Clarifies that only 1.14.0 receives fixes, streamlines Python compatibility guidance, and emphasizes companion package requirements at runtime. These changes help teams target the supported version and understand dependency expectations.
  
  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/support-lifecycle?view=sql-server-ver17

## Moderate Changes

- **BULK INSERT (Transact-SQL)**
  
  Updated Fabric Data Warehouse support to mark KEEPIDENTITY as unsupported and adjusted the no-effect options list. Added Fabric-specific guidance to use COPY INTO with IDENTITY_INSERT to preserve identity values, and to employ a format file to map fields explicitly.
  
  https://learn.microsoft.com/en-us/sql/t-sql/statements/bulk-insert-transact-sql?view=sql-server-ver17

- **Manage connections with mssql-python**
  
  Clarifies that the driver has two independent timeouts: login/authentication (SQL_ATTR_LOGIN_TIMEOUT) and per-statement (Connection.timeout), both defaulting to 0. Documents precedence when setting SQL_ATTR_LOGIN_TIMEOUT via attrs_before, updates examples, and notes that Microsoft Entra ID token acquisition occurs before connecting and is not bounded by the authentication timeout.
  
  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/connection-management?view=sql-server-ver17

- **Connection strings for mssql-python**
  
  Clarifies that the “timeout” parameter controls authentication only and points to Connection.timeout for statement limits, with updated examples. Adds guidance to port connection strings from other drivers by mapping keywords and noting unsupported or driver-controlled options, with links to reserved keywords, pooling, and multiple cursors.
  
  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/connection-strings?view=sql-server-ver17

- **DECLARE CURSOR (Transact-SQL)**
  
  Expands FAST_FORWARD documentation to explain runtime selection between STATIC and DYNAMIC based on cost, which may vary per execution. Advises choosing DYNAMIC or KEYSET when concurrent updates must be visible; otherwise prefer STATIC.
  
  https://learn.microsoft.com/en-us/sql/t-sql/language-elements/declare-cursor-transact-sql?view=sql-server-ver17

- **Download the Microsoft Drivers for PHP for SQL Server**
  
  Updates Linux and macOS installation guidance to use PIE, replacing deprecated PECL, while retaining manual download references. This streamlines extension installation and aligns with the supported tooling.
  
  https://learn.microsoft.com/en-us/sql/connect/php/download-drivers-php-sql-server?view=sql-server-ver17

- **Error Handling and SQLSTATE Codes for mssql-python**
  
  Enhances troubleshooting for connection string issues by clarifying causes of unknown or reserved keywords and linking to corrective guidance. Improves discoverability of related sections to resolve errors faster.
  
  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/error-handling?view=sql-server-ver17

- **Install the Microsoft ODBC driver for SQL Server (macOS)**
  
  Adds “brew trust microsoft/mssql-release” after tapping the repository to address Homebrew 6.0+ untrusted tap behavior, with explanatory notes and troubleshooting steps. This prevents installation failures stemming from untrusted sources.
  
  https://learn.microsoft.com/en-us/sql/connect/odbc/linux-mac/install-microsoft-odbc-driver-sql-server-macos?view=sql-server-ver17

- **Loading the Microsoft Drivers for PHP for SQL Server**
  
  Adds Windows guidance to install and enable SQLSRV and PDO_SQLSRV using PIE, including prerequisites like OpenSSL and php.ini configuration. Clarifies installation paths for Linux/macOS using PIE or PECL and updates references to extension filenames accordingly.
  
  https://learn.microsoft.com/en-us/sql/connect/php/loading-the-php-sql-driver?view=sql-server-ver17

- **Configure SQL Server enabled by Azure Arc**
  
  Replaces deprecated modify-license-type.ps1 with manage-payg-transition.ps1 for reviewing and applying license changes at scale. Links to updated prerequisites and Cloud Shell instructions to streamline licensing transitions across SQL resources.
  
  https://learn.microsoft.com/en-us/sql/sql-server/azure-arc/manage-configuration?view=sql-server-ver17

- **Security Best Practices for mssql-python Applications**
  
  Clarifies that Always Encrypted cannot be configured via mssql-python connection strings and removes prior recommendations to use pyodbc for this purpose. Emphasizes alternatives like dynamic data masking and row-level security while noting their different protection levels.
  
  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/security-best-practices?view=sql-server-ver17

- **System requirements for the Microsoft Drivers for PHP for SQL Server**
  
  Updates Linux and macOS installation guidance to use PIE instead of deprecated PECL for driver installation. Links to existing instructions and prebuilt binaries remain unchanged to support varied environments.
  
  https://learn.microsoft.com/en-us/sql/connect/php/system-requirements-for-the-php-sql-driver?view=sql-server-ver17

- **Troubleshoot the Microsoft Drivers for PHP for SQL Server**
  
  Expands installation troubleshooting to include PIE alongside PECL, with required ODBC headers, Apple silicon flags for unixODBC, and PIE install commands. Notes that missing build tools may be required and that PIE can install them on Linux and macOS.
  
  https://learn.microsoft.com/en-us/sql/connect/php/troubleshooting-php-sql-driver?view=sql-server-ver17

- **What's New in mssql-python Driver**
  
  Adds mssql-python 1.14.0 release notes highlighting a native parameter binding pipeline for significant throughput gains, corrected authentication timeout behavior, support for timeout=0 in bulk copy, and better error reporting and Arrow View support. Also merges go-mssqldb v1.11.0 updates including ADO.NET-style connection string synonyms, connection reliability fixes, safer PLP handling, quoting improvements in bulk copy, and charset decoding optimizations.
  
  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/whats-new?view=sql-server-ver17

- **Connection strings for mssql-python**
  
  Adds ADO.NET keyword synonym support for go-mssqldb (ADO-format only) with mapping tables and examples, while clarifying that URL/ODBC formats still require native parameter names. For mssql-python, clarifies authentication vs. statement timeouts and provides keyword substitution guidance when porting from other drivers to avoid errors.
  
  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/connection-strings?view=sql-server-ver17