# Power Query
**Date created:** 2026-07-15 UTC  
**Tags:** Administration  

## Moderate Changes

- **Power Query Oracle database connector**

  Updated guidance to include preview support for the built-in Oracle managed ODP.NET driver for DirectQuery via the on-premises data gateway, along with setup and configuration details. Clarified TNS alias resolution requirements by instructing admins to set TNS_ADMIN at the system scope and restart the gateway service, and revised limitations to reflect preview status. Expanded troubleshooting for DirectQuery TNS resolution errors (ORA-12154, ORA-50201), including checks for system-level TNS_ADMIN and the gateway service account’s access.

  https://learn.microsoft.com/en-us/power-query/connectors/oracle-database