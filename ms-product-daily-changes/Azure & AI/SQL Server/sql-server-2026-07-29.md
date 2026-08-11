# SQL Server
**Date created:** 2026-07-29 UTC  
**Tags:** Programming  

## Moderate Changes

- **Use Bulk Copy with mssql-python Driver**

  Clarified that bulkcopy() opens an internal connection which, starting in mssql-python 1.12.0, inherits the parent connection’s connect timeout (defaulting to 15 seconds if none is set) and snapshots it at call time. Updated guidance recommends increasing the parent connection’s timeout in slow or high‑latency environments and clarifies that the timeout option applies to the bulk operation, not the internal connection.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/bulk-copy?view=sql-server-ver17

- **Install mssql-django**

  Updated version references to 1.7.4 across install steps and compatibility notes. Clarified that pytz remains a required runtime dependency because the backend uses it to convert timezone‑aware datetime values for SQL Server, even when Django uses zoneinfo.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-django/installation?view=sql-server-ver17

- **Support Lifecycle for mssql-python Driver**

  Updated lifecycle information to reflect current GA versions (mssql-python 1.12.0 and mssql-django 1.7.4) and moved prior versions to Previous. Clarified dependency changes: mssql-python now depends on the mssql-python-odbc companion package (auto‑installed and preferred, with fallback to bundled binaries), and reiterated that only the current versions receive updates; also refined notes on pytz usage in the Django backend.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/support-lifecycle?view=sql-server-ver17

- **Troubleshoot mssql-django**

  Added guidance for raw SQL GROUP BY issues that can trigger IndexError with escaped %% and %s parameters, and NotImplementedError when using IntegerChoices. Recommends upgrading to mssql-django 1.7.4, which narrows placeholder rewriting and adjusts type checks so enums and booleans bind correctly.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-django/troubleshooting?view=sql-server-ver17

- **What's New in mssql-python Driver**

  Documented mssql-python 1.12.0, introducing the mssql-python-odbc companion package dependency and improving native loader behavior, plus fixes where cursor.bulkcopy() now honors the parent connection’s connect timeout and supports CLR UDT columns via varbinary(max). Also captured mssql-django 1.7.4 fixes that resolve GROUP BY issues by refining placeholder handling and enum/boolean parameter binding.

  https://learn.microsoft.com/en-us/sql/connect/python/mssql-python/whats-new?view=sql-server-ver17