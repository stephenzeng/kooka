# Microsoft Fabric
**Date created:** 2026-09-04 UTC  
**Tags:** Analytics, Billing, Compliance, Configuration, Consumption, Governance, Guidance, Identity, Monitoring, Troubleshooting  

## New Articles

- **Other operators**

  Introduced a reference for operators in Fabric Planning formulas, covering arithmetic, comparison, grouping with parentheses, and unary signs. Provides syntax blocks and examples to help authors control evaluation order and build accurate expressions. Includes guidance for applying operators with calendar date nodes and combining multiple operations in a single formula.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-reference-formulas/planning-reference-other-operators

- **Save a Fabric map to a Real-Time Dashboard**

  Added step-by-step guidance to save an existing Fabric map to a new or existing Real-Time Dashboard, including prerequisites and permissions. Clarifies that the dashboard embeds a view-only map tile that references the source map, so saved map changes require a page reload and follow the source map’s refresh behavior. Highlights access requirements, lifecycle behavior when items are moved or deleted, and limitations such as no editing of queries, data, layers, or styling from the dashboard.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/map/save-map-to-real-time-dashboard

- **Build Top-Down and Bottom-Up Revenue Plans in Fabric Planning**

  Published a tutorial that walks through setting a top-down 2026 revenue target, allocating values proportionally, and managing locks to control distribution. Demonstrates building a bottom-up plan with targeted uplifts, quarterly trends, and bulk edits to adjust specific regions and categories. Shows how to collaborate with comments, user tagging, and a Status column to track progress.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-tutorial/planning/tutorial-1-allocation-collaboration

## Major Changes

- **Sharing Microsoft Fabric Maps**

  Expanded guidance to include adding Fabric maps to Real-Time Dashboards, detailing view-only interactions and how source updates propagate. Clarifies permission requirements across the dashboard, map, and data source, and adds workflow notes for saving, placing, renaming, and sizing tiles (including behavior when re-saving). Reframed sharing options with a new comparison table for direct sharing, organization apps, and Real-Time Dashboards, plus a feature preview note and updated next steps.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/map/sharing-maps

## Moderate Changes

- **Create a Real-Time Dashboard**

  Updated the Fabric Maps tile guidance to standardize terminology, set view-only interactions, and note that dashboard parameters don’t affect the map. Clarifies that the tile references the source map, so saved changes require reloading the dashboard, and that editing queries, data sources, layers, filters, or styling isn’t supported in the dashboard. Adds details on resizing/maximizing, viewer access and authorization, and a workflow to save a map directly to a Real-Time Dashboard.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/dashboard-real-time-create

- **OneLake compute and storage consumption**

  Clarified that certain OneLake operations executed during Spark workloads will start being included in OneLake CU consumption reporting on October 1, 2026; consumption rates remain unchanged, but CU usage may rise for workloads with many such operations. Updated the OneLake security RLS consumption table by changing Capacity Units from 0.1 CU seconds to 1 CU seconds for the OneLake security RLS operation.

  https://learn.microsoft.com/en-us/fabric/onelake/onelake-consumption

- **Operations Agent Best Practices and Limitations**

  Expanded Eventhouse data source support to include shortcut tables and clarified that queries must include a timestamp so the agent can track the latest time and handle late-arriving events. Revised regional availability to remove the South Central US exclusion; the agent is now excluded only in East US.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/operations-agent-limitations

- **Refresh SQL analytics endpoint activity**

  Renamed the activity and UI references from “SQL Endpoint” to “SQL analytics endpoint,” including updated headings and settings that specify the endpoint ID. Clarified activity messages and lock contention troubleshooting, refreshed section anchors, and aligned terminology and alt text across examples and images.

  https://learn.microsoft.com/en-us/fabric/data-factory/refresh-sql-endpoint-activity

- **Microsoft Fabric for US Government GCC High customers (preview)**

  Updated the capabilities table: Data Engineering now includes API for GraphQL and User Data Functions; Data Factory removes “default semantic model”; Developer experience removes API for GraphQL and Git integration; and Power BI adds direct Lake on SQL and direct Lake on OneLake. These changes refine feature expectations for GCC High during public preview.

  https://learn.microsoft.com/en-us/fabric/enterprise/us-government-community-cloud-high