# Power Query
**Date created:** 2026-08-22 UTC  
**Tags:** Best Practices, Configuration, Get Started, Guidance  

## Moderate Changes

- **SingleStore**

  Updated guidance recommends using native database queries for new reports while confirming SingleStoreODBC.Query remains supported; connection steps now explicitly include Server, Database, Data Connectivity mode, and an optional Native query field. Windows authentication details were clarified, including Kerberos setup and user mapping, and credential management steps were aligned with the new flow. A new limitations section highlights read-only access, lack of DDL support, and potential credential-approval prompts to help plan secure, compliant queries.

  https://learn.microsoft.com/en-us/power-query/connectors/singlestore