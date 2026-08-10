# Microsoft Fabric
**Date created:** 2026-07-18 UTC  
**Tags:** Administration, Agent, Analytics, Automation, Governance, Monitoring, Security  

## New Articles

- **Get started with Real-Time Intelligence**

  Introduced an onboarding guide offering two entry paths: a pre-provisioned sample solution and a nine-part end-to-end tutorial. Defines core building blocks (Eventstream, Eventhouse with KQL database, KQL queryset, Real-Time Dashboard, Activator) and explains the Real-Time hub. Lists optional components (Event schema set, Map, Anomaly Detector, Digital twin builder) to extend scenarios and links to related overviews and tutorials.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/get-started-with-real-time-intelligence

- **Display and Formatting Options in PowerTable Sheet**

  Added a how-to guide for configuring PowerTable appearance, including row height, text and header formatting, and padding controls. Explains gridline customization, row highlighting modes with color options, header borders, and outline separators. Provides a reset option to revert all appearance changes to defaults.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-how-to-configure-display-formatting-settings

- **Schedule a User Data Function**

  Added step-by-step instructions to schedule User Data Functions using Microsoft Fabric Job Scheduler without pipelines. Covers prerequisites, creating schedules (controller, recurrence, interval, start/end, time zone), passing case-sensitive parameters, test runs, and monitoring in Monitor Hub. Explains configuring email notifications for failures and links to related next steps.

  https://learn.microsoft.com/en-us/fabric/data-engineering/user-data-functions/schedule-functions

- **Sensitivity label inheritance upon update**

  Introduced a conceptual article that explains how sensitivity labels are reevaluated and applied when items are modified, connected to new data sources, or linked via new lineage relationships. Details default label behavior across Power BI and non-Power BI items, downstream propagation (including automation and consent), and refresh-based reevaluation. Outlines precedence rules (more restrictive label wins, manual labels preserved), data source inheritance scope, and limitations such as gateway/VNet exclusions and downstream limits, with examples and links to related guidance.

  https://learn.microsoft.com/en-us/fabric/governance/service-security-sensitivity-label-inheritance-upon-update

## Major Changes

- **Overview of Fabric deployment pipelines**

  Expanded supported items for deployment pipelines to include new Data Factory items (Airflow, dbt Job, Operations Agent – all in preview), a Graph section (Graph Model and Graph QuerySet), CI/CD Variable Library, and IQ Plan (preview). Updated Real-Time Intelligence coverage by adding Maps and removing the Activator preview status. Removed preview status for SQL database and Data Science Data Agents, and corrected a Warehouse preview marker, broadening CI/CD applicability and clarifying readiness.

  https://learn.microsoft.com/en-us/fabric/cicd/deployment-pipelines/intro-to-deployment-pipelines

- **Overview of Fabric Git integration**

  Added support for additional item types in Git integration: Data Factory (Airflow, dbt Job, Operations Agent – preview), Real-Time Intelligence (Digital twin builder – preview; Activator now GA), and maintained Event Schema Set as preview. Split Graph into Graph Model and Graph QuerySet, and introduced new categories for CI/CD (Variable Library) and IQ (Ontology and Plan – preview). These updates expand versioning coverage and clarify maturity across services.

  https://learn.microsoft.com/en-us/fabric/cicd/git-integration/intro-to-git-integration

## Moderate Changes

- **What is Fabric Activator?**

  Removed the “preview” designation for Fabric copy jobs across the article, updating action lists, capability tables, and section headings. This signals general availability and aligns terminology with current product status.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/data-activator/activator-introduction

- **Trigger Fabric items**

  Updated references to reflect Copy jobs are now generally available and clarified that Copy jobs do not accept parameters. Retained the preview label for Publish business events to accurately represent current support.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/data-activator/activator-trigger-fabric-items

- **Tutorial: Create and activate a Fabric Activator rule**

  Updated the “Run Fabric activities” section to remove preview labels for Copy jobs and clarified that Copy jobs don’t accept parameters. Streamlines guidance to reflect current capabilities.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/data-activator/activator-tutorial

- **View refresh history and monitor your dataflows**

  Clarified that downloading detailed logs for gateway-refreshed dataflows requires only gateway-level Admin consent for diagnostics, not tenant-level consent. This simplifies setup for monitoring and auditing.

  https://learn.microsoft.com/en-us/fabric/data-factory/dataflows-gen2-monitor

