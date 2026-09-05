# Microsoft Fabric
**Date created:** 2026-09-05 UTC  
**Tags:** Analytics, Configuration, Get Started, Governance, Guidance, Monitoring, Troubleshooting  

## New Articles

- **Optimize Data Input Measures in Fabric Planning**

  Introduced a step-by-step tutorial for using the Optimizer in Fabric Planning to reach target outcomes by adjusting input measures. Guides you to build a Gross Profit sheet, create editable inputs from Sales Plan and COGS, and define a Gross Profit formula. Explains how to configure objectives, variables, and optional constraints, run optimization to hit a $12.5M goal, apply results, and compare against the baseline.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-tutorial/planning/tutorial-3-optimizer

- **Get Started with PowerTable and Create a Data App in Plan**

  Added an end-to-end tutorial for building an asset management data app with PowerTable. Covers creating a Fabric SQL database and Plan item, importing Excel data into assets, employees, and locations, and configuring columns, lookups, conditional formatting, and formulas. Details data operations like inline edits, form-based inserts, bulk updates, change review, and additional imports to accelerate app creation.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-tutorial/powertable/tutorial-7-get-started-with-powertable

## Major Changes

- **Fabric data agent example with the AdventureWorks dataset (preview)**

  Streamlined the tutorial by removing detailed Copilot in Power BI publishing/usage steps and screenshots. The article now states that once published, the data agent can be consumed as a Model Context Protocol (MCP) server. This reduces ambiguity and directs users to the supported integration model going forward.

  https://learn.microsoft.com/en-us/fabric/data-science/data-agent-end-to-end-tutorial

- **Data agent as Model Context Protocol server**

  Removed preview status to reflect general availability and expanded setup guidance. Clarified client requirements and authentication, noting that dynamic client registration and client identity metadata aren’t supported and clients must attach a Fabric token. Added support details for long-running requests via the MCP tasks extension, including task IDs, polling, and cancellation, and indicated orchestrators are available without preview labels to aid robust production integrations.

  https://learn.microsoft.com/en-us/fabric/data-science/data-agent-mcp-server

- **Use prebuilt Text Analytics with REST API**

  Updated REST and SynapseML examples to use api-version 2024-11-01 for analyze-text operations, aligning samples to current service behavior. Introduced a new PII detection section using api/model version 2026-05-01, with sample requests, responses, and redactedText handling. These changes improve compatibility and provide clearer guidance for sensitive data processing.

  https://learn.microsoft.com/en-us/fabric/data-science/ai-services/how-to-use-text-analytics

- **Use Azure Translator in Foundry Tools with REST API**

  Clarified supported Translator API versions and the limits of the prebuilt Fabric endpoint. Translation remains on Translator Text API v3.0, while transliteration and supported-languages move to API version 2026-06-06 with a new request/response schema and migration guidance. Removed obsolete endpoints and streamlined samples to reduce integration errors during the transition.

  https://learn.microsoft.com/en-us/fabric/data-science/ai-services/how-to-use-text-translator

- **Sharing Microsoft Fabric Maps**

  Refocused the article on two governed distribution methods: direct sharing and org apps, removing Real-Time Dashboard guidance. Rewrote the comparison to highlight audience, permissions, resharing, governance, and revocation trade-offs, helping teams choose the right approach. Updated navigation to steer readers to direct access and org apps content for clearer deployment paths.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/map/sharing-maps

- **Spark connector for SQL databases**

  Removed preview status to mark GA and added guidance on timestamp mapping to SQL datetime2 and precision considerations. Expanded read/write scenarios with Python and Scala samples, including running custom queries and clarifying overwrite behavior with recommendations to use option("truncate", true). Added troubleshooting for bulk write failures (SQLServerException 4815) with concrete fixes, improving reliability in production pipelines.

  https://learn.microsoft.com/en-us/fabric/data-engineering/spark-sql-connector

## Moderate Changes

- **Use Foundry Tools in Fabric**

  Added explicit API-version guidance for Azure AI Language and Translator usage in Fabric. Clarified REST examples for Language (2024-11-01; PII detection using 2026-05-01) and Translator (v3.0 for translation; 2026-06-06 for transliteration and supported languages) and flagged breaking schema changes with migration references. This helps teams avoid version mismatches and plan updates.

  https://learn.microsoft.com/en-us/fabric/data-science/ai-services/ai-services-overview

- **What is Copilot in Fabric?**

  Updated enablement guidance to note Copilot is on by default for paid Fabric capacities (F2+), with admin steps to review tenant and capacity settings and control access. Clarified how agent conversation history is stored within the Azure security boundary, retention (28 days), regional alignment, and user deletion options, improving governance and privacy posture.

  https://learn.microsoft.com/en-us/fabric/fundamentals/copilot-fabric-overview

- **Create a Real-Time Dashboard**

  Clarified behavior for Fabric Maps tiles, including inherited changes from source items and editor limits to layout and sizing. Documented viewer interactions (pan/zoom, selection, basemap/layer controls, and unlocked filters), locked filter behavior, prerequisites for adding tiles, and error handling when source maps are missing. This reduces confusion and streamlines dashboard building and viewing.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/dashboard-real-time-create

- **Enable monitoring in your workspace**

  Expanded and structured prerequisites, adding a requirement that the “Users can create Fabric items” tenant setting must be enabled for monitoring to appear and function. Explained behavior when disabled and clarified capacity requirements to improve setup success and troubleshooting.

  https://learn.microsoft.com/en-us/fabric/fundamentals/enable-workspace-monitoring

- **Fabric planning tutorial part 1: Allocation and collaboration**

  Added guidance to configure and verify a two-level approval workflow with role-based approvers, reset-on-rejection, and Teams notifications. Described approval status columns and example submission flows, helping teams operationalize governed plan changes.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-tutorial/planning/tutorial-1-allocation-collaboration