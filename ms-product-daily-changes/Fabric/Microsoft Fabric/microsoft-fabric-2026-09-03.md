# Microsoft Fabric
**Date created:** 2026-09-03 UTC  
**Tags:** Analytics, Automation, Best Practices, Compliance, Configuration, Consumption, Get Started, Governance, Guidance, Identity, Monitoring, Security, Troubleshooting  

## New Articles

- **Fabric Capacity Operation Source in Fabric Eventstream**

  Introduced a new how-to for ingesting Fabric capacity operation events directly into Eventstreams. It walks through prerequisites, connector selection, connection, and publishing, with guidance to route data to destinations like Lakehouse and apply transformations. The article also calls out a current limitation: Git integration and deployment pipelines are not supported for this source and may error during export/import. This helps admins and engineers operationalize capacity telemetry for monitoring and downstream analytics.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/add-source-fabric-capacity-operation-events

- **Capacity Operation Events in Fabric Real-Time Hub**

  Added step-by-step guidance to create eventstreams for capacity operation events from Real-Time Hub. It explains the supported event type, what metrics are captured (CU consumption, duration, throttling, status), and multiple entry points to create and configure streams. Verification steps and links to processing, analysis, and alerting content are included, enabling faster setup of capacity monitoring pipelines.

  https://learn.microsoft.com/en-us/fabric/real-time-hub/create-streams-fabric-capacity-operation-events

- **Explore Fabric capacity operation events in Fabric Real-Time hub**

  Published a deep-dive article on exploring capacity operation events, including event details pages and schema. It describes how to create eventstreams and set alerts from the event view, and documents the CloudEvents envelope and a comprehensive schema for operations telemetry. This helps teams understand available fields and build precise monitoring and analytics solutions.

  https://learn.microsoft.com/en-us/fabric/real-time-hub/explore-fabric-capacity-operation-events

- **Set alerts on Fabric capacity operation events in Real-Time hub**

  Added a how-to for configuring alerts on capacity operation events to detect spikes, throttling, or failures. It covers selecting the event type and source, choosing measures (e.g., capacityUnitMs, durationMs, throttlingDelayMs, status), and scoping by capacity or workspace to prevent alert storms. The article also explains saving and managing the resulting activator rule, helping organizations operationalize capacity observability.

  https://learn.microsoft.com/en-us/fabric/real-time-hub/set-alerts-fabric-capacity-operation-events

- **Fabric Planning Tutorial: Set Up Your Environment**

  Introduced the first tutorial in the Fabric Planning series focused on environment setup. It outlines prerequisites and guides you to import the sample semantic model, create a Fabric SQL database for writeback, and build an initial planning sheet in the Plan app. It also covers connecting the Plan app to your database and orienting users to the planning interface, accelerating onboarding for planning scenarios.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-tutorial/planning/tutorial-0-introduction

## Major Changes

- **Fabric data agent example with the AdventureWorks dataset (preview)**

  Replaced deprecated OpenAI Assistants API guidance with the MCP endpoint to align with current platform direction. Added a new Python section that shows installing the MCP SDK and includes an end-to-end async example to authenticate, discover tools, invoke them, and handle results. The notes clarify the retirement of the Assistants API and explain that conversation state must be managed by the caller. This update ensures developers use supported interfaces and understand conversation management responsibilities.

  https://learn.microsoft.com/en-us/fabric/data-science/data-agent-end-to-end-tutorial

- **Use the Office 365 Outlook activity to send an email with Outlook**

  Expanded authentication guidance to include User OAuth, Workspace Identity, and Service Principal, with setup steps for Microsoft Entra ID and Graph permissions and governance considerations. Updated limitations by removing outdated CI/CD and WI/SPN restrictions and adding that Purview sensitivity labels are not supported for sent emails. These changes enable more secure and flexible authentication choices and clarify current constraints for compliance scenarios.

  https://learn.microsoft.com/en-us/fabric/data-factory/outlook-activity

- **Secure Your Cosmos DB Database**

  Significantly broadened security guidance with a Zero Trust foundation and new sections for network security, data protection, logging and monitoring, governance, and backup and recovery. It details private link scope, encryption defaults and CMK limits, securing mirrored OneLake data, and auditing practices. Identity and access content now covers managed identities, Entra authentication, execution identities for notebooks, and workspace identity limitations. This provides a more complete blueprint for securing Cosmos DB in Fabric, including clarity on what is and isn’t supported today.

  https://learn.microsoft.com/en-us/fabric/database/cosmos-db/security

