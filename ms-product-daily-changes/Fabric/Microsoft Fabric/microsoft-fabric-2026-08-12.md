# Microsoft Fabric
**Date created:** 2026-08-12 UTC  
**Tags:** Analytics, Best Practices, Configuration, Get Started, Governance, Guidance, Monitoring, Performance, Security, Troubleshooting  

## New Articles

- **Workspace Monitoring for Dataflow Gen2 in Microsoft Fabric**

  Introduced a how-to guide for enabling and using workspace monitoring to track Dataflow Gen2 refresh and publish events, including CI/CD scenarios. Explains how to enable monitoring, access the generated eventhouse/KQL database, and interpret the ItemJobEventLogs schema for statuses, job types, and correlations. Provides KQL examples for failure detection, duration analysis, run history, and scheduled versus manual comparisons. Adds guidance to create KQL-based alerts and best practices for combining workspace monitoring with dataflow history and the monitoring hub.

  https://learn.microsoft.com/en-us/fabric/data-factory/dataflow-gen2-workspace-monitoring

- **Configure calendar layout**

  Added step-by-step guidance for creating a PowerTable calendar view, mapping display, start, and end/duration fields. Describes switching among Month/Week/Day views, customizing formats and week settings, and navigating with Previous/Next/Today. Details adding, editing, duplicating, and deleting tasks with appropriate access controls, plus importing in bulk and interacting via hover and pop-ups. Covers filtering, bulk edits, and managing or resetting the layout.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-layouts/how-to-configure-calendar-layout

- **Configure Kanban layout**

  Added instructions to create and configure a Kanban layout in PowerTable, including Task ID/Name, Stack By, Assignee, and Progress. Explains navigating cards, compact versus expanded views, collapsing columns, and toggling header counts. Shows how to add, edit, move, duplicate, and delete tasks, with filtering, sorting, grouping within columns, bulk editing, and layout management.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-layouts/how-to-configure-kanban-layout

- **Move shortcuts to a new region**

  Introduced a migration guide for relocating OneLake shortcuts by recreating them in a workspace in the destination region. Covers prerequisites, downtime planning, documenting dependencies, and recreating shortcuts via the portal or the OneLake Shortcuts REST API. Explains handling external connections (ADLS Gen2, S3), updating downstream consumers, validating results, and post-migration cleanup. Lists key limitations, including no direct relocation, metadata history loss, and write constraints, with links to related articles and APIs.

  https://learn.microsoft.com/en-us/fabric/onelake/shortcuts/move-shortcuts-region

- **Bottom-up Planning for Business Hierarchies in Fabric Plan**

  Introduced the bottom-up planning concept where detailed inputs roll up automatically to parent hierarchy levels. Outlines the process from detailed entry through aggregation, review, and refinement. Highlights benefits such as accurate consolidation and suitability for sales forecasting, expense planning, demand estimation, production, and workforce planning. Emphasizes many-to-one aggregation for reliable consolidated plans.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-concept-bottom-up-planning

- **Top-down Planning for Business Hierarchies in Fabric Plan**

  Introduced the top-down planning concept where high-level targets are allocated to lower levels using configurable rules. Explains process steps, including defining values, evaluating hierarchies, and distributing via allocation logic. Describes benefits for alignment and speed across budgets, revenue targets, workforce, and capacity planning, with consistent application of rules. Emphasizes translating strategy into actionable plans through one-to-many allocation.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-concept-top-down-planning

- **Generate Statistical Forecasts using the Predict Feature**

  Added a how-to guide for generating statistical forecasts in Fabric Plan using the Predict feature. Details prerequisites and historical data needs, selection of cells and date ranges, configuration via profiles, and choosing top-down or bottom-up approaches. Explains algorithm options (MSTL, Exponential Smoothing, ARIMA), seasonality settings, and guidance on matching patterns to methods. Covers reviewing, saving, and exporting forecasts with graphical and tabular previews.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-forecasting/planning-how-to-generate-statistical-forecasts-using-predict-feature

