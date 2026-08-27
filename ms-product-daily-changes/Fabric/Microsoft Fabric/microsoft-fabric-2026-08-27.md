# Microsoft Fabric
**Date created:** 2026-08-27 UTC  
**Tags:** Analytics, Best Practices, Billing, Configuration, Get Started, Governance, Guidance, Monitoring, Performance, Security, Troubleshooting  

## New Articles

- **Activity Retries in Microsoft Fabric Data Factory**

  Introduced detailed guidance for configuring per‑activity retries, including retry count and interval options with fixed or increasing delays, exponential back‑off, and randomized waits. Documents defaults and constraints, clarifies that retry interval values must be static integers, and explains evaluation timing. Adds preview retry conditions to target retries by message, failure type, or error code with AND/OR logic, outlines supported activities, and lists known limitations and related links.

  https://learn.microsoft.com/en-us/fabric/data-factory/activity-retries

- **Common dbt job patterns in Microsoft Fabric (preview)**

  Added conceptual guidance on four dbt architecture patterns across medallion designs, detailing when to use each and how dbt integrates with Fabric components. Covers orchestration choices between dbt scheduling and Fabric pipelines, including dependency handling, parameters, and monitoring. Highlights adapter differences, metadata considerations, OneLake shortcuts, and runtime behaviors.

  https://learn.microsoft.com/en-us/fabric/data-factory/common-dbt-job-patterns

- **Consume a Fabric data agent as a tool in Microsoft Copilot Studio**

  Published a step‑by‑step how‑to for adding a Fabric data agent as a tool in Copilot Studio, including prerequisites and setup on the Copilot Studio harness. Explains connecting the Fabric IQ Data MCP tool, selecting a published agent, providing tool descriptions, and choosing authentication mode with implications. Covers testing, evaluation, publishing to Teams and Microsoft 365 Copilot, and compliance and permissions considerations.

  https://learn.microsoft.com/en-us/fabric/data-science/data-agent-microsoft-copilot-studio-tool

- **Duplicate a query in Infobridge**

  Added instructions to duplicate an existing Infobridge query via the Home tab action. Clarifies that the duplicated query is independent, enabling safe modification without affecting the original, and includes supporting screenshots.

  https://learn.microsoft.com/en-us/fabric/iq/plan/infobridge-transform-queries/how-to-duplicate-query

- **Use Super Filter**

  Introduced the Super Filter visual for Fabric Plan Intelligence Sheet and explained eight filter types that enable cross‑filtered dashboards in a single visual. Provides steps to add and configure the visual, including automatic field‑type detection and overrides in the Format pane. Details advanced capabilities such as cascading filters, KPI variance, saved presets, conditional formatting, and animated playback, with an intro video.

  https://learn.microsoft.com/en-us/fabric/iq/plan/intelligence-how-to-start-with-super-filters

- **Lookup Functions**

  Added a reference for the XLOOKUP function in Plan, describing condition‑based lookups that return a value or array with a fallback. Documents syntax, arguments, output modes, and the THIS keyword for context‑aware comparisons. Includes worked examples, common patterns, and business use cases for analytics and planning.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-reference-formulas/lookup-functions

- **Allocation Rules and Data Input Controls in Plan**

  Published conceptual guidance on planning rules: distribution, min/max constraints, and locking. Explains when to use equal vs. weighted distributions, how constraints validate across hierarchies, and how locking protects finalized data. Describes combining rules for budgeting scenarios to enforce integrity during updates and allocations.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-concept-allocation-rules-controls

- **Export PowerTable Layouts to PDF**

  Added a how‑to for exporting PowerTable layouts (Gantt, Resource, Calendar) to PDF via the ribbon. Explains Standard vs. Grouped export types and configurable options including page size, quality, orientation, grouping, date range, and headers. Notes that other layouts don’t support PDF exports and includes screenshots.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-how-to-export-to-pdf

