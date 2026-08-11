# Dynamics 365 Customer Insights
**Date created:** 2026-08-11 UTC  
**Tags:** Configuration, Guidance, Security, Troubleshooting  

## New Articles

- **Transform dynamic text with Power Fx formulas**

  Introduced new guidance for applying Power Fx formulas to dynamic text in the email editor, including how to enable formula mode and reference the dynamic text display name as the variable. Provides practical examples for case conversion, handling empty values with Coalesce, and locale-aware number/date formatting using Text with format strings. Explains execution behavior (runs at send time, operates on a single dynamic value, and sends even if a formula fails by reverting to the original/default). Details limits and scope, including supported single-value functions only, no table/record/custom functions, and constraints on expression length and nesting, plus a reference pane with examples.

  https://learn.microsoft.com/en-us/dynamics365/customer-insights/journeys/power-fx-dynamic-text

## Major Changes

- **Connect to Microsoft Fabric OneLake**

  Removed preview status and reorganized the article with clear Supported capabilities and Limitations sections to improve discoverability. Added configuration guidance for enabling Private Link when Fabric inbound access protection is enabled, plus cross-references for setup. Enabled editing of Fabric OneLake data sources to add or remove tables, clarified what can’t be changed, and refined prerequisites, primary key detection, and connect/select steps. Centralized schema change guidance and updated Delta logs recommendations, including retention practices and using full refresh when versions are missing. Expanded troubleshooting for scenarios where inbound access protection blocks table listing and consolidated unsupported items (for example, non-Delta formats and Fabric Data Warehouse), while confirming one data source per workspace and noting an upcoming in-place upgrade path.

  https://learn.microsoft.com/en-us/dynamics365/customer-insights/data/connect-fabric-onelake