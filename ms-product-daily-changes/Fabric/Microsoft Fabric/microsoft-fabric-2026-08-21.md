# Microsoft Fabric
**Date created:** 2026-08-21 UTC  
**Tags:** Analytics, Automation, Compliance, Configuration, Consumption, Governance, Guidance, Monitoring, Performance, Security  

## New Articles

- **Writeback Planning Data to Fabric SQL**

  Introduced a concept article explaining how to write back planning data to Fabric SQL or OneLake for centralized storage and downstream reporting. It covers supported data types, optional change-history structures (long/wide variants), and automatic synchronization to keep plan inputs current. The guidance details runtime selection of measures, data filtering, and validation rules to ensure data quality, plus scenario management to control which versions are persisted. This helps teams integrate planning inputs across Fabric and streamline analytics in Power BI and other workloads.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-concept-writeback

## Major Changes

- **Dataflow Gen2 cost and performance: capability benchmarks and CU costs**

  Substantially expanded the article into a definitive reference for Dataflow Gen2 performance and cost. It adds broader benchmarks with CU consumption metrics, Gen1 vs. Gen2 comparisons, new summary tables and charts, and a transparent methodology section. Billing guidance for Standard Compute and per-tier CU calculations were clarified, and Partitioned Compute is marked as Preview with scope notes. The updated “cost over time” analysis and refreshed FAQ help organizations estimate costs, plan migrations, and set realistic performance expectations.

  https://learn.microsoft.com/en-us/fabric/data-factory/dataflow-gen2-cost-performance-benchmarks

- **Insert Data Input Rows in a Planning Sheet**

  The article was refocused to clearly explain when and why to insert data input rows, emphasizing the basic steps. Advanced procedures and import/configuration options were removed to reduce complexity and keep the guidance task-centric. This streamlining makes it easier for users to execute common insert actions while avoiding outdated or niche instructions.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-how-to-insert-rows-data-input

- **Manage Inserted Rows in a Planning Sheet**

  Content was restructured to center on using the Manage Rows pane to search, filter, show, and hide items. Formatting for available actions was improved, and the prior “Row settings” configuration details were removed. The update clarifies day-to-day management tasks and reduces distraction from deprecated or advanced options.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-how-to-manage-inserted-rows

## Moderate Changes

- **Network security for continuous integration/continuous deployment**

  Updated guidance clarifies that Deployment Pipelines aren’t supported for workspaces with inbound access protection, and it removes a prior restriction related to outbound access protection. This helps admins avoid unsupported configurations and align security settings with deployment needs.

  https://learn.microsoft.com/en-us/fabric/cicd/cicd-security

- **Azure Map tenant settings**

  Added notes explaining that if Azure Maps access or cross-region processing is disabled, users can open Map items but will see a blank basemap while data layers remain visible. Guidance indicates re-enabling the setting restores the full mapping experience, helping admins balance controls with usability.

  https://learn.microsoft.com/en-us/fabric/admin/map-settings

- **Operation list**

  Expanded the audit log operations list with entries for policy and policy set lifecycle actions, including activation, deactivation, creation, deletion, reading, and updates. These additions improve governance and compliance visibility across Fabric policy changes.

  https://learn.microsoft.com/en-us/fabric/admin/operation-list

- **Query Eventstream monitoring data (preview)**

  Removed the notice that Eventstream workspace monitoring was temporarily disabled, indicating the capability is available again. This reduces confusion and signals admins can resume using workspace monitoring as expected.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/query-fabric-workspace-monitoring-data