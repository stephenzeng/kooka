# Dynamics 365 Business Central
**Date created:** 2026-08-27 UTC  
**Tags:** Best Practices, Compliance, Configuration, Get Started, Guidance, Troubleshooting  

## New Articles

- **Synchronize inventory with Shopify**

  Introduced a dedicated how-to for configuring and running inventory synchronization between Business Central and Shopify. The article explains prerequisites, enabling sync per Shopify Location, and how stock is calculated, including projected and free inventory examples. It clarifies handling of locations and fulfillment services, use of the Default Product Location toggle, and how Business Central replenishment updates Shopify availability. It also recommends scheduling sync with job queues and provides troubleshooting steps for common setup and data-linking issues.

  https://learn.microsoft.com/en-us/dynamics365/business-central/shopify/synchronize-inventory

- **Synchronize prices with Shopify**

  Introduced comprehensive guidance for price synchronization, including main and compare-at prices, and the configuration fields that drive price calculations. The article outlines the operational flow, lowest-price logic, bulk updates, and visibility into skipped records. It adds coverage for B2B pricing via Shopify B2B Catalogs and market-specific pricing via Shopify Markets, including currency handling. It also aligns Business Central settings with Shopify tax behaviors for domestic, international, and EU VAT scenarios to ensure storefront prices match expectations.

  https://learn.microsoft.com/en-us/dynamics365/business-central/shopify/synchronize-prices

## Major Changes

- **Record special purchase prices and discounts**

  Overhauled purchase pricing guidance to align with the new pricing experience and clarified when to enter lines for each special purchase price. Clarified vendor selection rules (pay-to vs. buy-from) across current and new experiences and noted that invoice discounts use the pay-to vendor. Refined best-price logic for purchases, including date usage (Posting Date vs. Order Date) and the absence of vendor price/discount groups on purchases. Updated fallback behavior to use SKU or item last direct cost when no special purchase price applies.

  https://learn.microsoft.com/en-us/dynamics365/business-central/purchasing-how-record-purchase-price-discount-payment-agreements

- **Synchronize items with Shopify**

  Retitled and expanded the article to cover syncing items, products, images, and variants. Moved pricing and inventory content into dedicated articles to simplify navigation and reduce duplication, and added guidance to choose a system of record before setup. Updated field descriptions and related links to point to the new pricing and inventory pages and streamlined metadata to improve discoverability.

  https://learn.microsoft.com/en-us/dynamics365/business-central/shopify/synchronize-items

- **Synchronize and fulfill sales orders**

  Added detailed tax guidance for imported Shopify orders, including multi-rate VAT handling, country-specific settings, and behavior for “Prices including VAT.” Introduced instructions for Marketplace Facilitator (Channel Liable) taxes effective Jan 1, 2025, with tracking fields, import filtering, and review steps. Expanded warehouse mapping guidance for locations with Directed Put-away and Pick, recommending settings that preserve proper warehouse flows.

  https://learn.microsoft.com/en-us/dynamics365/business-central/shopify/synchronize-orders

## Moderate Changes

- **Australia local functionality**

  Updated the roadmap of investigated legislation by removing Payment Times Reporting Bill Compliance for 2026 wave 1 and moving the TPAR timeline to 2027 wave 1. This sets clearer expectations for customers planning compliance projects.

  https://learn.microsoft.com/en-us/dynamics365/business-central/LocalFunctionality/Australia/australia-local-functionality

- **Germany local functionality**

  Removed the planned February 2026 VAT VIES Declaration Export in XML item from the investigated legislation list, with other items unchanged. This provides a more accurate view of upcoming regulatory priorities.

  https://learn.microsoft.com/en-us/dynamics365/business-central/LocalFunctionality/Germany/germany-local-functionality

- **Get started with the Shopify Connector**

  Split a combined synchronization topic into separate links for items, prices and taxes, and inventory. This improves discoverability and helps readers quickly find the specific guidance they need.

  https://learn.microsoft.com/en-us/dynamics365/business-central/shopify/get-started

- **Record special sales prices and discounts**

  Clarified that sales line pricing and discounts are determined by the Bill-to Customer No. across both current and new pricing experiences. Redirected purchase-related best-price details to a dedicated purchase-focused section for accuracy and ease of reference.

  https://learn.microsoft.com/en-us/dynamics365/business-central/sales-how-record-sales-price-discount-payment-agreements

- **Synchronize customers and companies**

  Added best-practice guidance to decide the system of record for customer data to avoid conflicts and bi-directional issues. Renamed a configuration option from “Auto Create Catalog” to “Auto Create B2B Catalog” to better reflect its purpose.

  https://learn.microsoft.com/en-us/dynamics365/business-central/shopify/synchronize-customers