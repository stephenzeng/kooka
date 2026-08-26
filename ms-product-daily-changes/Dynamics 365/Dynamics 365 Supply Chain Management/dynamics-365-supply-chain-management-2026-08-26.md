# Dynamics 365 Supply Chain Management
**Date created:** 2026-08-26 UTC  
**Tags:** Best Practices, Configuration, Guidance, Performance, Troubleshooting  

## New Articles

- **"Updates not allowed for PurchaseOrderNumber" error when you import purchase order lines**

  New troubleshooting guidance explains why imports fail with “Updates not allowed for PurchaseOrderNumber,” including attempts to change the purchase order number on existing lines or data mismatches that cause unintended record matching. It provides two resolutions: correct the source key in the import file, or use the purchase order consistency check (v10.0.50+) to detect and remove corrupted lines with blank inventory transaction IDs, with instructions for detection versus fix mode. It also advises when to contact Microsoft Support (earlier versions or unresolved cases) and links to related topics to streamline triage.

  https://learn.microsoft.com/en-us/troubleshoot/dynamics-365/supply-chain/procurement/purchase-order-number-update-not-allowed

- **Summary Order Must Be Specified Error on Vendor Invoice**

  Introduces a resolution for the “Summary order must be specified” error during vendor invoice posting. The article clarifies that the issue occurs when Summary update for is set to Order without a valid summary order and walks through fixing it by setting the posting dialog to None or selecting a valid summary order. It also shows how to adjust Summary update parameters to prevent future issues and notes when to involve Microsoft Support.

  https://learn.microsoft.com/en-us/troubleshoot/dynamics-365/supply-chain/procurement/summary-order-must-be-specified

## Major Changes

- **Purchase order line number errors when you import Purchase order lines V2 data**

  The article was significantly expanded to cover two key scenarios: imports that ignore configured line number increments and failures with “Renumbering of lines is not allowed.” It now provides structured guidance with Summary, Symptoms, Cause, and step-by-step Workarounds/Solutions. The update recommends explicitly assigning unique line numbers in source files or enabling renumbering in Procurement and sourcing parameters when stable references aren’t required, with cautions about Dataverse sync and integration stability. Related content links were added to help diagnose adjacent issues.

  https://learn.microsoft.com/en-us/troubleshoot/dynamics-365/supply-chain/procurement/line-number-increments

## Moderate Changes

- **Consolidate inventory transactions (preview)**

  Updated prerequisites advise running Inventory settlements clean up to process closed InventTrans records and cleaning up license plate registration history before consolidation. These steps improve consolidation accuracy and performance, reducing processing time and potential data issues.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/inventory/inventory-transaction-consolidation