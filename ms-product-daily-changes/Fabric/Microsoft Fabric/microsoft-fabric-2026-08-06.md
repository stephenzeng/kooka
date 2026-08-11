# Microsoft Fabric
**Date created:** 2026-08-06 UTC  
**Tags:** Administration, Analytics  

## New Articles

- **Buy Fabric capacity Azure SKUs**

  Introduced a step-by-step guide to purchase Microsoft Fabric capacity using Azure F SKUs in the Azure portal or via a Cloud Solution Provider. Clarifies prerequisites, recommended RBAC permissions, and required actions to create and administer a Fabric Capacity resource. Provides links and guidance for managing, scaling, pausing/resuming capacity, and monitoring costs and metrics.

  https://learn.microsoft.com/en-us/fabric/enterprise/buy-capacity

- **Multidimensional Forecasting with Cube Measures in Fabric Plan**

  Added a how-to for building multidimensional forecast cubes with weighted allocation using reference measures. Explains configuring breakdown dimensions, handling open vs. closed periods, and enabling column subtotals with distribution options. Covers importing forecast cubes into other planning sheets, redistributing values, and using bidirectional updates to keep aggregates and granular edits in sync.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-cubes/how-to-create-forecast-cube

- **Upgrade Dataflow Gen1 to Dataflow Gen2 (CI/CD) using the Upgrade Wizard**

  Published a migration guide for using the Dataflows Upgrade Wizard to move Power BI Dataflows Gen1 to Dataflow Gen2 (CI/CD) in Fabric. Details assessment outcomes, step-by-step upgrade flow, and post-upgrade tasks like refreshing and rebinding downstream items. Outlines known limitations and provides connector guidance with example M updates to help teams plan and execute upgrades with minimal disruption.

  https://learn.microsoft.com/en-us/fabric/data-factory/migrate-to-dataflow-gen2-using-upgrade-wizard

## Moderate Changes

- **Anomaly detection in Real-Time Intelligence (Preview)**

  Added support for creating anomaly detectors on Eventhouse shortcut tables. This extends analysis and continuous monitoring to external and federated sources without duplicating data, simplifying setup and governance.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/anomaly-detection

- **Install the Microsoft Fabric Chargeback app**

  Expanded setup instructions and added a verification step to confirm data is flowing after installation. Clarified configuration details for time zones, start-date logic, authentication defaults, and privacy levels, reducing misconfiguration and support overhead.

  https://learn.microsoft.com/en-us/fabric/enterprise/chargeback-app-install

- **What is Data Factory in Microsoft Fabric?**

  Introduced an SLA section aligning Fabric pipeline guarantees with Azure Data Factory. Clarifies reliability and timing expectations, helping teams plan operations against a documented 99.9% commitment.

  https://learn.microsoft.com/en-us/fabric/data-factory/data-factory-overview

- **Deploy Fabric Data Warehouse Using Pipelines**

  Documented safer default deployment behavior to prevent data loss and avoid dropping objects not present in source. Clarifies that deployments can succeed while skipping drops, which may cause drift until addressed, and reiterates single-warehouse deployment limits.

  https://learn.microsoft.com/en-us/fabric/data-warehouse/deploy-pipelines

- **Understand Microsoft Fabric licenses and capacity**

  Expanded coverage to clearly distinguish Azure F capacities and Microsoft 365 Power BI Premium P capacities, including billing models and recommendations. Added guidance on enabling Fabric on P capacities and introduced CSP purchasing as an additional path.

  https://learn.microsoft.com/en-us/fabric/enterprise/licenses

- **Optimal refresh for materialized lake views in a lakehouse**

  Clarified incremental refresh rules for aggregates, requiring partitioned sources with the partition column in GROUP BY for functions like AVG and STDDEV. Expanded exceptions to include MIN and MAX alongside SUM and non-distinct COUNT; mixing other aggregates still requires partitioning to avoid full refreshes.

  https://learn.microsoft.com/en-us/fabric/data-engineering/materialized-lake-views/refresh-materialized-lake-view

- **Power BI licensing guide for organizations**

  Updated terminology and links to reflect capacity-based purchasing rather than subscriptions. Aligns language and navigation to the “buy capacity” model for clearer procurement guidance.

  https://learn.microsoft.com/en-us/fabric/enterprise/powerbi/service-admin-power-bi-licensing

- **What's new in Microsoft Fabric?**

  Removed three preview feature entries from the What's New table to keep the list current. No other content changes were made.

  https://learn.microsoft.com/en-us/fabric/fundamentals/whats-new