- **Create an Operations Agent to Use with Ontology**

  Refined UI labels and steps in the setup flow (for example, “Instructions” to “Agent instructions,” “Knowledge source” to “Knowledge” with “Add data”) and emphasized saving before generating the playbook. Improves accuracy of the procedure without changing conceptual guidance.

  https://learn.microsoft.com/en-us/fabric/iq/ontology/how-to-create-operations-agent

- **Get the size of OneLake items**

  Removed preview markings for the OneLake storage report and deleted the preview note, indicating general availability. Users can rely on the report for production use.

  https://learn.microsoft.com/en-us/fabric/onelake/how-to-get-item-size

- **Information protection in Microsoft Fabric**

  Added a new capability describing sensitivity label inheritance upon updates and relationship changes, with a new table entry and dedicated explanation. Helps readers understand when labels are reevaluated and how inheritance works across modifications, new data connections, and lineage.

  https://learn.microsoft.com/en-us/fabric/governance/information-protection

- **Creating a lifecycle management policy in OneLake**

  Updated the main heading to remove the preview label, reflecting general availability. No procedural changes were made.

  https://learn.microsoft.com/en-us/fabric/onelake/onelake-lifecycle-management

- **Understand medallion lakehouse architecture for Fabric with OneLake**

  Updated performance guidance to target 128 MB–1 GB file sizes based on workload and consumption patterns. Adjusted layer-specific recommendations (smaller files for bronze with Spark prep; moderate for silver; larger files and row groups for gold) and advised Liquid Clustering over partitioning for silver and gold, discouraging new partitioning in bronze.

  https://learn.microsoft.com/en-us/fabric/onelake/onelake-medallion-lakehouse-architecture

- **OneLake storage tiers**

  Removed the preview label to indicate general availability and clarified limitations: CU consumption for Oracle and SQL database mirroring occurs only with on-premises data gateway versions prior to June 2026. Advises upgrading the gateway to avoid unnecessary CU usage; other mirroring types are unaffected.

  https://learn.microsoft.com/en-us/fabric/onelake/onelake-storage-tiers

- **Create and configure operations agents**

  Added a section on Operations agent identities explaining that each agent gets a dedicated Microsoft Entra Agent ID (service principal) for visibility and auditing. Clarified that agents run in delegated mode using the creator’s permissions via OBO, with actions attributed to the agent identity.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/operations-agent

- **Sensitivity label downstream inheritance**

  Expanded coverage to include inheritance upon updates and relationship changes, complementing existing downstream scenarios. Clarified that manual labels on associated reports aren’t overwritten when the semantic model label changes.

  https://learn.microsoft.com/en-us/fabric/governance/service-security-sensitivity-label-downstream-inheritance

- **Sensitivity labels troubleshooting**

  Added a troubleshooting section on label inheritance upon updates and new lineage relationships, including rules for default labeling and limitations. Clarified scope (for example, Power BI semantic models only for data source inheritance, exclusions for gateways/VNets) and consent requirements when fully automated downstream inheritance isn’t enabled, with a link to detailed guidance.

  https://learn.microsoft.com/en-us/fabric/governance/service-security-sensitivity-label-troubleshooting

- **Troubleshoot lifecycle management issues**

  Added guidance for unexpected uncommitted changes when report names contain special characters that trigger automatic dependency path corrections to semantic model links. Recommends committing the changes or using “Commit to new branch” to review diffs and confirm only path adjustments occurred.

  https://learn.microsoft.com/en-us/fabric/cicd/troubleshoot-cicd

- **The deployment pipelines process**

  Added a note clarifying that “same pipeline stage” refers to the stage’s numeric position rather than its display name. Ensures accurate stage matching across pipelines during deployment operations.

  https://learn.microsoft.com/en-us/fabric/cicd/deployment-pipelines/understand-the-deployment-process

- **Customer-managed keys for Fabric workspaces**

  Updated guidance on disabling CMK, removing prior discouragement and clarifying that disabling CMK leaves encryption with Microsoft-managed keys. Provides clearer expectations for post-disablement state.

  https://learn.microsoft.com/en-us/fabric/security/workspace-customer-managed-keys