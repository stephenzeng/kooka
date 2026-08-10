# Microsoft Fabric
**Date created:** 2026-07-11 UTC  
**Tags:** Administration, Agent, AI, Analytics, Monitoring  

## New Articles

- **Observability for Fabric data agents in Microsoft Foundry**

  Introduced guidance on tracing Fabric data agents connected to Microsoft Foundry via the project’s linked Application Insights, enabling end-to-end diagnostics alongside Foundry agent traces. Explains the trace structure (agent and tool spans), how to investigate performance and failures, and required permissions to view telemetry. Details a tenant setting that governs sending operational metadata (agent/data source names, reasoning step IDs, conversation IDs) without customer content.

  https://learn.microsoft.com/en-us/fabric/data-science/fabric-data-agent-foundry-observability

- **Operations Agent for Pipelines (preview)**

  Introduced an AI-powered agent in Data Factory that monitors pipeline health, diagnoses failures, and recommends performance optimizations using execution logs, activity metadata, and performance signals. Shows how to create and start the agent from the pipeline canvas, customize instructions, and receive proactive Microsoft Teams notifications. Current scope focuses on health monitoring scenarios, with examples for failure triage, performance tuning, and large-scale observability.

  https://learn.microsoft.com/en-us/fabric/data-factory/operations-agent-for-pipelines

## Moderate Changes

- **Add an Azure Data Explorer database source to an eventstream (preview)**

  Removed the Limitations section that cited query result size and record count caps and potential failures under high ingestion rates. This streamlines guidance and suggests previous limits may no longer apply or have been re-evaluated.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/add-source-azure-data-explorer-database

- **Burstable Capacity**

  Added new high-capacity SKUs F4096 and F8192 to the guardrails table with updated burst ranges. This helps admins plan for short-term performance spikes at larger scales.

  https://learn.microsoft.com/en-us/fabric/data-warehouse/burstable-capacity

- **Capacity overage (preview) in Microsoft Fabric**

  Expanded the capacity table with F4096 and F8192, including their daily CU hours. This clarifies overage expectations and budgeting for higher-tier capacities.

  https://learn.microsoft.com/en-us/fabric/enterprise/capacity-overage-overview

- **Configure and manage starter pools in Fabric Spark**

  Added F4096 and F8192 to the starter pool limits with core/memory specs, node sizes, and default/max node counts. This improves sizing guidance for large Spark workloads and faster startup.

  https://learn.microsoft.com/en-us/fabric/data-engineering/configure-starter-pools

- **Direct Lake overview**

  Added F4096 and F8192 tiers to the Direct Lake semantic model capacity limits. This helps model authors understand memory, CPU, and concurrency at the highest capacity levels.

  https://learn.microsoft.com/en-us/fabric/fundamentals/direct-lake-overview

- **Understand Microsoft Fabric licenses**

  Expanded the SKU table with F4096 and F8192 entries and associated CU details. This provides clearer licensing choices for organizations scaling to top-tier capacities.

  https://learn.microsoft.com/en-us/fabric/enterprise/licenses

- **Plan your capacity size**

  Updated capacity planning tables with new SKUs F4096 and F8192 and their CU totals. This enables more accurate right-sizing for large, mission-critical deployments.

  https://learn.microsoft.com/en-us/fabric/enterprise/plan-capacity

- **Configure workloads in a Premium capacity**

  Added F4096 and F8192 to limit tables, setting a 10 GB hard ceiling for offline semantic model size and a 40 GB effective per-workspace memory query limit. This clarifies operational boundaries when upgrading to higher tiers.

  https://learn.microsoft.com/en-us/fabric/enterprise/powerbi/service-admin-premium-workloads

- **What is Power BI Premium?**

  Added F4096 and F8192 to capacity metrics and to Dataflows parallel tasks/memory limits. This supports accurate sizing, concurrency planning, and workload configuration for new tiers.

  https://learn.microsoft.com/en-us/fabric/enterprise/powerbi/service-premium-what-is

- **Concurrency limits and queueing in Apache Spark for Fabric**

  Expanded the Spark capacity limits with F4096 and F8192 core allocations and per-job caps, and cleaned up an obsolete “Not available” entry. This provides clearer guidance for parallelism and job planning at higher capacities.

  https://learn.microsoft.com/en-us/fabric/data-engineering/spark-job-concurrency-and-queueing

- **Billing and Utilization Reporting**

  Extended the SQL database SKU sizing estimations with F4096 and F8192 and their corresponding values. This aids in forecasting utilization and cost at scale.

  https://learn.microsoft.com/en-us/fabric/database/sql/usage-reporting

- **What's new in Microsoft Fabric?**

  Added a new entry for Operations Agent for Pipelines (Preview) with details and a link, and updated the timeline to include July 2026 and shift the AI-assisted Synapse pipeline migration item to July. This keeps the release timeline and feature highlights current for customers tracking announcements.

  https://learn.microsoft.com/en-us/fabric/fundamentals/whats-new