- **Workspace private links for Azure and Fabric events**

  Introduced guidance for workspace‑level private links and their effect on Real‑Time hub event consumption. Defines source vs. consumer workspaces, summarizes allowed scenarios, and details behavior changes when settings are updated (paused configurations requiring re‑creation). Notes interactions with tenant Block Public Internet Access and links to related topics.

  https://learn.microsoft.com/en-us/fabric/real-time-hub/workspace-private-links-real-time-events

## Major Changes

- **Customize a map**

  Rewrote and expanded the map customization guide with a two‑tier model separating basemap and per‑layer settings. Added detailed properties for styles, initial view, elements, controls (including Traffic and World wrap), localization, and geometry‑specific layer options (polygon, line, point with bubble/marker/heatmap). Expanded data‑driven styling, introduced visibility controls, clarified marker rotation behavior for built‑in icons, and refreshed examples and screenshots.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/map/customize-map

- **IDENTITY Columns in Fabric Data Warehouse**

  Substantially expanded guidance on IDENTITY behavior, metadata, and operations in distributed architecture. Documented support for SET IDENTITY_INSERT with examples and constraints, and reseeding via DBCC CHECKIDENT (RESEED) to avoid collisions. Updated limitations, clarified uniqueness and ordering semantics, and added comprehensive examples across insert patterns and COPY INTO.

  https://learn.microsoft.com/en-us/fabric/data-warehouse/identity

- **Migrate IDENTITY columns to Fabric Data Warehouse**

  Reworked migration guidance to preserve historical identity values using SET IDENTITY_INSERT and post‑load reseeding with DBCC CHECKIDENT. Added examples for INSERT and COPY INTO, verification steps, and best practices to prevent ID overlaps. Clarified platform capabilities (bigint only, no custom seed/increment) and removed the prior staging/remapping approach.

  https://learn.microsoft.com/en-us/fabric/data-warehouse/migrate-identity-columns

- **Migrate SQL Server to SQL Database in Microsoft Fabric Using Fabric Migration Assistant**

  Removed the Preview designation and updated guidance to reflect general availability. Adjusted the workflow to mark schema validation as optional and removed the limitation about Private Link, indicating it’s now supported. This streamlines planning and enables secure private connectivity scenarios.

  https://learn.microsoft.com/en-us/fabric/database/sql/migration-assistant

- **Tenant private links for Azure and Fabric events**

  Refocused content on tenant‑level private links and removed workspace‑level scenarios, examples, and allowlisting steps. Clarified the impact on Azure event flows (Fabric‑originated events unaffected) and updated remediation guidance to disable tenant Block Public Internet Access or remove the Private Link. Added links to workspace private links and paused configuration guidance.

  https://learn.microsoft.com/en-us/fabric/real-time-hub/private-links-real-time-events

- **SQL Analytics Endpoint Performance Considerations**

  Rewrote performance guidance to favor Fabric Spark runtime 2.0+ defaults with adaptive target file sizing and default compaction targets. Provided opt‑in steps for runtime 1.3, clarified V‑Order expectations, and added maintenance best practices (auto compaction, scheduled OPTIMIZE, VACUUM). Updated methods to identify tables needing maintenance via sys.sp_get_table_health_metrics and refined partitioning guidance.

  https://learn.microsoft.com/en-us/fabric/data-engineering/sql-analytics-endpoint-performance

- **Cross-Workload Table Maintenance and Optimization in Microsoft Fabric**

  Restructured and broadened optimization guidance across Lakehouse, Direct Lake, Warehouse, and Mirroring. Introduced a layout ownership model, cross‑workload recommendations, and outcome‑based practices for file sizing, compaction, deletion vectors, and VACUUM. Added sections on organizing data (clustering, partitioning), troubleshooting signals with remediation, and when to create new tables, replacing prescriptive fixed targets.

  https://learn.microsoft.com/en-us/fabric/fundamentals/table-maintenance-optimization

