# Microsoft Fabric
**Date created:** 2026-08-29 UTC  
**Tags:** Analytics, Best Practices, Billing, Configuration, Consumption, Get Started, Governance, Guidance, Identity, Licensing, Monitoring, Security, Troubleshooting  

## New Articles

- **Add schema object descriptions to a Microsoft Fabric data agent (preview)**

  Introduces schema object descriptions for SQL sources to add business meaning to tables, columns, and related elements, improving query interpretation. Explains preview/runtime prerequisites, inheritance from underlying data sources, and how to override descriptions at the agent level. Provides step-by-step UI instructions and a Python SDK example for programmatic updates, plus guidance on writing effective descriptions and links to related configuration and best-practices content.

  https://learn.microsoft.com/en-us/fabric/data-science/data-agent-schema-object-descriptions

## Major Changes

- **Best practices for improving data agent query generation**

  The article was overhauled to focus on boosting query accuracy with concrete techniques and examples. It now emphasizes clear schema naming, selective schema exposure, and using schema object descriptions to convey business context. New guidance covers cross-object rules (authoritative tables, joins, grain, filters, date logic), defining business terms and formats, and using example queries for complex scenarios. A testing and refinement workflow was added, and outdated, generic guidance was removed to streamline the article.

  https://learn.microsoft.com/en-us/fabric/data-science/data-agent-configuration-best-practices

- **Microsoft Fabric Mirrored Databases From Google BigQuery**

  Mirroring for Google BigQuery has moved to general availability with production support. The page title and notices were updated to remove preview language and highlight GA status. This change signals readiness for enterprise use and broader deployment.

  https://learn.microsoft.com/en-us/fabric/mirroring/google-bigquery

- **Ingest Data into the Warehouse**

  Added comprehensive guidance for using Workspace Identity with COPY INTO, including required storage, workspace, and SQL permissions, and a full SQL example. The behavior is clarified: Workspace Identity impersonates for source access while preserving the executing user’s SQL security context. COPY INTO now explicitly supports OneLake in addition to ADLS Gen2 and Azure Blob Storage, and notes potential failures due to sensitivity labels. Best practices were updated to reflect the expanded source options and identity behavior.

  https://learn.microsoft.com/en-us/fabric/data-warehouse/ingest-data

## Moderate Changes

- **Get events from Azure Event Hubs into Real-Time hub**

  Centralized schema selection and review/connect guidance into a shared include to reduce duplication and keep instructions consistent. The update clarifies fixed vs. dynamic schemas, Kafka header mapping, and schema registry usage without altering earlier configuration steps.

  https://learn.microsoft.com/en-us/fabric/real-time-hub/add-source-azure-event-hubs

- **Get events from Azure Service Bus into Real-Time hub (preview)**

  Reorganized connection steps to emphasize the Azure tab on the Add data page, with clearer search/filter and connect options. Added an alternative All sources path, updated screenshots and headings, and made minor wording improvements while retaining the existing configuration include.

  https://learn.microsoft.com/en-us/fabric/real-time-hub/add-source-azure-service-bus

- **On-demand billing for Apache Spark in Microsoft Fabric**

  Rebranded “Autoscale Billing” to “On-demand billing” across the article for consistent terminology. Text, headings, and comparisons were updated to reflect the new name without changing functionality.

  https://learn.microsoft.com/en-us/fabric/data-engineering/autoscale-billing-for-spark-overview

- **Configure On-demand Billing for Spark in Microsoft Fabric**

  Updated the article to use “On-demand billing” terminology throughout, including UI labels and screenshots. Clarified instructions and meter naming while keeping the overall procedure intact.

  https://learn.microsoft.com/en-us/fabric/data-engineering/configure-autoscale-billing

- **Configure custom live pools in Microsoft Fabric**

  Expanded prerequisites and clarified role-based permissions, distinguishing Admin-only actions from Member capabilities once settings are enabled. Added step-by-step guidance for the “Customize compute configuration for items” setting and a troubleshooting section for missing options.

  https://learn.microsoft.com/en-us/fabric/data-engineering/custom-live-pools-configure

- **Custom live pools for Fabric Data Engineering overview**

  Refined role definitions to differentiate Viewer/Contributor, Member, and Admin responsibilities, with clear ties to the workspace setting for compute customization. Clarified what Members can do once enabled, added B2B guest requirements, and linked to configuration steps.

  https://learn.microsoft.com/en-us/fabric/data-engineering/custom-live-pools-overview

- **Add and configure data sources in Fabric data agent**

  Added an option for Schema Object Descriptions (Preview) to enrich tables and columns with business context. This improves SQL generation quality when using the preview runtime.

  https://learn.microsoft.com/en-us/fabric/data-science/data-agent-add-datasources

- **Configure your data agent**

  Introduced “Schema object descriptions (Preview)” for SQL sources, including preview/runtime notes and supporting imagery. Streamlined guidance on agent instructions and examples, standardized terminology, and added visuals to aid setup.

  https://learn.microsoft.com/en-us/fabric/data-science/data-agent-configurations

- **Fabric data agent runtime**

  Clarified how runtime selection impacts when agent updates roll out and which preview features are available. Added a preview runtime entry for schema object descriptions to improve query understanding for SQL sources.

  https://learn.microsoft.com/en-us/fabric/data-science/data-agent-runtime

- **SQL sources in Fabric data agent**

  Expanded Advanced NL2SQL (preview) to highlight support for schema object descriptions that enhance schema comprehension. Clarified differences from NL2SQL and how existing configurations (schema selection, instructions, example queries) continue to work together.

  https://learn.microsoft.com/en-us/fabric/data-science/data-agent-sql-sources

- **Direct Lake overview**

  Updated to show Calculated Columns are now supported for Direct Lake in User Context only (Preview). Comparison tables and limitations were adjusted to reflect this new capability.

  https://learn.microsoft.com/en-us/fabric/fundamentals/direct-lake-overview

- **Mirroring**

  Added an important notice that Google BigQuery mirroring is now generally available with production support. Includes a link to detailed guidance for deployment.

  https://learn.microsoft.com/en-us/fabric/mirroring/overview

- **Fabric region availability**

  Updated region availability to indicate the Fabric App is now available in East US by removing it from the “Not available” list. This confirms broader regional coverage.

  https://learn.microsoft.com/en-us/fabric/admin/region-availability

- **Overview of managed private endpoints for Fabric**

  Clarified capacity requirements: managed private endpoints are supported only on capacities with 64 or more CUs, including Trial, F64, and larger. This replaces the earlier statement implying support across all F SKUs.

  https://learn.microsoft.com/en-us/fabric/security/security-managed-private-endpoints-overview

- **Tenant settings index**

  Added two settings: enabling search of OneLake catalog objects and controlling use of Fabric Copilot (preview). Removed two deprecated settings related to deployment plans and Database hub, and made minor text refinements.

  https://learn.microsoft.com/en-us/fabric/admin/tenant-settings-index

- **What's new in Microsoft Fabric?**

  Updated to reflect GA for Google BigQuery mirroring, removing preview references. Added August 2026 GA entries highlighting low-latency replication to OneLake, schema evolution, and integration across Fabric workloads.

  https://learn.microsoft.com/en-us/fabric/fundamentals/whats-new