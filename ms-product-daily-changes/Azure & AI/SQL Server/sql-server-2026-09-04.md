# SQL Server
**Date created:** 2026-09-04 UTC  
**Tags:** Best Practices, Configuration, Guidance, Security, Troubleshooting  

## Major Changes

- **Certificate Chain Not Trusted After Driver Upgrade**

  Updated guidance clarifies how encryption and trust keywords apply across OLE DB Driver 19 and ODBC Driver 18, including accepted values, defaults, and strict mode behavior. A new mapping shows which keywords work with each driver and connection method, with links to official keyword references. Solutions were reorganized to prioritize installing a client-trusted TLS certificate, with explicit steps for temporary TrustServerCertificate use and setting encryption to Optional (including DSN UI instructions). The article also explains default encryption changes, backward-compatibility mappings, linked server caveats for MSOLEDBSQL19, and positions older drivers as a short-term mitigation.

  https://learn.microsoft.com/en-us/troubleshoot/sql/database-engine/connect/certificate-chain-not-trusted

## Moderate Changes

- **go-mssqldb Queries and Statements**

  Expanded guidance explains how RowsAffected behaves for stored procedures with SET NOCOUNT ON, AFTER/INSTEAD OF triggers, and multi-statement batches. It advises verifying results when INSTEAD OF triggers return nonzero counts and using separate ExecContext calls to obtain per-statement counts.

  https://learn.microsoft.com/en-us/sql/connect/golang/queries-statements?view=sql-server-ver17