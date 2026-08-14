# Microsoft Fabric
**Date created:** 2026-08-14 UTC  
**Tags:** Analytics, Best Practices, Configuration, Get Started, Guidance, Identity, Licensing, Performance, Security, Troubleshooting  

## New Articles

- **Create Row Model using Model Builder**

  Introduced step-by-step guidance for enabling row-based modeling in planning sheets and using Model Builder to structure drivers hierarchically. Explains configuring Data Source, Aggregate, and Formula drivers, including trends and open/closed period aggregation. Provides a worked P&L example mapping leaf rows to semantic model sources and composing formulas such as Operating Profit. Highlights how to analyze driver impacts and run forecasts, scenarios, and simulations with visual examples.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-row-model/how-to-create-row-model

- **Column and Row Identifiers in Plan**

  Added comprehensive reference for Plan formula identifiers to streamline authoring and debugging. Documents time-aware functions, hierarchy navigation, relative references, and array-return behavior with clear syntax, arguments, and examples. Clarifies limitations and layout behaviors so modelers can build robust calculations across rows and columns.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-reference-formulas/identifiers

- **Eventstream for Azure Event Hubs and Stream Analytics users**

  Published migration guidance to consolidate Event Hubs + Stream Analytics workloads into Fabric Eventstream. Compares ingestion parity and expands on Eventstream’s built-in processing (no-code canvas, SQL operator) and DeltaFlow for CDC and schema evolution. Shows how to fan out to multiple Fabric destinations and when to retain Azure services for specialized needs.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/migrate-from-azure-event-hubs-stream-analytics

- **Update Forecast Periods with Reforecasting**

  Introduces the reforecasting approach to seed new forecast periods from a chosen source and apply adjustments such as growth. Outlines the end-to-end process—close, extend the horizon, select target/source, copy values, and adjust—so planners can keep forecasts current. Emphasizes maintaining a continuous forecast horizon and optionally distributing deficits to preserve annual totals.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-concept-reforecasting

- **Microsoft ODBC Driver for Microsoft Fabric Data Engineering on Linux**

  New how-to (Preview) that covers prerequisites, installation, and driver registration on Linux with unixODBC. Provides connection string formats, Microsoft Entra ID authentication options, DSN configuration, and quick-start code for Python, C/C++, and .NET. Includes performance tuning parameters and extensive troubleshooting to speed up connectivity and resolve common errors.

  https://learn.microsoft.com/en-us/fabric/data-engineering/spark-odbc-driver-linux

## Major Changes

- **Experience-specific disaster recovery guidance**

  Expanded disaster recovery instructions for Real-Time Intelligence, adding a dedicated section on event schema sets. Clarifies restoring schema sets first when recreating Business Events and distinguishes what definitions are recoverable versus non-restored elements like publisher registrations and event history. Provides two recovery paths: recommended Git backup-and-restore with validation steps, and manual recreation when Git integration wasn’t configured.

  https://learn.microsoft.com/en-us/fabric/security/experience-specific-guidance

- **Microsoft JDBC Driver for Microsoft Fabric Data Engineering**

  Enhanced guidance to highlight HikariCP integration for efficient connection reuse and updated artifacts to version 1.0.1 for Java 11/17/21. Clarifies HTTP transport settings versus connection pooling and adds a full section on configuring HikariCP with sample code and recommended pool settings. This improves performance practices and simplifies stable, validated connections in production workloads.

  https://learn.microsoft.com/en-us/fabric/data-engineering/spark-jdbc-driver

- **What's new in Microsoft Fabric?**

  Substantially refreshed the What's New page with new GA and Preview items and updates across August 2026. Reflects status changes (for example, Build agent with AI, Fabric Runtime 2.0, and Capacity Overview Events) and replaces or removes superseded entries. Provides up-to-date links and summaries to help readers quickly discover recent capabilities and their impact.

  https://learn.microsoft.com/en-us/fabric/fundamentals/whats-new

## Moderate Changes

- **Anonymous data access in Fabric apps**

  Added a Parameters subsection for the @role decorator, detailing roleName, actions (create/read/update/delete/*), and options (check/include/exclude). This clarifies how to configure anonymous and other roles for precise data operation permissions.

  https://learn.microsoft.com/en-us/fabric/apps/anonymous-data-access

- **Define data permissions**

  Introduced the built-in anonymous role alongside authenticated and updated the roles table with descriptions and usage guidance. Links to the anonymous access article to help determine when and how to enable public access safely.

  https://learn.microsoft.com/en-us/fabric/apps/data-permissions

- **Fabric trial capacity**

  Strengthened onboarding with clear calls to start a free trial, refined quick start language, and clarified steps distinct from becoming a Capacity admin. Expanded FAQs cover production suitability, eligibility limits, and retrial options, plus a new Next steps section to guide activation.

  https://learn.microsoft.com/en-us/fabric/fundamentals/fabric-trial

- **Workspace outbound access protection**

  Extended the supported workloads table for Fabric IQ by adding Data agent with a direct link. This makes the documented coverage consistent across Graph, Operations, and Data agents.

  https://learn.microsoft.com/en-us/fabric/security/workspace-outbound-access-protection-overview