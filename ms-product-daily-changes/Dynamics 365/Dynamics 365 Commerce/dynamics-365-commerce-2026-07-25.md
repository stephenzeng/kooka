# Dynamics 365 Commerce
**Date created:** 2026-07-25 UTC  
**Tags:** Administration  

## Moderate Changes

- **Archive credit card transaction data**

  Updated guidance clarifies how to configure the Minimum transaction age, recommending starting with larger values to keep batch durations manageable and noting the default of 91 days. Parameter descriptions were reorganized and clarified, and instructions for token compression were streamlined, including that the Use compression option appears seven days after enabling the feature. These edits improve setup accuracy and governance without changing job functionality.

  https://learn.microsoft.com/en-us/dynamics365/commerce/dev-itpro/archive-cc-data

- **Purge Commerce transactions**

  The purge job documentation now includes RetailReceiptsContent and RetailTransactionPriceTrans in the list of tables that are actively purged, removing prior future-state notes. This ensures receipt content and price transaction data are properly cleaned up, improving data hygiene and compliance.

  https://learn.microsoft.com/en-us/dynamics365/commerce/purge-transactions