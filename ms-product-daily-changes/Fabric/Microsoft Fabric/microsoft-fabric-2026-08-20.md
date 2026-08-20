# Microsoft Fabric
**Date created:** 2026-08-20 UTC  
**Tags:** Analytics, Best Practices, Compliance, Configuration, Get Started, Governance, Guidance, Identity, Licensing, Monitoring, Security, Troubleshooting  

## New Articles

- **Statistical Functions: Calculate Measures of Central Tendency**

  Introduced reference documentation for MEDIAN, MODE, and MODESNGL in Plan, including syntax, parameters, and return values. Provides worked examples and notes on error behavior when no values repeat. Links to equivalent Excel functions to ease adoption and comparison.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-reference-formulas/statistical-functions/calculate-measures-central-tendency

- **Statistical Functions: Calculate normal distribution values**

  Added a reference covering NORMDIST, NORMSDIST, NORMINV, and NORMSINV for computing normal and standard normal distributions, probabilities, and inverse values. Includes purpose, syntax, arguments, and practical examples with screenshots. Cross-references Excel equivalents for familiarization.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-reference-formulas/statistical-functions/calculate-normal-distribution

- **Statistical Functions: Calculate Percentiles and Percent Ranks**

  Published guidance for PERCENTILEINC, PERCENTILEEXC, PERCENTRANKINC, and PERCENTRANKEXC to analyze data distribution and relative position. Details syntax, boundary/error behavior, and examples to apply inclusive and exclusive methods correctly. Includes images and links to analogous Excel functions.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-reference-formulas/statistical-functions/calculate-percentiles-percent-ranks

- **Statistical Functions: Calculate Ranking and Quartiles**

  Documented QUARTILEINC and QUARTILEEXC with behavioral differences and constraints, plus RANKEQ and RANKAVG for ranking with ties. Provides clear syntax, return values, and examples to choose the right method for analysis. Maps each function to its Excel counterpart for continuity.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-reference-formulas/statistical-functions/calculate-ranking-quartiles

- **Statistical Functions: Calculate Variance and Standard Deviation**

  Added reference for VARS, VARP, STDEVS, and STDEVP to calculate sample vs. population variance and standard deviation. Explains when to use each variant, with syntax, arguments, and worked examples. Includes screenshots and Excel equivalence for quick onboarding.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-reference-formulas/statistical-functions/calculate-variance-standard-deviation

- **Use dimension level in Infobridge**

  Introduced a how-to explaining how Dimension Level converts selected dimension items into measures and moves original measures to rows in Infobridge queries. Provides step-by-step setup in Model Builder, creating and validating queries, and resetting Dimension Level. Includes guidance for restoring desired measures via Manage Queries/Manage Source.

  https://learn.microsoft.com/en-us/fabric/iq/plan/infobridge-how-to-use-dimension-level

- **Approval Workflows in Fabric Plan**

  New conceptual article outlining how to route planning changes through sequential approval levels. Explains key capabilities such as configuring levels, assigning approvers, tracking statuses, Teams notifications, and handling rejections. Describes implementation options via the Approval Workflow interface or scripts, with a link to configuration guidance.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-concept-approval-workflow

- **Microsoft Fabric for US Government GCC High customers**

  Added environment-specific guidance for GCC High, including eligibility, licensing (no free trials; Power BI Pro requirements), and sign-in URL. Lists GCC High API endpoints and a feature availability matrix across workloads for Public Preview and GA. Provides links for government customers and subscription guidance to streamline deployment decisions.

  https://learn.microsoft.com/en-us/fabric/enterprise/us-government-community-cloud-high

## Major Changes

- **Customize Real-Time Dashboard visuals**

  Expanded customization guidance with a comprehensive KPI section covering display modes, setup steps, and configuration of values, conditional thresholds, and reference lines. Added notes on accessibility, event-driven change detection with stale-data handling, and responsive sizing. Updated property applicability tables so KPI is included for conditional formatting, value columns, Y-axis bounds, and reference lines, enabling consistent configuration across visuals.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/dashboard-visuals-customize

- **Experience-specific disaster recovery guidance**

  Broadened Data Engineering recovery to include user data functions and GraphQL APIs. Added detailed recovery procedures for user data functions via Git integration (preparation, synchronization, and considerations) and manual reconstruction from source backups with dependency reinstallation and validation. Also updated the GraphQL section heading to remove the preview label, clarifying current support status.

  https://learn.microsoft.com/en-us/fabric/security/experience-specific-guidance

## Moderate Changes

