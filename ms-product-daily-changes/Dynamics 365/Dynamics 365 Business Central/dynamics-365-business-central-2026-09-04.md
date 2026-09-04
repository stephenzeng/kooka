# Dynamics 365 Business Central
**Date created:** 2026-09-04 UTC  
**Tags:** Configuration, Guidance, Performance, Troubleshooting  

## Major Changes

- **Manage storage by deleting documents or compressing data**

  Introduced the Data Administration page as the centralized entry point for data cleanup. Added categorized actions with detailed scopes across archives, invoiced documents, marketing, cost accounting, and miscellaneous areas to streamline routine deletions. Highlighted irreversible deletions and cautioned to review filters carefully, as some batch jobs run without confirmation. Clarified language in the date compression section without changing functionality.

  https://learn.microsoft.com/en-us/dynamics365/business-central/admin-manage-documents

## Moderate Changes

- **Synchronize inventory with Shopify**

  Expanded troubleshooting with a structured checklist covering stock calculation configuration (including custom extensions), Shopify tracking and locations, and correct item/variant mapping with exclusions for non-inventory and service items. Added guidance on using the Shopify Inventory FactBox and updated log analysis using the inventorySetQuantities filter, including when to enable Logging Mode = All to capture runs and understand suppressed updates when calculated and Shopify stock match.

  https://learn.microsoft.com/en-us/dynamics365/business-central/shopify/synchronize-inventory