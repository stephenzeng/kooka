# Dynamics 365 Supply Chain Management
**Date created:** 2026-08-21 UTC  
**Tags:** Configuration, Guidance, Performance, Troubleshooting  

## New Articles

- **"Enter the mandatory warehouse" error when you post a product receipt (GRN)**

  Introduced troubleshooting guidance for GRN posting failures caused by mismatches between a purchase order line warehouse and an item configured with a mandatory warehouse. Explains symptoms and root cause, then outlines corrective steps to align the PO line warehouse and validate item setup. Clarifies how default order settings, site-specific overrides, and storage dimension group options affect warehouse requirements, with cautions for shared configuration changes. Includes related references to support deeper investigation.

  https://learn.microsoft.com/en-us/troubleshoot/dynamics-365/supply-chain/procurement/grn-receiving-error-item-transactions-mandatory-warehouse

- **Consolidate inventory transactions**

  Added comprehensive how-to guidance for the inventory transaction consolidation feature to reduce database size and improve performance by archiving detailed transactions and creating summaries. Covers prerequisites, number sequence setup, validations, and step-by-step execution via batch with options to monitor, pause, and resume runs. Highlights business impacts on auditing, inventory closing, costing, and reporting, and provides developer guidance for extending custom fields using the new mapping pattern. Notes version and feature management requirements to enable the capability.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/inventory/inventory-transaction-consolidation

- **Product receipt posting fails with the "only allowed in state draft" error**

  Published troubleshooting steps for product receipt failures when change management prevents document changes during posting. Explains the cause—recalculations triggering changes on a Confirmed PO—and provides a clear recovery path: request change to Draft, recalculate totals, complete approvals, reconfirm, and re-post. Includes links to related procurement and accounting distribution resources to ensure compliant processing.

  https://learn.microsoft.com/en-us/troubleshoot/dynamics-365/supply-chain/procurement/product-receipt-fails-with-changes-only-allowed-in-draft-state-error

## Moderate Changes

- **Import data into Demand planning**

  Added a dedicated troubleshooting section that links to a focused import profile guide, helping users diagnose and resolve common data import issues faster. Improves discoverability of corrective steps without altering core import procedures.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/demand-planning/import-data

- **Consolidate inventory transactions FAQ**

  Removed outdated guidance on bundle size selection and the recommendation to cap transactions per bundle at 100,000. Clarified consolidation rules to ensure transactions for a document consolidate only when all its transactions are eligible, and removed a backdating example that no longer reflects current behavior. This streamlines configuration choices and sets clearer expectations for subsequent runs.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/inventory/inventory-transactions-consolidation-faq

- **What's new or changed in Dynamics 365 Supply Chain Management 10.0.49 (September 2026)**

  Promoted Optimized inventory transaction consolidation from a preview enhancement to an included feature listing, reflecting its updated status. This change helps customers discover and adopt the capability as part of the standard release.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/get-started/whats-new-scm-10-0-49