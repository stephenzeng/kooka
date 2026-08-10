# Microsoft Fabric
**Date created:** 2026-07-22 UTC  
**Tags:** Administration, Agent, AI, Analytics, Automation, Governance, Monitoring, Other, Security  

## New Articles

- **Explore the Add Data Page in Fabric Real-Time Hub**

  Introduced a conceptual guide to the Add data page, outlining how to start from Quick start, Azure, and Diagnostics tabs to connect sources. Describes supported Azure and CDC sources and how connections create eventstreams surfaced on Streaming data. Provides links to related Real-Time hub pages to help users progress from connection to monitoring.

  https://learn.microsoft.com/en-us/fabric/real-time-hub/add-data-page

- **Explore the Azure Events Page in Real-Time Hub**

  Introduced the Azure events page with guidance on discovering and subscribing to Azure-originated events via event streams. Explains how to route events to destinations and set alerts or notifications, helping teams operationalize Azure event data.

  https://learn.microsoft.com/en-us/fabric/real-time-hub/azure-events-page

- **Explore the Business Events Page in Real-Time Hub**

  Added a conceptual article explaining business events, how they differ from system events, and how to define, publish, discover, and consume them. Highlights key actions such as managing schemas and setting alerts so organizations can operationalize user-defined event signals.

  https://learn.microsoft.com/en-us/fabric/real-time-hub/business-events-page

- **Date Functions: Create, Format, and Convert Dates**

  Documented new planning date functions for creating, formatting, and converting dates, including Excel serial conversions. Provides syntax and examples to speed up modeling tasks and ensure consistent date handling across scenarios.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-reference-formulas/date-functions/create-format-convert-dates

- **Explore the Event Schema Registry Page in Real-Time Hub**

  Added documentation for the Event schema registry page to help users search, filter, and manage event schemas. Covers key columns, endorsement, and actions to streamline schema governance across workspaces.

  https://learn.microsoft.com/en-us/fabric/real-time-hub/event-schema-registry-page

- **Date Functions: Extract Date Components and Find Start and End Dates**

  Introduced functions to extract day, month, year and to compute period starts and ends (week, month, quarter, year). Provides examples and references to accelerate time-based calculations in planning workflows.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-reference-formulas/date-functions/extract-components-start-end-dates

- **Explore the Fabric Events Page in Real-Time Hub**

  Added a conceptual page describing Fabric system events, how to discover and subscribe to workspace events, and how to route or alert on them. Guides users to next steps for broader event coverage, improving visibility into Fabric activities.

  https://learn.microsoft.com/en-us/fabric/real-time-hub/fabric-events-page

- **IBCS Area and Line Charts to Visualize Trends**

  Published a how-to guide for configuring IBCS line and area charts, including comparison series and deviation lines. Provides step-by-step configuration, stacking options, and color customization to standardize trend visualizations.

  https://learn.microsoft.com/en-us/fabric/iq/plan/intelligence-ibcs/how-to-configure-ibcs-line-area-charts

- **Date Functions: Perform Date Calculations**

  Added reference coverage for date arithmetic and differences, including business days and period ranges. Offers clear syntax and practical examples to simplify forecasting and calendar logic in planning models.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-reference-formulas/date-functions/perform-date-calculations

- **Pipeline Canvas in Fabric Data Factory**

  Introduced a comprehensive guide to the pipeline canvas, covering layout, activity nodes, dependencies, nested activities, and navigation. Documents an updated canvas experience for better scalability and editing, with steps to enable or disable it.

  https://learn.microsoft.com/en-us/fabric/data-factory/pipeline-canvas-experience

- **Explore the Streaming Data Page in Real-Time Hub**

  Added a detailed overview of the Streaming data page, including common tasks, Microsoft sources, samples, and learning resources. Defines stream and KQL table actions (such as preview, endorse, anomaly detection, and Copilot-assisted tasks) to accelerate real-time workflows.

  https://learn.microsoft.com/en-us/fabric/real-time-hub/streaming-data-page

## Major Changes

- **PostgreSQL database connector overview**

  Expanded Dataflow Gen2 capabilities from source-only to both source and destination for PostgreSQL. Updated the support matrix and added a gateway requirement note specifying the June 2026 on-premises data gateway (version 3000.322) or later for destination scenarios via the gateway.

  https://learn.microsoft.com/en-us/fabric/data-factory/connector-postgresql-overview

- **Get Started With Fabric Real-Time Hub**

  Reworked the article from a step-by-step UI walkthrough to a streamlined conceptual overview focused on key hub pages. Added prerequisites, clarified differences between business and system events, and linked to focused topics for deeper guidance. This helps readers quickly understand the hub and navigate to task-specific instructions.

  https://learn.microsoft.com/en-us/fabric/real-time-hub/get-started-real-time-hub

