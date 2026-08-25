# Power Query
**Date created:** 2026-08-25 UTC  
**Tags:** Best Practices, Configuration, Guidance, Troubleshooting  

## Moderate Changes

- **Transition from ODBC to ADBC drivers in Power BI and Fabric**

  Updated guidance clarifies that tenant and workspace ADBC settings affect only cloud executions, while on-premises gateway refreshes continue using ODBC until future gateway updates. The migration checklist was expanded to emphasize testing via cloud connections, validating behaviors in Power BI Desktop, and recreating queries where needed to ensure ADBC routing. A new FAQ explains testing approaches, gateway implications, inability to permanently opt out, why workspace settings don’t impact Desktop files, that settings don’t rewrite M queries, and how explicit Implementation pins take precedence, with links to connector-specific differences.

  https://learn.microsoft.com/en-us/power-query/transition-to-adbc