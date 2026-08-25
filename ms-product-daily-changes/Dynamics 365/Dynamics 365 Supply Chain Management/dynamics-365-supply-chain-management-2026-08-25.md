# Dynamics 365 Supply Chain Management
**Date created:** 2026-08-25 UTC  
**Tags:** Best Practices, Configuration, Guidance, Performance  

## New Articles

- **Test impact analysis features (production-ready preview)**

  New how-to article for testing Procurement Agent impact analysis. Covers four approaches: forwarding real vendor emails to a sandbox, using live emails in production, testing with Add vendor messages without full email setup, and simulating purchase order change scenarios without supplier communications. Provides guidance to ensure planning data is current, verify downstream demand via Net requirements, create linked demand when needed, and rerun planning before tests. Includes references to related setup and review articles to support end-to-end validation.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/procurement/procurement-agent-impact-analysis-testing

## Moderate Changes

- **Consolidate inventory transactions (preview)**

  Marked the article and feature as preview via title and banners to clarify availability and support expectations. No functional guidance changed, so existing procedures remain the same while the preview status is clearly communicated.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/inventory/inventory-transaction-consolidation

- **Review impact of purchase order changes from vendors (production-ready preview)**

  Streamlined guidance by removing outdated references and excess detail, including the net requirements link from Filter by and the Product dimensions row in the Impacted inventory table. Tightened acceptance criteria to focus on essentials, reducing confusion and keeping the review process current.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/procurement/procurement-agent-impact-analysis-review-changes

- **Use the agent deployment wizard to set up impact analysis features (production-ready preview)**

  Updated to indicate a production-ready preview and removed superseded notes about alternative setup. Clarified that impact analysis runs only with the “Updates from vendors (reading vendor emails)” feature and honors whether email reading is enabled for all or specific vendors, across multiple configurations. This helps admins configure supplier communications correctly.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/procurement/procurement-agent-impact-analysis-setup-wizard

- **How impact analysis works (production-ready preview)**

  Added clear guidance on how impact analysis uses markings and peggings from the current dynamic master plan, with examples of multilevel demand chains. Identified where to set the Current dynamic master plan and removed mixed guidance about external planning to focus on master planning data. This helps users trace downstream impact reliably.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/procurement/procurement-agent-impact-analysis-works

- **Product lifecycle states**

  Clarified that the “BOM report as finished” process applies to the standalone Report as finished function (for example, via the BOM inventory journal), not production orders. This precision helps teams choose the correct completion method and avoid misconfiguring production workflows.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/pim/product-lifecycle