- **Workspace Outbound Access Protection for Fabric Maps**

  Introduced outbound access protection for Fabric Maps (preview), detailing how rules apply to Lakehouse, Kusto, Ontology, and external geospatial connections. Explains evaluation points across CRUD, runtime access validation, and external connection resolution, with steps to enable protection and configure data connection rules. Provides guidance for geospatial services (WMS/WMTS/WFS) via the Geospatial Web Services connection kind and outlines limitations, including fail-closed behavior and planned support for additional sources. Recommends next steps to build allow lists using private endpoints or data connection rules.

  https://learn.microsoft.com/en-us/fabric/security/workspace-outbound-access-protection-fabric-maps

## Major Changes

- **Configure Private Networks for Azure Cosmos DB Fabric Mirroring**

  Rewrote guidance to center on private-network mirroring of Azure Cosmos DB for NoSQL using a Virtual Network Data Gateway and trusted-workspace network ACL bypass, replacing IP allow lists and the prior quick-start script. Added end-to-end portal and CLI/PowerShell steps, including RP registration, delegated gateway subnet setup, data-plane RBAC, ACL bypass enablement, gateway provisioning, OAuth-based v2 connection creation, and mirroring via REST API due to current UI limitations. Expanded limitations (same-region scope, OAuth-only, dedicated delegated subnet, workspace-specific ACLs) and added troubleshooting for OAuth token issues and outbound/NAT requirements given default outbound access retirement. The update streamlines secure deployment and clarifies operational constraints for reliable private connectivity.

  https://learn.microsoft.com/en-us/fabric/mirroring/azure-cosmos-db-private-network

- **Roles in Fabric plan**

  Substantially expanded and reorganized planning role documentation with detailed descriptions for Viewer, Stakeholder, and Planner, including capabilities and audiences. Clarified that creating/editing PowerTable and intelligence sheets are Stakeholder activities, while Planner is reserved for planning sheets, and added a permission matrix across workloads. Updated guidance on dynamic role assignment, workspace role mapping, and introduced an “Upgrade roles” section covering session lifecycles and admin prompts. Added capability tables and refined FAQs to improve clarity without changing core policies.

  https://learn.microsoft.com/en-us/fabric/iq/plan/overview-roles

## Moderate Changes

- **Experience-specific disaster recovery guidance**

  Added a Platform section subsection on enabling monitoring for the recovered workspace and clarified that monitoring data from the original workspace does not carry over. Updated the introduction to state the section covers recovery steps for shared Fabric capabilities, improving post-recovery setup guidance.

  https://learn.microsoft.com/en-us/fabric/security/experience-specific-guidance

- **Upgrade Dataflow Gen1 to Dataflow Gen2 (CI/CD) using the Upgrade Wizard**

  Removed prior guidance that tenant admins could upgrade dataflows they don’t own via the Power BI REST API, including bulk upgrades and ownership preservation. Updated prerequisites and removed the dedicated paragraph to align documentation with supported capabilities.

  https://learn.microsoft.com/en-us/fabric/data-factory/migrate-to-dataflow-gen2-using-upgrade-wizard

- **Scale Your Capacity Size in Azure**

  Added an important notice that resizing across the F256-and-below to F512-and-above SKU boundary can interrupt capacity, cancel running operations, and stop jobs. Recommends performing such changes during maintenance windows or low activity and rerunning any canceled jobs.

  https://learn.microsoft.com/en-us/fabric/enterprise/scale-capacity

- **Semantic model best practices for data agent**

  Added an “Advanced DAX generation (preview)” section describing a multi-step reasoning tool that leverages model metadata to interpret questions and generate DAX for complex scenarios, with potential accuracy and latency gains. Includes enablement steps via preview runtime and clarifies instance value indexing depends on the semantic model’s Q&A setting (enabled by default for Import/Direct Lake) with a forthcoming replacement setting noted.

  https://learn.microsoft.com/en-us/fabric/data-science/semantic-model-best-practices

- **Workspace outbound access protection**

  Expanded the Real-Time Intelligence workload coverage to include Fabric Maps and added a link to its outbound access protection guidance, signaling broader applicability.

  https://learn.microsoft.com/en-us/fabric/security/workspace-outbound-access-protection-overview