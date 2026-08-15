# Microsoft Fabric
**Date created:** 2026-08-15 UTC  
**Tags:** Analytics, Best Practices, Billing, Compliance, Configuration, Consumption, Governance, Guidance, Identity, Licensing, Monitoring, Performance, Security, Troubleshooting  

## New Articles

- **Dataflow Gen2 cost and performance: capability benchmarks and CU costs**

  Introduced a new concept article that benchmarks key Dataflow Gen2 capabilities, including Fast Copy, Modern Evaluator, Optimized copy to Lakehouse, and Partitioned Compute. It explains CU pricing tiers and provides side-by-side comparisons that highlight faster runtimes and reduced CU consumption versus Gen1. The article offers practical design guidance and an FAQ on estimating costs, selecting the right capability, and using the Metrics app for planning.

  https://learn.microsoft.com/en-us/fabric/data-factory/dataflow-gen2-cost-performance-benchmarks

- **Consolidate data between sheets**

  Added a step-by-step guide for consolidating plans, budgets, and forecasts from multiple planning sheets using Infobridge. It shows how to build a bridge, append selected queries, and map row dimensions to a new planning sheet so teams can roll up data consistently. This streamlines multi-sheet aggregation and improves reconciliation.

  https://learn.microsoft.com/en-us/fabric/iq/plan/infobridge-how-to-consolidate-data-between-sheets

## Major Changes

- **Pricing for Dataflow Gen2**

  Expanded pricing guidance clarifying that Fast Copy charges are based on aggregate core time, not wall-clock duration, and how parallel cores contribute to billed time. The pricing model and table now detail core balancing, include a new row for Mapping Data Flow transforms compute (Preview), and provide an example rate calculation. A reference to cost/performance benchmarks helps users estimate and optimize spend.

  https://learn.microsoft.com/en-us/fabric/data-factory/pricing-dataflows-gen2

- **Tenant settings index**

  Updated tenant settings with new controls for Database hub access (preview), default ADBC connections, and Kusto options enabling embedded app visuals in Real-Time Dashboards. Microsoft Entra SSO gateway options were restructured into separate settings for on-premises/VNet gateways, and deployment plan was marked as preview. Legacy settings for Operations Agents creation and Plan items were removed, aligning the index with current capabilities.

  https://learn.microsoft.com/en-us/fabric/admin/tenant-settings-index

- **Understand capacity throttling and smoothing**

  Substantially revised guidance to explain capacity units, bursting, and smoothing with clearer examples and CU-seconds math. Introduced overage protection and progressive throttle stages, plus how carryforward and burndown affect enforcement. Enhanced monitoring and operational guidance shows how to detect and resolve throttling, including scaling options, autoscale notes, and user-facing error messages.

  https://learn.microsoft.com/en-us/fabric/enterprise/throttling

## Moderate Changes

- **Understand your Azure bill for a Fabric capacity**

  Updated billing meter descriptions to remove outdated preview references and clarify base naming and units, including storage shown in GB per month. These refinements help admins interpret bills accurately and reconcile capacity charges.

  https://learn.microsoft.com/en-us/fabric/enterprise/azure-billing

- **Configure custom live pools in Microsoft Fabric**

  Added scheduling guidance for live pool hydration, noting availability may lag schedule start and recommending a 60–90 minute buffer. The guide now advises verifying clusters in the Monitoring hub before latency-sensitive runs and refines best practices for scheduling.

  https://learn.microsoft.com/en-us/fabric/data-engineering/custom-live-pools-configure

- **Fast copy in Dataflow Gen2**

  Documented how Fast Copy runtime and cost are computed based on parallel core time rather than elapsed duration. This helps users plan performance and budget by understanding automatic core allocation and CU consumption mapping.

  https://learn.microsoft.com/en-us/fabric/data-factory/dataflows-gen2-fast-copy

- **How Direct Lake works**

  Clarified the “Keep your Direct Lake data up to date” model setting, its default, and when framing occurs based on Delta table changes. Added guidance on when to enable or pause automatic updates, plus options for manual, scheduled, and programmatic refresh; also noted that automatic updates pause on non-recoverable errors until a successful on-demand refresh.

  https://learn.microsoft.com/en-us/fabric/fundamentals/direct-lake-how-it-works

- **Configure calendar layout**

  Specified that Week and Day views require DateTime-type Start/End Date columns and highlighted quick navigation from Month/Week to Day view. Clarified backlog task behavior and aligned UI terminology with the current ellipsis icon.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-layouts/how-to-configure-calendar-layout

- **Configure Kanban layout**

  Standardized terminology from columns to stacks across the guide and UI references, including grouping, counts, and interactions. Clarified actions for collapsing, hiding, and revealing stacks, and aligned examples and alt text with the updated labels.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-layouts/how-to-configure-kanban-layout

- **Operation list**

  Added three tenant relocation audit operations—execution, consent granted, and consent revoked—so admins can track relocation state changes in logs. This improves governance and auditability during tenant moves.

  https://learn.microsoft.com/en-us/fabric/admin/operation-list

- **Known Limitations in Plan**

  Noted that inserting a Data input column can fail when a semantic model contains unsupported Unicode characters. Also documented that Blend (From Sheets) doesn’t support RLS, meaning source data isn’t filtered by viewer permissions.

  https://learn.microsoft.com/en-us/fabric/iq/plan/overview-limitations

- **Create table app by connecting to a semantic model**

  Added an FAQ clarifying that PowerTable seeds a Fabric SQL destination from the semantic model but doesn’t update the model or its source, regardless of storage mode or source type. It explains how new members surface in planning sheets and when a model refresh may be needed after schema changes.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-how-to-connect-semantic-model

- **Trusted workspace access**

  Clarified that trusted workspace access requires a purchased Microsoft Fabric capacity (F SKU) and isn’t supported on Trial capacities. Updated scenarios and prerequisites and noted that moving off F SKUs or to trial/non-Fabric capacities causes access to stop after about an hour.

  https://learn.microsoft.com/en-us/fabric/security/security-trusted-workspace-access

- **Configure Multi-Geo support for Fabric**

  Strengthened migration guidance to require both source and destination capacities to be active before starting a workspace migration. It details risks when migrating from paused or deleted capacities and advises resuming and rerunning the migration if issues occur.

  https://learn.microsoft.com/en-us/fabric/admin/service-admin-premium-multi-geo

- **Workspace identity**

  Clarified that workspace identities can be created in any workspace except My workspace and are supported across capacity SKUs for cloud connection credentials. Updated trusted workspace access requirements for firewall-enabled Storage accounts (F SKU needed) and described behavior when moving to trial capacities.

  https://learn.microsoft.com/en-us/fabric/security/workspace-identity

- **Authenticate with workspace identity**

  Updated considerations to confirm workspace identities can be created outside My workspace regardless of capacity SKU and used as credentials for cloud connections in any capacity. Reiterated that trusted workspace access requires assignment to a purchased F SKU.

  https://learn.microsoft.com/en-us/fabric/security/workspace-identity-authenticate