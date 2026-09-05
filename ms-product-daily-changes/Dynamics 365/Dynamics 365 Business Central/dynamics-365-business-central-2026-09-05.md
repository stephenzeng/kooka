# Dynamics 365 Business Central
**Date created:** 2026-09-05 UTC  
**Tags:** Automation, Best Practices, Billing, Configuration, Guidance  

## New Articles

- **Rebilling usage data**

  Introduced a new article that explains how rebilling corrects previously invoiced usage when new data arrives for the same period. Corrections are billed as separate lines, calculated on their own quantities, and the subscription’s next billing date is temporarily moved back to capture the delta, then restored if the correction is canceled. The article details how to review rebilling status from Usage Data Billings, subscription line Service Commitments, and customer/vendor subscription contracts, including visibility of Rebilling and Invoiced columns. This guidance helps ensure accurate, auditable billing adjustments without mixing them with regular charges.

  https://learn.microsoft.com/en-us/dynamics365/business-central/UBB/processing-usage-data/rebilling

## Major Changes

- **Manage product variants**

  Expanded guidance highlights managing multiple product combinations under one item while controlling details at the variant level. Added instructions for mapping customer/vendor item numbers and units of measure to specific variants, enabling precise transactions and reporting. Introduced variant-aware item translations and clarified how language-specific descriptions flow into documents. Detailed how stockkeeping units connect item, location, and variant to enable targeted replenishment and planning, with examples and related links for deeper setup guidance.

  https://learn.microsoft.com/en-us/dynamics365/business-central/inventory-item-variants

## Moderate Changes

- **Run tasks in the background and recurrently**

  Clarified how to schedule targeted Shopify jobs, including using Only Sync Prices on report 30108 to update prices without syncing products. Documented options on report 30102 to limit exports to specific Shopify variant IDs or skip inventory import before export, with references for focused price and inventory syncs to reduce unnecessary processing.

  https://learn.microsoft.com/en-us/dynamics365/business-central/shopify/background

- **Link supplier subscriptions with subscriptions**

  Added guidance that shipping a usage-based subscription item in advance requires linking to a supplier subscription to fully process usage data. Explained Usage Data Generic Import statuses (Not Available, Available, Connected) to indicate readiness and next steps, helping teams complete connections and proceed to invoicing with confidence.

  https://learn.microsoft.com/en-us/dynamics365/business-central/UBB/processing-usage-data/connect-subscription-service-object

- **Subscription contract types**

  Introduced settings to control currency handling for usage data: automatically convert amounts to the contract currency or block imports when currencies differ. This reduces reconciliation errors and enforces consistent billing based on contract rules.

  https://learn.microsoft.com/en-us/dynamics365/business-central/SRB/setup/contract-types

- **Data exchange definitions**

  Strengthened guidance to align field mappings with minimum data requirements and clarified Overwrite Value behavior. Recommended enabling Overwrite for key fields (for example, Customer Name, Subscription ID, Product/Name, Quantity) so imported values take precedence, improving data accuracy in downstream processing.

  https://learn.microsoft.com/en-us/dynamics365/business-central/UBB/masterdata/dataexchangedefinitions

- **Import data in usage-based billing**

  Added minimum data requirements, explained that records missing required fields or unresolved subscriptions aren’t processed, and pointed to error lookups for review. Clarified how currency differences are handled or rejected based on contract settings, with links to contract types and rebilling for related scenarios.

  https://learn.microsoft.com/en-us/dynamics365/business-central/UBB/processing-usage-data/imports-processing

- **Block items or item variants from use in sales, purchasing, service, and production**

  Clarified that Purchasing Blocked items/variants can still appear in planning suggestions, but executing the resulting action messages fails. Provided steps to stop such suggestions by adjusting or removing SKU reordering policies, avoiding noise in planning.

  https://learn.microsoft.com/en-us/dynamics365/business-central/inventory-how-block-items

- **Create a demand forecast**

  Reworked the introduction to focus on planning objectives and outcomes, such as handling seasonality, long lead times, and capacity balancing for better order promising. Clarified how MPS nets sales and production orders against the forecast and refined Forecast Type behavior to specify which demands are considered.

  https://learn.microsoft.com/en-us/dynamics365/business-central/production-how-to-create-a-forecast

- **Replan or refresh production orders directly**

  Expanded instructions for using Refresh when adding lines manually, including leaving Source Type/No. blank and enabling only Routings and Component Need to avoid overwriting manual lines. Clarified Calculate options behavior and how routings/BOMs are chosen (SKU vs. item card), and explained creating warehouse inbound requests independently of line/component calculations.

  https://learn.microsoft.com/en-us/dynamics365/business-central/production-how-to-replan-refresh-production-orders

- **Planning**

  Updated the introduction to emphasize end-to-end supply planning that balances independent and dependent demand across all item types. Added explicit guidance on running MPS and MRP from the Planning Worksheet to generate suggested supply orders.

  https://learn.microsoft.com/en-us/dynamics365/business-central/production-planning

- **Usage data supplier references**

  Clarified that product references are matched at the item level, not by item variant, because suppliers publish separate items for different plans or tiers. This helps teams avoid relying on variants when matching or creating subscription lines from usage data.

  https://learn.microsoft.com/en-us/dynamics365/business-central/UBB/masterdata/references

- **Synchronize inventory with Shopify**

  Added targeted inventory sync using Sync Stock to Shopify, including Variant ID filtering and the option to skip importing stock before export. Included guidance to periodically run full syncs to refresh quantities and maintain local records, and reorganized supporting explanations for clarity.

  https://learn.microsoft.com/en-us/dynamics365/business-central/shopify/synchronize-inventory

- **Overview of subscription billing**

  Added a new section describing usage-based billing: importing supplier usage data, automated processing, and price calculation. Included a related link to the overview of usage-based billing to guide readers to deeper processes.

  https://learn.microsoft.com/en-us/dynamics365/business-central/SRB/welcome