- **How to Create a Copy Job in Data Factory**

  Added guidance on choosing data sources and destinations for Copy jobs, integrating modules for Home, New, OneLake catalog, Azure, Sample data, and New Fabric item. This streamlines the get data experience and clarifies where to start based on source type.

  https://learn.microsoft.com/en-us/fabric/data-factory/create-copy-job

- **Apply conditional formatting in Real-Time Dashboard visuals**

  Expanded conditional formatting to support KPI visuals in addition to multi stat, stat, and table. Added step-by-step instructions for configuring KPI rules in the Visual setup pane with an illustrative example, enabling consistent visual cues for key metrics.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/dashboard-conditional-formatting

- **Create a Real-Time Dashboard**

  Introduced instructions to add a Fabric Maps tile (preview), explaining the differences from the built-in Map visual and how embedded map settings remain managed in the original item. Provided steps to add, size, and save the tile, detailed viewer interactions, and noted error handling if the referenced map is missing.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/dashboard-real-time-create

- **How to configure dbt jobs in Microsoft Fabric**

  Updated the supported adapters, adding the Fabric Lakehouse adapter with Microsoft Entra (OAuth) authentication. Refreshed adapter versions for Azure SQL Database (1.9.1), Fabric Data Warehouse (1.10.0), PostgreSQL (1.10.0), and Snowflake (1.11.5) to align with current support.

  https://learn.microsoft.com/en-us/fabric/data-factory/dbt-job-configure

- **Get data in Dataflow Gen2**

  Reorganized the get data experience with modular entry points (Home, Copilot, New, Recent, OneLake catalog, Upload, Blank table, Blank query) and clarified access via the ribbon and dialog. Consolidated Copilot guidance for selecting recent tables, chatting to transform, @-selecting columns, and restoring steps, and streamlined connector guidance to the overview.

  https://learn.microsoft.com/en-us/fabric/data-factory/get-data-dataflow-gen2

- **Get Started with Mirroring in Fabric**

  Added guidance for selecting the source connection when creating a mirrored item, with options via Home, New, and OneLake catalog. Instructs readers to complete source-specific setup after choosing the connection to ensure a successful mirror.

  https://learn.microsoft.com/en-us/fabric/mirroring/get-started-with-mirroring

- **Get data experience for pipelines**

  Introduced a “Choose a data source for a pipeline” section with options spanning Home, New, OneLake catalog, Azure, Sample data, and New Fabric item, and clarified OneLake catalog concepts like connectors, recent, recommended, and Fabric items. Updated instructions for launching from the Copy activity via Connection > Browse all and refined related link text.

  https://learn.microsoft.com/en-us/fabric/data-factory/modern-get-data-experience-pipeline

- **What is Real-Time Dashboard?**

  Added KPI to the supported visuals table, describing its role as a single key metric tile with optional trend. Included example scenarios and a reference image to help users choose the right visual for critical metrics.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/real-time-dashboards-overview

- **OneLake table, column, and row-level security**

  Clarified that RLS roles do not support dynamic and multitable queries. This sets expectations on RLS capabilities and helps prevent unsupported configurations.

  https://learn.microsoft.com/en-us/fabric/onelake/security/table-column-row-security

- **Troubleshoot Fabric Apps**

  Replaced prior guidance with a focused section on “Database schema apply fails,” emphasizing that the app code is the source of truth and advising against out-of-band schema changes. Lists unsupported column operations and provides remediation steps, with a caution on using --force due to data-loss risk.

  https://learn.microsoft.com/en-us/fabric/apps/troubleshooting

- **Ontology (preview) tutorial part 0: Introduction and environment setup**

  Clarified Lakehouse creation by separating item creation from naming, workspace location, and enabling Lakehouse schemas before creation. This reduces setup errors and ensures schema features are enabled from the start.

  https://learn.microsoft.com/en-us/fabric/iq/ontology/tutorial-0-introduction

- **Workspace identity support in Data Factory**

  Documented that the identity executing a pipeline must be an admin, member, or contributor in the workspace for Fabric to issue a workspace identity token. Highlights diagnostics for schedules that fail while manual runs succeed due to insufficient workspace role assignments.

  https://learn.microsoft.com/en-us/fabric/data-factory/workspace-identity

- **Authenticate with workspace identity**

  Added an important note that the running identity (user or service principal) must have an admin, member, or contributor role in the workspace, not just data source permissions. Clarifies why scheduled runs can fail while manual runs succeed and directs readers to verify workspace role assignments.

  https://learn.microsoft.com/en-us/fabric/security/workspace-identity-authenticate