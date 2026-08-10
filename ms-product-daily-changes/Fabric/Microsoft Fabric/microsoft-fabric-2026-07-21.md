# Microsoft Fabric
**Date created:** 2026-07-21 UTC  
**Tags:** Administration, AI, Analytics, Governance, Programming  

## New Articles

- **Tutorial: Connect a Fabric dbt job to Azure HorizonDB (preview)**

  Introduced a step-by-step tutorial to deploy Azure HorizonDB (PostgreSQL-compatible) and connect it to a Fabric dbt job using the PostgreSQL adapter. Covers prerequisites, creating the HorizonDB resource in the Azure portal, configuring the dbt profile, and setting up the connection with required credentials. Includes cleanup steps and links to related dbt job overview, creation, and configuration articles to streamline end-to-end setup.

  https://learn.microsoft.com/en-us/fabric/data-factory/dbt-connect-azure-horizondb

- **Forecasting FAQ: Common Questions Answered**

  Published a comprehensive FAQ explaining how forecasting works in Fabric, including open vs. closed periods, managing multiple forecast measures, and deletion behaviors. Details statistical prerequisites, confidence intervals, growth factors, and model choices (MSTL, Exponential Smoothing, ARIMA) with guidance on seasonality and evaluation approaches. Explains preview behavior, re-running predictions, targeting subsets, handling closed periods, extending horizons, and best practices for reforecasting versus direct edits. Highlights operational specifics such as positional period mapping, proportional growth, and writing finalized forecasts to a Fabric SQL database to operationalize results.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-forecasting/forecasting-faq

- **Fabric Plan (preview) Frequently Asked Questions**

  Added an FAQ for Plan (preview) covering permissions, connection types, and troubleshooting model visibility, clarifying how semantic model and SQL database connections differ and can be reused. Explains recommended sequencing for creating the SQL database and plan app, plus guidance on sheet design, filters, and navigating large sheets. Details export options (PDF, Excel modes, CSV) and what actions persist versus remain temporary in reading mode, including data entry, allocations, forecasts, comments, and writeback, helping teams adopt Plan reliably.

  https://learn.microsoft.com/en-us/fabric/iq/plan/resources/frequently-asked-questions

- **IBCS Waterfall Charts for Financial Analysis**

  Introduced a practical how-to guide for configuring IBCS waterfall charts across C05, C06, and C12 variants. Provides configuration steps for categories, actuals, and comparison measures, along with advanced settings like native axis sorting, result bars, inverting expense bars, and category sign indicators. Equips finance and BI teams to produce consistent, standards-based visuals for variance and progression analysis.

  https://learn.microsoft.com/en-us/fabric/iq/plan/intelligence-ibcs/how-to-configure-ibcs-waterfall-charts

- **Writeback FAQ**

  Released an FAQ explaining writeback in Plan (preview), including persistence behavior across sessions, RLS-respecting writes, and sequential writeback modes (overwrite vs. changes only). Details supported formats (Long, Wide, and hybrid with Changes), multi-destination writes to Fabric SQL databases, column selection, and duplicate prevention logic, noting that writes are additive. Covers security via a dedicated Writeback layer, auditing/logging fields, failure handling, and troubleshooting guidance, so administrators can govern and monitor writeback reliably.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-writeback/writeback-faq

## Moderate Changes

- **Consumption rates and billing for Copilot in Fabric**

  Clarified prompt caching for Copilot and AI features, noting that shared prompt components (system instructions, schema context, conversation history) are automatically cached and billed at a reduced rate without configuration. Updated the consumption table to add a cached input prompt rate of 10 CU seconds per 1,000 tokens, improving cost estimation and transparency for AI workloads.

  https://learn.microsoft.com/en-us/fabric/fundamentals/copilot-fabric-consumption

- **Overview of Materialized Lake Views**

  Updated regional availability by removing a note that excluded South Central US, indicating expanded access. Customers in that region can now plan deployments without prior regional limitations.

  https://learn.microsoft.com/en-us/fabric/data-engineering/materialized-lake-views/overview-materialized-lake-view

- **Analyze planning outcomes with scenarios**

  Added an FAQ clarifying Base as a fixed reference, the independence of scenarios, and how leaf-level adjustments propagate and recalculate dependent and parent measures in real time. Explains limits for calculated measures referencing native measures and confirms you can run multiple scenarios concurrently and adjust or delete them without affecting Base or source data.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-how-to-set-up-scenarios

- **Real-Time Intelligence Tutorial Part 4 - Transform data in a KQL Database**

  Revised the workflow to match the latest Eventhouse UI, replacing ribbon-based steps with navigation through the Databases pane and top navigation bar. The updated guidance clarifies how to create a stored function and configure a table update policy, reducing confusion for users following the current interface.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/tutorial-4-transform-kql-database