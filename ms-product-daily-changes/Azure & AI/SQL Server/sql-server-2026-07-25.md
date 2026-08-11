# SQL Server
**Date created:** 2026-07-25 UTC  
**Tags:** Administration, Security  

## Moderate Changes

- **Extended Security Updates: Frequently asked questions**

  Added a dedicated FAQ explaining how ESU patches are delivered through Microsoft Update, Windows Update, System Center Configuration Manager, and Azure Update Manager, with an option to download from the Azure portal. Clarified that servers with automatic updates enabled will receive ESUs without manual intervention, helping admins verify compliance and streamline patching workflows.

  https://learn.microsoft.com/en-us/sql/sql-server/end-of-support/extended-security-updates-frequently-asked-questions?view=sql-server-ver17

- **MSSQLSERVER_17053**

  Expanded troubleshooting for startup errors 17053 and 5173 caused by OS error 112 when database files (often tempdb) exceed available disk space. Provides a step-by-step recovery: start SQL Server in minimal configuration to connect via DAC, review file sizes in sys.master_files, reduce file sizes with ALTER DATABASE, then restart.

  https://learn.microsoft.com/en-us/sql/relational-databases/errors-events/mssqlserver-17053-database-engine-error?view=sql-server-ver17

- **What are Extended Security Updates for SQL Server?**

  Updated ESU overview to detail patch delivery via Microsoft/Windows Update, System Center Configuration Manager, and Azure Update Manager, with downloadable packages from the Azure portal. Emphasizes that automatic update settings ensure ESUs are applied automatically, simplifying update management for supported instances.

  https://learn.microsoft.com/en-us/sql/sql-server/end-of-support/sql-server-extended-security-updates?view=sql-server-ver17