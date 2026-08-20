# Dev and Admin for Dynamics 365 Business Central
**Date created:** 2026-08-20 UTC  
**Tags:** Guidance  

## Moderate Changes

- **Create purchaseInvoiceLines**

  Updated guidance with end-to-end examples for creating a purchase invoice with a single line via deep insert and for adding multiple lines using OData transactional $batch. Clarifies when to choose deep insert versus $batch and demonstrates request structure and the Isolation: snapshot header to ensure atomic rollback.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/api-reference/v2.0/api/dynamics_purchaseInvoiceLine_create

- **Create salesInvoiceLines**

  Expanded guidance to show how to create a sales invoice with a line using deep insert and how to add multiple lines through OData transactional $batch. Provides complete JSON request samples, explains the Isolation: snapshot header, and clarifies selection between deep insert and $batch for reliable, atomic operations.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/api-reference/v2.0/api/dynamics_salesInvoiceLine_create