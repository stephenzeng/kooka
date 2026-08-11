# Microsoft Fabric
**Date created:** 2026-07-23 UTC  
**Tags:** Administration, AI, Analytics, Automation, Monitoring, Security  

## New Articles

- **Get Started with Mirroring in Fabric**

  Introduced a new getting-started guide that walks through the end-to-end mirroring lifecycle, from setup to troubleshooting and automation. It links to source-specific setup tutorials, highlights preview sources, and notes the auto-configured exception for Fabric SQL databases. The article shows how to explore mirrored data via the SQL analytics endpoint, OneLake, notebooks, and Power BI, and how to monitor health, review logs, and manage permissions. It also outlines advanced scenarios, including REST API usage and CI/CD.

  https://learn.microsoft.com/en-us/fabric/mirroring/get-started-with-mirroring

- **Join queries**

  Added a how-to for Infobridge that explains joining queries using inner, left, right, and full outer joins with practical examples. The guide provides a step-by-step UI walkthrough to join sample datasets by a shared column, with tips for choosing the join type and handling duplicate columns in results. The page is designated as a preview feature.

  https://learn.microsoft.com/en-us/fabric/iq/plan/infobridge-transform-queries/how-to-join-query

## Major Changes

- **Create Paginated Reports in Fabric Plan Intelligence Sheets**

  Expanded from a brief overview to a comprehensive how-to with detailed, step-by-step scenarios. The update adds prerequisites and introduces multiple pagination options, including fixed rows per page, single scrollable pages, and dimension-based or custom page breaks. Header and footer customization is greatly enhanced with presets, logos, slicer selections, timestamps, and color choices. The article also deepens coverage of annotations and adds robust export guidance for PDF and Excel, including handling hierarchical expansions.

  https://learn.microsoft.com/en-us/fabric/iq/plan/intelligence-how-to-create-paginated-reports

- **Commenting and Collaboration in Planning Sheet**

  Restructured and expanded guidance to cover end-to-end commenting workflows at both data and report levels. New capabilities include Teams notifications for mentions, explicit lock/resolve/reopen flows, and a centralized pane to view all comments with categorized filters. A comprehensive settings panel now controls comment enablement, UI indicators, column visibility, Teams notifications, and bulk delete/reset options, plus a new comments column for row-level discussions and clarified security permissions.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-how-to-add-comments

- **Schedule a Materialized Lake View Refresh**

  Introduced event-triggered refresh (Preview) alongside time-based schedules, with configuration for OneLake ingestion events and job events from Notebooks and Pipelines. The UI is updated to “Manage schedules,” and planning guidance was refined for unpredictable data arrival. Notes clarify dependencies (auto-created Notebook and Activator), current limitations, and updated steps for cross-lakehouse configurations and on-demand runs.

  https://learn.microsoft.com/en-us/fabric/data-engineering/materialized-lake-views/schedule-lineage-run

## Moderate Changes

- **Anomaly detection in Real-Time Intelligence (Preview)**

  Removed references to support for Eventhouse shortcut tables and analysis across external or federated sources. This reduces the documented scope of supported data sources while leaving other guidance unchanged.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/anomaly-detection

- **Manage your Fabric capacity**

  Updated guidance to reflect the retirement of Power BI Premium per-capacity (P SKUs) and directed customers to migrate to Microsoft Fabric capacity (F SKUs). Included links to a migration overview and FAQ to help plan the transition.

  https://learn.microsoft.com/en-us/fabric/admin/capacity-settings

- **Create a lakehouse in Microsoft Fabric**

  Clarified that creating a lakehouse no longer auto-creates a default semantic model for Power BI. Only the SQL analytics endpoint is automatically provisioned, which affects downstream reporting expectations.

  https://learn.microsoft.com/en-us/fabric/data-engineering/create-lakehouse

- **Data agent in Fabric consumption**

  Clarified token and Capacity Unit consumption by detailing that supporting context (instructions, examples, and conversation history) also contributes to usage, not just user questions. Added a new billing metric for cached input prompts at 10 CU seconds per 1,000 tokens to improve cost predictability.

  https://learn.microsoft.com/en-us/fabric/fundamentals/data-agent-consumption

- **Close your account, cancel your subscription, end your trial**

  Rewrote the section on Power BI Premium P SKUs to emphasize retirement and guide customers to migrate workloads to Fabric F SKUs. Added official resources, including an overview, decision guide, workspace migration steps, and FAQs.

  https://learn.microsoft.com/en-us/fabric/enterprise/fabric-close-end-cancel

- **Get Started with Materialized Lake Views in a Microsoft Fabric Lakehouse**

  Updated the scheduling steps to reflect the current UI with “Manage” and “Manage schedules,” and clarified how to enable refresh, select views, choose refresh types, and configure settings. Improved guidance for navigation and monitoring through Recent runs and tracking ongoing executions.

  https://learn.microsoft.com/en-us/fabric/data-engineering/materialized-lake-views/get-started-with-materialized-lake-views

- **Lakehouse SQL analytics endpoint use cases**

  Clarified that warehouses, mirrored databases, SQL databases, and Azure Cosmos DB also auto-provision SQL analytics endpoints. This corrects earlier implications and explains why a workspace may have more endpoints than lakehouses.

  https://learn.microsoft.com/en-us/fabric/data-engineering/lakehouse-sql-analytics-endpoint-use-cases

- **Microsoft Spark Utilities (MSSparkUtils) for Fabric**

  Updated mounting guidance to recommend Microsoft Entra tokens as the default authentication method, expanding supported options beyond account keys and SAS tokens. Included a reference to related mount/unmount documentation.

  https://learn.microsoft.com/en-us/fabric/data-engineering/microsoft-spark-utilities

- **Power BI licensing guide for organizations**

  Revised external sharing guidance to state that a Fabric (Free) license is sufficient only when content runs in Fabric capacity F64 or larger, and removed references to P SKUs. Added a retirement notice for P SKUs and links to migration resources to help organizations plan the move to F SKUs.

  https://learn.microsoft.com/en-us/fabric/enterprise/powerbi/service-admin-power-bi-licensing