- **Tenant settings index**

  Introduced several new tenant settings for apps and operations agents, including anonymous access for public Fabric Apps (preview) and observability routes to Agent 365 and Microsoft Foundry. Added insights for operations agents to summarize events and improve transparency. These settings enhance governance, monitoring, and secure data access at scale.

  https://learn.microsoft.com/en-us/fabric/admin/tenant-settings-index

## Moderate Changes

- **Anomaly detection in Real-Time Intelligence (Preview)**

  Added support for creating anomaly detectors on Eventhouse shortcut tables, extending coverage to external and federated sources. This reduces data duplication and enables the same modeling and monitoring experiences as native tables.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/anomaly-detection

- **Assign a workspace to a Microsoft Fabric deployment pipeline**

  Added a limitation effective November 1, 2026: users lacking read-write permissions on items due to sensitivity labels and protection policies will be blocked from certain stage operations. Aligns deployment behavior with contributor permission requirements and links to protection policy guidance.

  https://learn.microsoft.com/en-us/fabric/cicd/deployment-pipelines/assign-pipeline

- **Connector overview**

  Updated the support matrix to show full Dataflow Gen2 support for the PostgreSQL connector. This signals readiness for broader use in both source and destination scenarios.

  https://learn.microsoft.com/en-us/fabric/data-factory/connector-overview

- **Set up your PostgreSQL database connection**

  Added a requirement for the June 2026 on-premises data gateway update (version 3000.322) or later when using PostgreSQL as a Dataflow Gen2 destination via the gateway. This ensures compatibility for write scenarios.

  https://learn.microsoft.com/en-us/fabric/data-factory/connector-postgresql

- **Integrate Direct Lake security**

  Clarified how Direct Lake over SQL analytics endpoints enforces OLS/CLS and when queries fall back to DirectQuery for RLS and views, including failure cases when fallback is disabled. Added references to evaluation details to help diagnose errors and choose the right mode.

  https://learn.microsoft.com/en-us/fabric/fundamentals/direct-lake-security-integration

- **Basic concepts in Git integration**

  Added a note that starting November 1, 2026, users without read-write permissions on workspace items can’t use Git integration. Calls out potential loss of access due to sensitivity labels and links to Information Protection guidance.

  https://learn.microsoft.com/en-us/fabric/cicd/git-integration/git-integration-process

- **Entity type details in ontology (preview)**

  Removed the tenant-level Graph enablement prerequisite, requiring only the Ontology item (preview) to be enabled. Simplifies setup for trying ontology features.

  https://learn.microsoft.com/en-us/fabric/iq/ontology/how-to-view-entity-type-details

- **What is ontology (preview)?**

  Rewrote the Ontology graph section to describe its relationship to Graph in Microsoft Fabric without a separate IMPORTANT prerequisite. Clarified where to view the graph and how nodes, edges, lineage, and refresh behave.

  https://learn.microsoft.com/en-us/fabric/iq/ontology/overview

- **AI Functions: Transform data at scale with LLMs**

  Clarified runtime guidance and installation steps for pandas AI Functions with Fabric Runtime 2.0, including temporary nest_asyncio usage and notes about future built-in support. Consolidated model defaults across engines, explained async inference with row-level isolation, and removed a separate performance section to streamline guidance.

  https://learn.microsoft.com/en-us/fabric/data-science/ai-functions/overview

- **Configure display and formatting settings in PowerTable**

  Added a feature preview note to indicate the functionality is in preview. Helps readers set expectations about availability and potential changes.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-how-to-configure-display-formatting-settings

- **Secure Your Cosmos DB Database**

  Clarified notebook execution identity based on trigger type: interactive runs use the current user, pipeline runs use the last pipeline modifier, and scheduled runs use the schedule owner/updater. Added a link to notebook security context details and emphasized that operations run under the triggering user’s identity.

  https://learn.microsoft.com/en-us/fabric/database/cosmos-db/security

- **The deployment pipelines process**

  Added a policy note that from November 1, 2026, users without read-write permissions on all workspace items can’t deploy to or assign certain stages if items are protected by sensitivity labels with protection policies. Aligns deployment permissions with Information Protection to prevent unauthorized operations.

  https://learn.microsoft.com/en-us/fabric/cicd/deployment-pipelines/understand-the-deployment-process

- **What is workspace monitoring (preview)?**

  Reorganized logging coverage into a single “Available events and logs” table and expanded entries for Data Factory, Real-Time hub, GraphQL, Mirroring, and semantic models. Shifted guidance from “install” to “enable,” making it easier to understand how to activate monitoring.

  https://learn.microsoft.com/en-us/fabric/fundamentals/workspace-monitoring-overview

## Minor Changes