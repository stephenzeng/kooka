# Microsoft Fabric
**Date created:** 2026-08-05 UTC  
**Tags:** Administration, Analytics, Automation, Monitoring, Other, Programming, Security  

## New Articles

- **Use a function as a Data Activator rule action**

  Introduced a step-by-step guide for invoking a user data function as an action in a Data Activator rule. Explains defining functions with the @udf.function() decorator, mapping JSON parameters to Python types, and passing dynamic values from streaming events. Provides testing guidance, best practices for publishing, performance, error handling, and logging, and links to related documentation.

  https://learn.microsoft.com/en-us/fabric/data-engineering/user-data-functions/activator-action-function

- **Fabric Plan Billing and Pricing Model**

  Launched a concept article outlining Fabric plan’s active-session, capacity-based billing. Defines user roles and 30‑day consumption rates, how sessions are started and billed, and how automation jobs are charged. Covers capacity planning guidance, use of MACC and buffer recommendations, and an extensive FAQ for real-world billing scenarios.

  https://learn.microsoft.com/en-us/fabric/iq/plan/resources/billing-fabric-plan

- **Cube Measures FAQ for Planning and Allocation**

  Added an FAQ clarifying how Cube measures distribute values across dimensions based on a reference measure. Explains multi-breakdown support, behavior when copying or importing measures, and how subtotal edits propagate proportionally. Highlights when to use Insert as measure to retain two-way edit behavior and other key limitations.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-cubes/faq-cube

- **Create a Multi-Dimensional Planning Cube**

  Published a how-to on building multi-dimensional planning cubes for allocation and aggregation across dimensions. Details prerequisites, configuring breakdowns, using reference measures for weighted distribution, and importing measures into other sheets while maintaining bidirectional updates. Includes best practices for driver selection, redistribution behavior, and optional calculated measures.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-cubes/how-to-create-cube

- **Manage Cube Measures and Breakdowns**

  Introduced guidance for managing cube measures, including syncing with the semantic model, viewing logs, and modifying dimension breakdowns. Shows how to insert and sync individual measures, adjust breakdowns in the Model ribbon, and safely delete measures. Describes downstream implications for linked planning sheets to avoid disruption.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-cubes/how-to-manage-cube-measures

- **Measure-Based Modeling in Fabric Plan**

  Added a how-to for creating measure hierarchies and scenario-driven simulations in planning. Covers building from semantic model measures, organizing hierarchies, configuring formulas, and using Tree layout to explore dependencies. Explains scenario creation, cascading impacts across measures and geographies, and provides an FAQ to resolve common modeling questions.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-how-to-create-measure-model

- **Semantic Model Best Practices for Fabric Plan**

  Published comprehensive best practices for dimension-driven modeling in planning scenarios. Recommends replacing scenario-specific measures with a Scenario dimension and using business-configured planning windows, backed by tables like Date, Validity, and Weight Matrix. Provides patterns for editability, managed combinations, and fiscal calendar planning, with a sample PBIX for reference.

  https://learn.microsoft.com/en-us/fabric/iq/plan/resources/best-practices/semantic-modeling

## Major Changes

- **Operations Agent Capacity and Billing**

  Overhauled billing metrics to introduce CU Hours and CU seconds and added cached input token billing across relevant entries. Revised rates for Investigation agent and Operations agent autonomous reasoning, and clarified units for Operations agent compute. These changes affect how workloads are costed and help customers more accurately estimate usage and optimize spend.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/operations-agent-billing

- **What's new? archive**

  Expanded the archive with a broad set of May 2026 updates spanning Data Factory, OneLake, Platform and admin, Data Engineering, Data Warehouse, SQL database in Fabric, Real-Time Intelligence, and Data Science/IQ. The additions include multiple GA announcements and previews such as security roles, storage lifecycle tiers, capacity metrics enhancements, incremental clustering, unified monitoring, and new developer capabilities. This consolidation helps admins and practitioners quickly track feature availability and plan adoption.

  https://learn.microsoft.com/en-us/fabric/fundamentals/whats-new-archive

## Moderate Changes

- **Legacy HTTP Data Collector API path for Azure Log Analytics**

  Standardized terminology to “environment item” and updated setup steps accordingly. Revised Kusto examples to use ItemId_g instead of artifactId_g, aligning queries with current schemas for Spark telemetry.

  https://learn.microsoft.com/en-us/fabric/data-engineering/azure-fabric-diagnostic-emitters-log-analytics

- **Create Tables in the Warehouse**

  Refreshed examples to use a realistic sales fact table and updated CTAS guidance with a new OPENROWSET parquet source. These improvements provide more relevant patterns for production-grade table design.

  https://learn.microsoft.com/en-us/fabric/data-warehouse/create-table

- **Optimize Delta Lake tables with V-order**

  Clarified that Fabric runtime 1.3+ removes spark.sql.parquet.vorder.enable and that V-order should be applied via Delta OPTIMIZE. This helps teams clean up legacy configs and use the supported approach going forward.

  https://learn.microsoft.com/en-us/fabric/data-engineering/delta-optimization-and-v-order

- **Ingest data in the warehouse**

  Updated COPY INTO examples to target dbo.fact_sale and new WideWorldImportersDW paths for Parquet and CSV. The refreshed examples align ingestion patterns with the latest tutorial datasets.

  https://learn.microsoft.com/en-us/fabric/data-warehouse/ingest-data-into-table

- **Migrate SQL Server to SQL Database in Fabric by using the Fabric Migration Assistant**

  Added an optional schema validation step to check the uploaded DACPAC before configuring the destination, with guidance to review the validation summary and fix issues. Subsequent steps were renumbered to reflect the new validation phase, improving migration readiness.

  https://learn.microsoft.com/en-us/fabric/database/sql/migrate-with-migration-assistant-using-dacpac

- **Migrate SQL Server to SQL Database in Microsoft Fabric Using Fabric Migration Assistant**

  Introduced a “Validate schema” step to assess the DACPAC without creating a database, highlighting objects that will migrate, need updates, or won’t migrate. This addition reduces surprises during execution and streamlines remediation.

  https://learn.microsoft.com/en-us/fabric/database/sql/migration-assistant

- **How to create and update a Spark job definition with Microsoft Fabric REST API**

  Replaced deprecated sjdartifactid references with sjditemid in endpoints and ABFSS paths. The update aligns examples with current identifiers to avoid configuration errors.

  https://learn.microsoft.com/en-us/fabric/data-engineering/spark-job-definition-api

- **Service details and limitations of Fabric User Data Functions**

  Documented a 100‑second execution timeout for functions invoked through public endpoints. This helps developers design functions and client calls with appropriate timeouts and retries.

  https://learn.microsoft.com/en-us/fabric/data-engineering/user-data-functions/user-data-functions-service-limits