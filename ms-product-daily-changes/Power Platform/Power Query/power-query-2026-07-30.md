# Power Query
**Date created:** 2026-07-30 UTC  
**Tags:** Programming, Security  

## Moderate Changes

- **Azure Databricks Power Query connector**

  Updated supported authentication to add Databricks Client Credentials and Service principal (Power Query Online/gateway) and remove Username/Password. This strengthens security by moving away from basic credentials and aligns guidance with current, enterprise-ready auth options.

  https://learn.microsoft.com/en-us/power-query/connectors/databricks-azure

- **TripPin part 7 - Advanced schema with M types**

  Expanded guidance to change the TripPin.Feed schema parameter from table to type and provided an updated M code example for the new function signature. Clarified that GetEntity now calls Table.ChangeType, improving type safety and making sample usage clearer for implementers.

  https://learn.microsoft.com/en-us/power-query/samples/trippin/7-advancedschema/readme