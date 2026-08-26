# Microsoft Fabric
**Date created:** 2026-08-26 UTC  
**Tags:** Analytics, Configuration, Guidance, Monitoring  

## New Articles

- **Use the dynamic expression editor for Dataflow Gen2 data destinations**

  Introduced a how-to guide for the dynamic expression editor (preview) to build parameterized table and file names using UTC date/time, parameters, and workspace variables. Explains keyboard-driven insertion via the '/' menu, shows example expressions, and clarifies how values resolve at runtime. Provides steps to enable or disable the editor in Options and outlines limitations, including availability by destination/field and that it’s not a general M editor. Helps teams standardize naming patterns and reduce manual errors across runs.

  https://learn.microsoft.com/en-us/fabric/data-factory/dataflow-gen2-dynamic-expression-editor-data-destinations

- **Row Model Forecasts for Driver-Based Planning**

  Added step-by-step guidance to create driver-based forecasts in a row model, including prerequisites and a walkthrough for building a 2026 forecast. Shows how to lock closed periods to Actuals, open periods for input, and pre-fill values from prior Actuals with period mapping. Demonstrates how changing driver inputs (such as Revenue or Purchase expense) cascades through calculated rows and impacts KPIs like Profit. Enables faster, consistent planning cycles with clear links to related forecasting and scenario analysis topics.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-row-model/how-to-create-row-model-forecasts

- **Scenario Analysis with Tree Layout in Row Model**

  Introduces scenario analysis using the tree layout to compare Best, Worst, and Balanced cases against a baseline. Details prerequisites, enabling the layout, selecting time periods, and adjusting key drivers to observe cascading impacts. Provides techniques to analyze results in graph/table views, compare scenarios for variance insights, and copy a selected simulation back to the base scenario. Helps planners rapidly test assumptions and communicate trade-offs.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-row-model/how-to-create-row-model-scenarios

- **Manage sources**

  Provides a how-to on managing Infobridge sources, including viewing source details, ownership, queries, measures, and update actions. Explains how to manually refresh a source and review refresh history with filters and key columns like Execution ID, timing, duration, and status. Includes screenshots to help administrators quickly navigate and troubleshoot source refreshes. Improves operational visibility and control over data pipelines.

  https://learn.microsoft.com/en-us/fabric/iq/plan/infobridge-how-to-manage-sources

- **Time Intelligence Functions: Period-to-Date Calculations**

  Documents Plan functions for MTD, QTD, and YTD with optional offsets, plus cumulative TOTALMTD, TOTALQTD, and TOTALYTD variants. Provides syntax, arguments, return behavior, and examples that pair with aggregations like SUM to compute period-to-date and cumulative values. Offers visual examples to accelerate adoption and reduce errors in financial and operational reporting. Helps standardize time-intelligence calculations across models.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-reference-formulas/time-intelligence-functions/period-to-date-calculations

- **Time Intelligence Functions: Relative Time Periods**

  Adds reference material for LASTN and NEXTN functions across days, months, quarters, and years to analyze historical and future ranges. Shows how to combine these functions with SELECT.BYDATE and aggregations (e.g., SUM, AVERAGE) to retrieve and summarize dynamic windows. Includes examples and visuals to guide correct usage and improve time-based insights in planning scenarios. Enables repeatable, parameter-driven analysis across rolling horizons.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-reference-formulas/time-intelligence-functions/relative-time-periods

- **Time Intelligence Functions: Specific Time Periods**

  Introduces MONTHPERIOD, QTRPERIOD, and YEARPERIOD to select exact periods or ranges for targeted analysis. Explains syntax, arguments, and returns, with examples combining SELECT.BYDATE and aggregations for robust summaries. Provides illustrative outputs to speed implementation and reduce logic mistakes. Supports consistent period selection for month, quarter, and year reporting.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-reference-formulas/time-intelligence-functions/specific-time-periods

- **Time Intelligence Functions: Time-Based Aggregations**

  Documents AGGREGATE, MOVINGSUM, and MOVINGAVERAGE for rolling and windowed analyses across time. Covers syntax, arguments, and examples using date ranges, COLUMN.CURRENT_PERIOD with SHIFT, and forecast OPEN_START/OPEN_END fields. Visuals show practical patterns for moving calculations, enabling clearer trend and volatility analysis. Helps practitioners standardize advanced time-based metrics.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-reference-formulas/time-intelligence-functions/time-based-aggregations

## Moderate Changes

- **Dataflow Gen2 data destinations and managed settings**

  Updated parameterization guidance to highlight the new dynamic expression editor, with examples for combining text, dates/times, parameters, and workspace variables, and the '/' shortcut for quick insertion. Streamlined content by removing outdated UI screenshots, linking to advanced editor guidance, and clarifying that unsupported destination settings can still be parameterized using M script.

  https://learn.microsoft.com/en-us/fabric/data-factory/dataflow-gen2-data-destinations-and-managed-settings