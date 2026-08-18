# SQL Server
**Date created:** 2026-08-18 UTC  
**Tags:** Configuration, Guidance, Monitoring, Performance, Troubleshooting  

## Moderate Changes

- **Configure Extended Events for Availability Groups**

  Updated guidance on configuring and using Extended Events with Always On availability groups. Clarifies the alwayson_health session, standardizes T-SQL session definitions and UI steps, and expands event reference details. Adds troubleshooting for transport/connection issues with filtered error_reported events and documents new diagnostic events available from SQL Server 2019 CU15 to improve monitoring.

  https://learn.microsoft.com/en-us/sql/database-engine/availability-groups/windows/always-on-extended-events?view=sql-server-ver17

- **Compute capacity limits by edition of SQL Server**

  Clarifies that SQL Server doesn't support more than 64 logical cores per NUMA node and details SQL Server 2022 CU11/CU15 behaviors that prevent or warn on unsupported configurations. Provides targeted steps for reducing logical core counts on Azure VMs (disable SMT) and on bare metal (SNC/NPS), and warns that disabling SNC/NPS post-install to exceed 64 logical cores per NUMA node is unsupported. Helps avoid startup failures, reliability issues, and stack dumps.

  https://learn.microsoft.com/en-us/sql/sql-server/compute-capacity-limits-by-edition-of-sql-server?view=sql-server-ver17