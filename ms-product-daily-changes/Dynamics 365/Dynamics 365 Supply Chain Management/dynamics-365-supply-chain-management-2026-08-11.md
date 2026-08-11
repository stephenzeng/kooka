# Dynamics 365 Supply Chain Management
**Date created:** 2026-08-11 UTC  
**Tags:** Analytics, Configuration, Guidance, Monitoring, Performance  

## Major Changes

- **Monitor Warehouse Management usage and performance**

  Added preview telemetry that breaks down end-to-end time in the Warehouse Management mobile app (v4.1.5.0+), including active vs. idle time and time spent waiting on the server or completing pages. Expanded insights cover completed vs. abandoned operations, counts of pages and requests, button and dialog usage, errors, and data entry methods (for example, camera vs. scanner). Guidance shows how to correlate device and server telemetry via shared session IDs and includes KQL field references to accelerate analysis. This helps teams pinpoint bottlenecks and improve user flows and performance.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/warehousing/application-insights-monitor-usage-performance

- **Maintenance checklists**

  Introduced template-based checklist line management so you can add lines from one or more templates directly into a work order maintenance job checklist. Clarified that template-referenced lines can’t be deleted (use N/A to exclude) and that the system confirms how many lines were added. The update also refines steps for filling and manually adding lines, improving consistency and reducing manual effort.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/asset-management/work-orders/maintenance-checklists

- **Review impact of purchase order changes from vendors (production-ready preview)**

  Removed the section that described setting up sources to automatically trigger impact analysis. This eliminates outdated or redundant steps and helps keep setup guidance focused and accurate. All other content remains unchanged.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/procurement/procurement-agent-impact-analysis-review-changes

## Moderate Changes

- **Design forecast models**

  Added new options and guidance for filling missing signal values, including Zeros, Forward fill, Backward fill, and Linear interpolation, with examples and rules for when each applies (including version-based availability). Refined the “Forecast with signals” guidance to reference the dedicated article and clarified that XGBoost is used.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/demand-planning/design-forecast-models

- **Set up impact analysis (production-ready preview)**

  Added an important note directing users to an alternative setup wizard and expanded steps for Supplier communications to include creating an impact analysis configuration with Source set to Vendor emails. Introduced configuration steps for changes received via the Vendor Collaboration module, allowing selection of one or both sources and activation to automate impact analysis.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/procurement/procurement-agent-impact-analysis-setup

- **Use the agent deployment wizard to set up impact analysis features (preview)**

  Expanded the wizard instructions to configure sources that automatically trigger impact analysis from vendor emails and the vendor collaboration module, including selecting the appropriate tile, choosing sources, and activating. Clarified prerequisites (version 10.0.48 or higher, with newest build recommended) and refined wording to make the setup process clearer.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/procurement/procurement-agent-impact-analysis-setup-wizard

- **Review and apply purchase order changes received in vendor emails (production-ready preview)**

  Updated navigation paths and labels to match current workspaces and menus, including Agents > Agents and the full path for the Purchase order receipt and follow-up workspace. This keeps the steps aligned with the latest UI terminology.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/procurement/procurement-agent-supplier-com-apply-email-changes

- **Transform data**

  Clarified Time Bucket behavior and added new Precision and Aggregation Method settings in transformation profiles. Introduced a detailed “Aggregation methods” section with examples for Sum (default), Minimum, Maximum, Average, First, Last, and Count to ensure consistent and predictable rollups.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/demand-planning/transform-data