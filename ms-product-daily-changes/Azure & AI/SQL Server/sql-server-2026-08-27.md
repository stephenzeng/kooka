# SQL Server
**Date created:** 2026-08-27 UTC  
**Tags:** Analytics, Best Practices, Configuration, Get Started, Guidance, Identity, Monitoring, Performance, Troubleshooting  

## New Articles

- **queryinsights.external_api_call_stats (Transact-SQL)**

  Introduced a new system view that surfaces function-level diagnostics for external API calls made by AI functions, including counts, execution mode, retries, external wait time, payload sizes, and row outcomes. Clarified how to join with exec_requests_history via distributed_statement_id to analyze specific statements and interpret retry and payload metrics. Provided permissions guidance and six example queries to identify hotspots, quantify external wait, detect row-mode usage, and spot large payloads. Added related links and next steps to streamline troubleshooting and performance analysis.

  https://learn.microsoft.com/en-us/sql/relational-databases/system-views/queryinsights-external-api-call-stats-transact-sql?view=fabric

## Major Changes

- **AI_ANALYZE_SENTIMENT (Transact-SQL)**

  Added an optional ON ERROR clause to control error handling with NULL ON ERROR (default), ERROR ON ERROR, and DEFAULT <value> ON ERROR. Clarified return types and remarks, referencing Responsible AI checks and typical failure scenarios such as input limits and transient issues. Updated examples to demonstrate strict failure behavior with ERROR ON ERROR and explain implications for query execution.

  https://learn.microsoft.com/en-us/sql/t-sql/functions/ai-analyze-sentiment-transact-sql?view=fabric

- **AI_GENERATE_RESPONSE (Transact-SQL)**

  Added an ON ERROR clause to let callers choose between returning NULL, failing the query, or returning a default value when errors occur. Clarified error-handling semantics in remarks and expanded examples, including per-row usage and the default NULL ON ERROR behavior. This update helps developers design predictable pipelines that degrade gracefully or fail fast as needed.

  https://learn.microsoft.com/en-us/sql/t-sql/functions/ai-generate-response-transact-sql?view=fabric

- **AI_SUMMARIZE (Transact-SQL)**

  Introduced an ON ERROR clause that supports NULL ON ERROR (default), ERROR ON ERROR, and DEFAULT <value> ON ERROR. Expanded examples to show using DEFAULT values (for example, 'N/A') and added notes about sending values to the external AI service. Clarified common error causes and how to select behavior that best fits reliability and data quality needs.

  https://learn.microsoft.com/en-us/sql/t-sql/functions/ai-summarize-transact-sql?view=fabric

- **AI_TRANSLATE (Transact-SQL)**

  Added an ON ERROR clause with options to return NULL, fail the query, or emit a specified default when translation fails. Expanded examples cover ERROR ON ERROR and DEFAULT scenarios alongside the default behavior. This gives developers clear control over outcomes during external service issues or content restrictions.

  https://learn.microsoft.com/en-us/sql/t-sql/functions/ai-translate-transact-sql?view=fabric

- **DBCC CHECKIDENT (Transact-SQL)**

  Expanded cross-platform coverage and added a Fabric Data Warehouse section documenting supported behavior: RESEED is supported, custom reseed values aren’t, and running after IDENTITY_INSERT is recommended to prevent conflicts. Clarified syntax and parameters across platforms, added permissions, and provided multiple examples (post-migration, sentinel values, COPY INTO with IDENTITY_INSERT). These updates help ensure consistent identity value management across environments.

  https://learn.microsoft.com/en-us/sql/t-sql/database-console-commands/dbcc-checkident-transact-sql?view=sql-server-ver17

- **What's New in mssql-python Driver**

  Added the 1.13.0 release (August 2026) with packaging changes that require the separate mssql-python-odbc dependency, plus guidance for installs using --no-deps or private indexes. Introduced cursor.bulkcopy_arrow() for Apache Arrow ingestion, a token_provider parameter for Microsoft Entra authentication, and identity-aware connection pooling with token refresh behavior. Included multiple bug fixes (data insertion edge cases, type handling, output converters, Arrow reader cleanup, destructor safety) and streamlined documentation with updated links and performance notes.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/whats-new?view=sql-server-ver17

## Moderate Changes

- **AI_CLASSIFY (Transact-SQL)**

  Added an ON ERROR clause enabling NULL (default), ERROR, or DEFAULT <value> outcomes when classification fails. Documented typical error causes and updated examples to show returning a fallback label like 'unknown'.

  https://learn.microsoft.com/en-us/sql/t-sql/functions/ai-classify-transact-sql?view=fabric

