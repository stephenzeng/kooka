# SQL Server
**Date created:** 2026-08-04 UTC  
**Tags:** Administration  

## Moderate Changes

- **SQL Server 2019 Release Notes**

  Added a Known issues subsection covering access violations on Windows Server 2025 when Lock Pages in Memory (LPIM) is enabled, with linked guidance to mitigate the issue. This helps administrators prevent potential crashes by temporarily disabling LPIM until a fix is available.

  https://learn.microsoft.com/en-us/sql/sql-server/sql-server-2019-release-notes?view=sql-server-ver17

- **SQL Server 2022 Release Notes**

  Introduced a new known issue describing access violations on Windows Server 2025 when LPIM is enabled and provided guidance via an include to disable LPIM. This update helps reduce downtime by clarifying immediate mitigation steps.

  https://learn.microsoft.com/en-us/sql/sql-server/sql-server-2022-release-notes?view=sql-server-ver17

- **SQL Server 2025 Known Issues**

  Added a dedicated entry for access violations on Windows Server 2025 with LPIM enabled, including a new anchored section and referenced guidance to disable LPIM. The issues list now links to this section to centralize troubleshooting, helping administrators quickly apply the recommended mitigation.

  https://learn.microsoft.com/en-us/sql/sql-server/sql-server-2025-known-issues?view=sql-server-ver17