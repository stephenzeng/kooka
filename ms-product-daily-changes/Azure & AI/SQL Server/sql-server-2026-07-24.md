# SQL Server
**Date created:** 2026-07-24 UTC  
**Tags:** Administration, Programming, Security  

## Moderate Changes

- **Back up a Database Master Key**
  Updated and reorganized guidance to clarify the purpose and procedure for backing up a database master key, with dedicated Limitations and Permissions sections and streamlined, step-by-step T-SQL instructions. Examples were refreshed (AdventureWorks2025), and the article emphasizes secure password storage and removes SSMS UI steps to reduce confusion.
  https://learn.microsoft.com/en-us/sql/relational-databases/security/encryption/back-up-a-database-master-key?view=sql-server-ver17

- **Back up a service master key**
  Corrected the permission requirement to CONTROL SERVER and tightened guidance on risks and secure off-site storage. The backup procedure was streamlined with clear T-SQL steps and password handling cautions, while SSMS UI steps were removed for consistency.
  https://learn.microsoft.com/en-us/sql/relational-databases/security/encryption/back-up-the-service-master-key?view=sql-server-ver17

- **Create a database master key**
  Added explicit Permissions (CONTROL) and a clearer, step-by-step T-SQL procedure with guidance to use strong passwords and store them securely. The article now advises backing up the new key and links to related backup/restore topics for end-to-end key management.
  https://learn.microsoft.com/en-us/sql/relational-databases/security/encryption/create-a-database-master-key?view=sql-server-ver17

- **DBCC SHRINKDATABASE (Transact-SQL)**
  Expanded guidance on WAIT_AT_LOW_PRIORITY (including Fabric SQL Database) and clarified that MAX_DURATION is fixed at one minute, with improved explanations of IAM page locking and timeout error 49516. Updated permissions and known issues, and recommended the ShrinkDriver PowerShell script to orchestrate large shrinks for better reliability and visibility.
  https://learn.microsoft.com/en-us/sql/t-sql/database-console-commands/dbcc-shrinkdatabase-transact-sql?view=sql-server-ver17

- **DBCC SHRINKFILE (Transact-SQL)**
  Strengthened operational guidance, highlighting long-running and resource-intensive behavior, and substantially clarified WAIT_AT_LOW_PRIORITY, timeout behavior, and related errors/permissions. Added practical diagnostics (for example, sys.dm_db_log_space_usage), noted columnstore limitations before SQL Server 2025, and recommended using the ShrinkDriver script for large operations.
  https://learn.microsoft.com/en-us/sql/t-sql/database-console-commands/dbcc-shrinkfile-transact-sql?view=sql-server-ver17

- **Distribution Agent Security**
  Adjusted the moniker range to scope Azure SQL Managed Instance content precisely to the current version, improving version accuracy. No procedural or conceptual changes.
  https://learn.microsoft.com/en-us/sql/relational-databases/replication/distribution-agent-security?view=sql-server-ver17

- **EXECUTE (Transact-SQL)**
  Narrowed a syntax block’s applicability to exactly SQL Server 2017 (Windows and Linux) by refining moniker ranges. No other content changes.
  https://learn.microsoft.com/en-us/sql/t-sql/language-elements/execute-transact-sql?view=sql-server-ver17

- **Install SQL Server Database Engine**
  Broadened the moniker range for Machine Learning Services (In-Database) to include SQL Server 2017 and ver15, ensuring the component’s applicability is accurately reflected. This helps users plan supported installations more confidently.
  https://learn.microsoft.com/en-us/sql/database-engine/install-windows/install-sql-server-database-engine?view=sql-server-ver17

- **Restore a Database Master Key**
  Refocused the article on a T-SQL-only restore workflow with clearer prerequisites, limitations (including FORCE behavior), and a dedicated Permissions section. Updated examples and cautions emphasize secure password handling and reduce reliance on SSMS UI.
  https://learn.microsoft.com/en-us/sql/relational-databases/security/encryption/restore-a-database-master-key?view=sql-server-ver17

- **Restore the Service Master Key**
  Reorganized content with explicit Permissions (CONTROL SERVER), clarified restore behavior including FORCE implications, and advised scheduling during low-demand periods. The procedure and examples were refined for a cleaner T-SQL experience with improved cautions and references.
  https://learn.microsoft.com/en-us/sql/relational-databases/security/encryption/restore-the-service-master-key?view=sql-server-ver17

- **sp_execute_external_script (Transact-SQL)**
  Corrected and standardized moniker ranges to target supported versions more precisely, including narrowing SQL Server 2017 content to exactly that version. No functional T-SQL changes.
  https://learn.microsoft.com/en-us/sql/relational-databases/system-stored-procedures/sp-execute-external-script-transact-sql?view=sql-server-ver17