- **Microsoft Fabric for US Government GCC High customers (preview)**

  Marked the article as preview, added region availability (US Gov Virginia and Texas), and reworked feature availability per workload. It enumerates unsupported capabilities in public preview (for example, Private Link, CMK, outbound access protection, certain mirroring sources, and various platform features) and clarifies partial support areas. This helps government customers plan deployments with accurate expectations and understand current limitations during preview.

  https://learn.microsoft.com/en-us/fabric/enterprise/us-government-community-cloud-high

## Moderate Changes

- **Add and manage an event source in an eventstream**

  Generalized wording so the listed sources apply to all eventstreams, not just those with enhanced capabilities. This reduces confusion and reflects the current, broader support surface.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/add-manage-eventstream-sources

- **Create an eventstream in Microsoft Fabric**

  Removed references to enhanced vs. standard capabilities and related UI instructions, presenting a mode-agnostic introduction. This simplifies setup for new users and aligns the article with the unified eventstream experience.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/create-manage-an-eventstream

- **Enrich events with reference data in Fabric Eventstreams (Preview)**

  Updated prerequisites to no longer require enhanced-capability eventstreams; any eventstream with at least one source and destination now qualifies. This lowers the barrier to using reference data enrichment.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/enrich-events-with-reference-data

- **Microsoft Fabric disaster recovery experience specific guidance**

  Added detailed disaster recovery steps for the Fabric Migration Assistant for SQL Database and clarified recovery approaches across many experiences. The guidance emphasizes manual re-creation where needed, leveraging Git integration, and understanding failover behaviors and limitations. This strengthens operational readiness and reduces recovery time during incidents.

  https://learn.microsoft.com/en-us/fabric/security/experience-specific-guidance

- **What is a lakehouse in Microsoft Fabric?**

  Added a note that lakehouses without schema have a 10 GB metadata cap, with guidance to mitigate failures by enabling schema, trimming models, or splitting them. This helps prevent deployment issues and aids capacity planning.

  https://learn.microsoft.com/en-us/fabric/data-engineering/lakehouse-overview

- **Git integration and deployment pipelines for machine learning experiments and models (preview)**

  Clarified that Git tracks only artifact metadata, while experiment runs and model versions remain in workspace storage and aren’t versioned or promoted. The update explains lifecycle flow, representation details (including Logical ID), single-branch connection per workspace, and deployment behavior and limitations. This helps teams design promotions and dependencies correctly across environments.

  https://learn.microsoft.com/en-us/fabric/data-science/machine-learning-artifacts-git-deployment-pipelines

- **Overview of Microsoft Fabric eventstreams**

  Removed “Enhanced capabilities” references and clarified that sources and transformations are broadly supported. The article also notes that transformations work for all destinations, with derived streams bridging certain cases. This streamlines guidance and reflects the unified feature set.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/overview

- **Use R for Apache Spark**

  Updated Notebook utilities naming from MSSparkUtils to NotebookUtils and adjusted examples to use notebookutils.fs.help() directly. It also clarifies R notebook support, reducing friction for R users.

  https://learn.microsoft.com/en-us/fabric/data-science/r-overview

- **Secure Your Data Factory in Microsoft Fabric Deployment**

  Introduced a Zero Trust statement and consolidated identity and access guidance to encourage workload separation and role-based governance. Governance and compliance guidance now directs users to the OneLake catalog’s Govern tab, and backup/recovery emphasizes Git integration and DR planning. This provides clearer, more actionable security posture guidance.

  https://learn.microsoft.com/en-us/fabric/data-factory/secure-data-factory-in-microsoft-fabric

- **Supported scenarios and limitations for workspace-level private links**

  Added Activator support details and documented ingestion behavior with tenant-level and workspace-level private links. It clarifies that Activator cannot ingest from Eventstream when private links are enabled. This helps architects plan secure event ingestion paths without unexpected gaps.

  https://learn.microsoft.com/en-us/fabric/security/security-workspace-level-private-links-support

- **Semantic functions**

  Clarified that in Fabric Runtime 1.2 (Spark 3.4)+, semantic link and built-in semantic functions are included by default, removing the need to install a separate package. Users should still use pip to update SemPy. This reduces setup steps and ensures access to the latest capabilities. 

  https://learn.microsoft.com/en-us/fabric/data-science/semantic-link-semantic-functions