- **AI_EXTRACT (Transact-SQL)**

  Added an optional ON ERROR clause to return NULL, fail the query, or produce a default value on error. Clarified when AI functions return NULL and enumerated likely error causes, improving predictability in extraction workflows.

  https://learn.microsoft.com/en-us/sql/t-sql/functions/ai-extract-transact-sql?view=fabric

- **AI_FIX_GRAMMAR (Transact-SQL)**

  Updated the function to support ON ERROR with NULL (default), ERROR, or DEFAULT <value>. Clarified error causes and refined formatting to improve readability and error-handling guidance.

  https://learn.microsoft.com/en-us/sql/t-sql/functions/ai-fix-grammar-transact-sql?view=fabric

- **Connection Options**

  Expanded guidance for PHP SQL Server connection options, emphasizing MultiSubnetFailover=Yes for Azure SQL, SQL MI, Fabric SQL, AG listeners, and FCIs, and explaining parallel TCP behavior and limitations. Updated recommendations for serverless to use longer LoginTimeout with retry on resume errors and positioned TransparentNetworkIPResolution as legacy behavior.

  https://learn.microsoft.com/en-us/sql/connect/php/connection-options?view=sql-server-ver17

- **Container and Local Development with mssql-python**

  Updated all examples and CI templates to use the 2025-latest SQL Server container image and AdventureWorks 2025 samples. Raised the minimum mssql-python version to 1.13.0 to align environments with the latest driver.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/container-local-development?view=sql-server-ver17

- **COPY INTO (Transact-SQL)**

  For the Fabric moniker, added support for IDENTITY_INSERT with new syntax, parameter details, and an example loading identity columns. Clarified parameter scopes (such as ERRORFILE) and standardized endpoint examples for consistency.

  https://learn.microsoft.com/en-us/sql/t-sql/statements/copy-into-transact-sql?view=azure-sqldw-latest

- **IDENTITY (Function) (Transact-SQL)**

  Added platform-targeted syntax and applies-to coverage, including Fabric Data Warehouse with a simplified form (data_type only). Clarified that Fabric Data Warehouse does not accept seed or increment and updated cross-references and remarks accordingly.

  https://learn.microsoft.com/en-us/sql/t-sql/functions/identity-function-transact-sql?view=sql-server-ver17

- **Support for High Availability, Disaster Recovery**

  Strengthened guidance to enable MultiSubnetFailover for Azure SQL, SQL MI, Fabric SQL, AG listeners, and FCIs, and documented behavior, accepted values, and limitations (TCP-only, 64+ IP failure, no mirroring/Failover_Partner). Added serverless recommendations for LoginTimeout and retry, repositioned TNIR as legacy, and clarified upgrade considerations and incompatibilities.

  https://learn.microsoft.com/en-us/sql/connect/php/php-driver-for-sql-server-support-for-high-availability-disaster-recovery?view=sql-server-ver17

- **Quickstart: Repeatable deployments with the mssql-python driver for Python**

  Updated the pyproject.toml example to require mssql-python>=1.13.0. This ensures new environments align with the latest driver features and packaging model.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/python-sql-driver-mssql-python-repeatable-deployments-quickstart?view=sql-server-ver17

- **queryinsights.exec_requests_history (Transact-SQL)**

  Added a new is_using_external_api column to indicate whether a query invoked AI functions. Included a reference to the external_api_call_stats view for deeper execution diagnostics.

  https://learn.microsoft.com/en-us/sql/relational-databases/system-views/queryinsights-exec-requests-history-transact-sql?view=fabric

- **sys.fn_xe_file_target_read_file (Transact-SQL)**

  Clarified how XEL files are written in buffers and how to read them incrementally at buffer granularity via initial_offset. Updated the definition of file_offset to represent the byte offset of a buffer and aligned result column descriptions.

  https://learn.microsoft.com/en-us/sql/relational-databases/system-functions/sys-fn-xe-file-target-read-file-transact-sql?view=sql-server-ver17

- **sys.identity_columns (Transact-SQL)**

  Expanded applies-to coverage to include Microsoft Fabric and Fabric Data Warehouse. Adjusted wording and links without changing view semantics.

  https://learn.microsoft.com/en-us/sql/relational-databases/system-catalog-views/sys-identity-columns-transact-sql?view=sql-server-ver17

## Minor Changes

- None