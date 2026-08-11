# Dynamics 365 Supply Chain Management
**Date created:** 2026-07-24 UTC  
**Tags:** Administration, Automation, Other, Security  

## New Articles

- **Import inbound ASNs as despatch advice messages**

  Introduced documentation for importing inbound ASNs as despatch advice messages using a message processor that supports dependencies and full-document updates. Describes message structure (header, logistic units, and line items), identifiers, and how nested logistic units are represented using flat lists. Provides multiple import methods—Data management (XML), OData with Complete action, and Dataverse—plus examples. Explains replace-by-new-message update behavior, scheduled processing, monitoring via message processor logs and business events, and how to verify loads and packing structures.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/warehousing/despatch-advice-notice

- **Prevent multiple owners in warehouse locations**

  Introduced the “Prevent multiple owners” location constraint to enforce single-owner storage and avoid cross‑mingling. Provides prerequisites, setup steps for location profiles, and guidance for enabling and using the Owner tracking dimension across common scenarios. Details how the rule is enforced during putaway, manual moves, and replenishment, and includes troubleshooting tips, FAQs, and compatibility guidance with other mixing constraints.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/warehousing/prevent-multiple-owners-locations

- **Reserve the same batch for a production order (preview)**

  Added guidance for “Same batch selection” to keep batch traceability by reserving an entire quantity from a single batch in production and batch orders. Covers prerequisites, configuration via item model group, FEFO-based selection, and behavior when no single batch can fulfill the requirement. Explains conflict handling for manual reservations and the non‑WMS “Batch reservation policy for non‑advanced warehouses” with simple versus advanced behavior.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/production-control/reserve-same-batch-production-order

- **What's new or changed in Dynamics 365 Supply Chain Management 10.0.49 (September 2026)**

  Published the 10.0.49 release notes with schedule, build details, and consolidated feature tables across Master planning, Procurement and sourcing, Production control, and Warehouse management. Highlights enhancements, features moving to general availability, features turned on by default or becoming mandatory, and items removed from Feature management. Includes links to related platform and app updates and deprecations for deeper planning.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/get-started/whats-new-scm-10-0-49

## Major Changes

- **Master planning with demand forecasts**

  Added detailed guidance on reducing demand forecasts when customer or customer group, required BOM, and required route are specified on forecast lines. Documents prerequisites (10.0.49+ and feature flag), the matching principle, and specificity rules, with examples to illustrate behavior and interactions with delivered/invoiced orders. This helps planners avoid double‑counting and align forecasts to actual configured demand.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/master-planning/planning-optimization/demand-forecast

- **Master planning with supply forecasts**

  Introduced consideration of sub‑BOM and sub‑route in supply forecast reduction with clear matching principles and specificity rules. Includes examples and a summary of matching outcomes, plus notes on how the same rules apply to demand forecasts with additional dimensions. This improves forecast accuracy and prevents overstated supply when variant‑specific structures apply.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/master-planning/planning-optimization/supply-forecast

- **Exchange data between systems**

  Added a comprehensive section for Warehouse management only mode to map source system inventory statuses when using external shared warehouses. Explains prerequisites, setup via Source system inventory statuses, bulk import using a data entity, and how mappings apply across inbound and outbound requests and updates. Notes entity exposure for reporting and integration, enabling consistent status handling across systems.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/warehousing/wms-only-mode-exchange-data

## Moderate Changes

- **Advanced quality management overview**

  Clarified that as of version 10.0.49, both Dispense management and Advanced quality management are mandatory and cannot be turned off. This sets clear expectations for environments upgrading to or deploying 10.0.49+.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/inventory/advanced-quality-management-overview

- **Approved customer lists**

  Updated prerequisites to indicate Advanced quality management is mandatory starting in version 10.0.49. This ensures prerequisite alignment for organizations using approved customer lists.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/sales-marketing/approved-customer-lists

- **Manage test instrument calibration with Asset Management (preview)**

  Clarified that Advanced quality management is on by default from 10.0.47 and mandatory from 10.0.49. Removed the preview label from “Optional linking of test instruments to maintainable assets,” signaling general availability.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/asset-management/preventive-and-reactive-maintenance/asset-management-test-instrument-calibration

- **CAPA management administration**

  Updated requirements to state that Advanced quality management becomes mandatory in version 10.0.49. This helps admins plan for consistent quality process enablement.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/inventory/capa-admin

- **Coverage time fences**

  Added guidance for “Filter derived requirements by coverage time fence with Planning Optimization,” available from 10.0.49. When enabled, derived requirements respect the same coverage time fence logic as sales orders, improving planning precision across related requirements.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/master-planning/planning-optimization/coverage-time-fence

- **Dispatch work orders**

  Removed the section describing prerequisites for the Update forecasts feature to reflect current default/mandatory behavior. Core dispatch steps remain unchanged, simplifying setup guidance.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/asset-management/work-order-scheduling/dispatch-work-order

- **Dynamic work classification**

  Removed preview status and updated the title; noted the feature is turned on by default starting in version 10.0.49. This clarifies enablement for warehouse operations.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/warehousing/dynamic-work-classification

- **Use external item identifiers to add products to orders**

  Added a note that “Enable lookup based search for Sales External Item Identifier field” is mandatory in version 10.0.49. This ensures consistent product lookup behavior across sales processes.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/sales-marketing/external-item-product-search-lookup