- **How to: Use IDENTITY columns in Fabric Data Warehouse**

  Expanded the tutorial with a new Trip example, PARQUET‑based ingestion, and clearer INSERT patterns. Added guidance for explicit identity inserts with SET IDENTITY_INSERT, sentinel keys, and reseeding with DBCC CHECKIDENT to prevent collisions. Removed preview notes and refined explanations of identity value behavior with verification queries and optional cleanup.

  https://learn.microsoft.com/en-us/fabric/data-warehouse/tutorial-identity

- **What's new in Microsoft Fabric?**

  Consolidated new and updated feature entries, including multiple previews and general availability announcements across apps, data agents, Data Warehouse, and connectivity. Promoted Warehouse IDENTITY columns to GA and updated the catalog to reflect the transition. Updated Migration Assistant status to GA with links from “Recently transitioned” and SQL database updates, while removing outdated preview entries and duplicates.

  https://learn.microsoft.com/en-us/fabric/fundamentals/whats-new

## Moderate Changes

- **Troubleshooting errors in Activator**

  Added guidance to configure recipients for Activator error notifications, including navigation steps and field details. This helps ensure operational alerts reach the right people.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/data-activator/activator-troubleshooting

- **Activity overview**

  Streamlined retry guidance by replacing in‑page details with a link to a dedicated activity retries article. Added a Related content link for quicker discovery.

  https://learn.microsoft.com/en-us/fabric/data-factory/activity-overview

- **AI Functions (Preview)**

  Added a Handling errors section describing default best‑effort behavior that returns NULL on failures and how to inspect/retry affected rows. Introduced the ON ERROR clause with options to return NULL, fail the query, or supply a default, with SQL examples.

  https://learn.microsoft.com/en-us/fabric/data-warehouse/ai-functions

- **Upgrade Dataflow Gen1 to Dataflow Gen2 (CI/CD) using the Upgrade Wizard**

  Clarified that users with Viewer role can see an upgraded Dataflow Gen2 but can’t consume its tables via the Power Platform Dataflows connector. Recommends assigning Contributor, Member, or Admin roles for users who need to consume tables and links to connector limitations.

  https://learn.microsoft.com/en-us/fabric/data-factory/migrate-to-dataflow-gen2-using-upgrade-wizard

- **Migrate SQL Server to SQL Database in Fabric by using the Fabric Migration Assistant**

  Removed Preview references to reflect GA and updated UI text from “SQL Server (Preview)” to “SQL Server.” Corrected screenshot assets for upload and validation steps and updated related links.

  https://learn.microsoft.com/en-us/fabric/database/sql/migrate-with-migration-assistant-using-dacpac

- **Export PowerTable sheet to Excel**

  Clarified what exports include (sheet data, inserted rows, lookup labels) and exclude (visual/formula columns, comments), with a note on exclusions. Updated support to indicate all layouts except crosstab are supported.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-how-to-export-to-excel

- **Query Insights**

  Added a new system view, queryinsights.external_api_call_stats, to expose function‑level diagnostics for queries invoking external APIs via AI functions. Clarified availability across Fabric Data Warehouse and the SQL analytics endpoint and updated related links.

  https://learn.microsoft.com/en-us/fabric/data-warehouse/query-insights

- **T-SQL Surface Area in Fabric Data Warehouse**

  Noted that identity columns are supported in Fabric Data Warehouse within the tables section. This aligns surface area documentation with current capabilities.

  https://learn.microsoft.com/en-us/fabric/data-warehouse/tsql-surface-area

- **Tune the size of Delta table data files**

  Clarified that user‑defined delta.targetFileSize is for legacy compatibility and recommended adaptive target file sizing instead. Noted that adaptive sizing is enabled by default in Runtime 2.0+ (with file‑level compaction targets on by default) and provided guidance for enabling it on Runtime 1.3.

  https://learn.microsoft.com/en-us/fabric/data-engineering/tune-file-size