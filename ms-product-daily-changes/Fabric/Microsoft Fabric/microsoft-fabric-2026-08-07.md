# Microsoft Fabric
**Change date:** 2026-08-07 UTC  
**Tags:** Administration, AI, Agent, Analytics, Automation, Governance, Monitoring, Programming, Security  

## New Articles

- **Understand Dataflow Gen2 detailed refresh logs**

  Introduced a comprehensive guide to downloading and analyzing Dataflow Gen2 detailed refresh logs, including cautions about sensitive information. Clarifies ZIP archive structure, file naming, handling of parallel engine instances, and the JSON Lines format used for entries. Provides a practical workflow to aggregate, parse, sort, and correlate log records to troubleshoot refresh issues and links to related monitoring and refresh documentation.

  https://learn.microsoft.com/en-us/fabric/data-factory/dataflow-gen2-detailed-refresh-logs

- **Insert Multi-select Relationship Columns in PowerTable Sheet**

  Added guidance to configure multi-select relationship columns for many-to-many lookups, including prerequisites for master/lookup/relation tables and key fields. Explains how to map lookup and relation columns, set defaults, and persist selections that update the relation table. Covers entering values, adding new lookup records directly from the sheet, and an FAQ on value storage, self-referencing, hierarchical display, and dependent filtering.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-how-to-insert-columns/how-to-insert-multi-select-columns

- **Insert Relation Columns in PowerTable Sheet**

  Introduced instructions for creating relation columns that link master and detail tables. Details setup steps for selecting related tables and keys, configuring display labels and optional lookups, adding filters, enabling cascade delete, and adjusting display properties. Shows how to expand parent rows to view and work with related child records for common actions like insert, filter, sort, and search.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-how-to-insert-columns/how-to-insert-relation-columns

- **Insert Rollup Columns in PowerTable Sheet**

  Added a how-to for rollup columns to compute aggregates such as sums, counts, averages, min/max, and latest/earliest dates across related records. Walks through selecting the linking schema, matching keys, target column, and aggregation function, with optional filter conditions. Includes examples for summing order quantities and calculating the latest order date, plus notes on blank outputs when no related data exists.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-how-to-insert-columns/how-to-insert-rollup-columns

- **Row Model Concept for Driver-based Planning**

  Introduced the row model as an agile driver framework where a single row hierarchy turns each row into a planning driver. Explains how formulas and aggregations work across versions and KPIs and contrasts the approach with traditional spreadsheets. Outlines when to use the model, key benefits like rapid deployment and centralized logic, and common FP&A and operational planning use cases.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-row-model/planning-concept-row-model

- **Create a Model by Using Model Builder**

  Added a step-by-step guide to build a P&L planning model using Model Builder. Covers creating parent/child/sibling rows, defining row types (Data Source, Data Input, Aggregate, Formula), and writing formulas for key metrics like Net Profit and Income Before Tax. Highlights Bulk Insert and Bulk Edit for faster structure and formatting, aggregation settings for period rollups, Open Period configuration, and a complete example hierarchy.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-row-model/planning-how-to-create-model-using-model-builder

- **Skills for SQL database in Fabric**

  Introduced skills bundles to work with Fabric SQL databases via developer tools such as GitHub Copilot CLI and Claude Code. Details installation and verification steps and documents three skills for authoring schema/data changes, read-only exploration and queries, and operational diagnostics. Provides a safety checklist for reviewing and executing T-SQL and outlines security and responsible use practices.

  https://learn.microsoft.com/en-us/fabric/database/sql/skills

- **Tutorial: Orchestrate Fabric jobs with Job events**

  Added an end-to-end tutorial for event-driven orchestration using Job events in Real-Time hub. Demonstrates chaining a pipeline and a Dataflow Gen2 with a job-succeeded alert, then validating runs and outputs. Covers advanced scenarios including fan-out, cross-item chaining, failure handling with job-failed events, and auditing with eventstreams and eventhouse.

  https://learn.microsoft.com/en-us/fabric/real-time-hub/tutorial-orchestrate-jobs-with-job-events

## Moderate Changes

- **Anonymous data access in Fabric apps**

  Updated configuration guidance by removing the step to set services.data.anonymousAccess in rayfin.yml and revised governance recommendations. Clarified tenant-level controls so admins can disable anonymous access across all apps or restrict access to selected security groups. These changes streamline setup and reinforce centralized access management.

  https://learn.microsoft.com/en-us/fabric/apps/anonymous-data-access

- **View Dataflow Gen2 refresh history and monitoring**

  Expanded instructions for downloading and using detailed refresh logs, including availability timing, 28-day retention, and the required minimum Viewer role. Added a reference to a dedicated article that explains archive structure and interpreting JSON Lines records, improving troubleshooting and analysis.

  https://learn.microsoft.com/en-us/fabric/data-factory/dataflows-gen2-monitor

- **Explore, organize, and summarize data in PowerTable**

  Added a new section on Sort By with step-by-step guidance for multi-column sorting, choosing order, and reordering priority via drag-and-drop. Users can now persist sort configurations, improving repeatability for analysis workflows.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-how-to-explore-organize-data