- **Enable Inventory Visibility for Commerce**

  Updated feature status to indicate “Enable warehouse items in Inventory Visibility” is mandatory in 10.0.49 (still on by default from 10.0.45). This solidifies WHS item support when using Inventory Visibility.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/inventory/inventory-visibility-commerce-enable

- **Inventory Visibility reservations**

  Clarified that “Inventory Visibility integration with reservation offset” is mandatory starting in 10.0.49. This standardizes reservation offset behavior across environments.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/inventory/inventory-visibility-reservations

- **Track time-series inventory in Inventory Visibility**

  Updated prerequisites to state “Inventory Visibility integration with ATP” is mandatory starting with 10.0.49 (on by default from 10.0.45). This ensures consistent time-series ATP calculations.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/inventory/inventory-visibility-track-atp

- **Inventory Visibility support for WMS items**

  Noted that “Enable warehouse items in Inventory Visibility” becomes mandatory in 10.0.49. This aligns setup steps with enforced feature behavior.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/inventory/inventory-visibility-whs-support

- **Material availability check for work orders**

  Updated prerequisites to reflect that “Aggregated material availability check” is on by default from 10.0.47 and mandatory from 10.0.49. This helps organizations plan consistent material readiness checks.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/asset-management/work-orders/material-availability-check-work-orders

- **Optimize confirmed dates for CTP line changes**

  Promoted the feature to general availability by removing preview labels and notes. No changes to procedures or scenarios were made.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/master-planning/planning-optimization/optimize-confirmed-dates-for-ctp-line-changes

- **Purchase requisition overview**

  Added a configuration option that controls whether fixed asset fields on purchase requisitions are reevaluated based on accepted RFQ bids (Yes) or only the price is transferred (No). Available in version 10.0.49+, this provides tighter control over accounting and budget reservations during RFQ-driven procurement.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/procurement/purchase-requisitions-overview

- **Quality associations**

  Updated requirements to state Advanced quality management is mandatory from 10.0.49. This clarifies baseline quality configuration for triggered checks.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/inventory/quality-associations

- **Diagnostic types for nonconformances**

  Noted that Advanced quality management is on by default from 10.0.47 and mandatory starting in 10.0.49. This standardizes diagnostic group usage across environments.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/inventory/quality-diagnostic-types

- **Nonconformance work groups**

  Clarified that Advanced quality management is mandatory from 10.0.49. This ensures consistent governance for nonconformance handling.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/inventory/quality-nonconformance-workgroup

- **Nonconformance root cause codes**

  Updated requirements to indicate Advanced quality management is mandatory from 10.0.49. This aligns root cause management with core quality features.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/inventory/quality-root-cause-codes

- **Enable and configure sample management**

  Clarified that Advanced quality management becomes mandatory in 10.0.49 and Sample management is turned on by default in 10.0.49. This streamlines sampling configurations for quality processes.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/inventory/quality-sample-management-admin

- **Quality management test instruments**

  Updated requirements to note Advanced quality management is mandatory from 10.0.49. This establishes a consistent baseline for test instrument management.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/inventory/quality-test-instruments

- **Rebate management posting setup**

  Clarified that “Enable posting of vendor rebate outputs to purchase order vendors” is mandatory from 10.0.49 (previously on by default from 10.0.45). This cements posting behavior for vendor rebate settlements.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/rebate-management/rebate-management-posting

- **Safety margins**

  Promoted “Soft issue margin” to general availability by removing preview labels and notes. The functional guidance remains unchanged.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/master-planning/planning-optimization/safety-margins

- **Calendars and master planning**

  Added a section showing how “Closed for pickup” on the transport calendar is considered when the related Planning Optimization feature is enabled, requiring pickup windows to be open on both issuing warehouse and transport calendars. Also clarified that the receiving warehouse calendar takes precedence over the coverage group calendar for receipt dates when the feature is on.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/master-planning/supply-chain-calendars-master-planning

- **What's new or changed in Dynamics 365 Supply Chain Management 10.0.46 (December 2025)**

  Removed the preview label for “Optional linking of test instruments to maintainable assets” and deleted the “Dynamic work classification” preview entry. This aligns the page with features’ current availability status.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/get-started/whats-new-scm-10-0-46

- **What's new or changed in Dynamics 365 Supply Chain Management 10.0.47 (March 2026)**

  Removed two feature entries (Configure quality associations by product dimensions; Dynamic work classification using Power FX formulas). No other substantive changes were made.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/get-started/whats-new-scm-10-0-47

- **What's new or changed in Dynamics 365 Supply Chain Management 10.0.48 (June 2026)**

  Updated statuses to indicate GA for several Master planning features and aligned Feature management descriptions by removing preview qualifiers. Warehouse management retains production‑ready preview status in Feature management while removing preview notation from descriptive text.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/get-started/whats-new-scm-10-0-48

- **Enable and configure Warehouse management only mode**

  Added optional setup for mapping source system inventory statuses and guidance for using the Owner dimension, including required owner mappings (including empty values). Introduced guidance to prevent multiple owners in locations, with references for detailed configuration.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/warehousing/wms-only-mode-setup

- **Work order lifecycle states**

  Removed the section describing prerequisites for role‑based access control on lifecycle stages. Core configuration and usage guidance remain unchanged.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/asset-management/setup-for-work-orders/work-order-lifecycle-states