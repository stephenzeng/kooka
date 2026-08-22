# Microsoft Fabric
**Date created:** 2026-08-22 UTC  
**Tags:** Analytics, Best Practices, Configuration, Get Started, Governance, Guidance, Identity, Monitoring, Security  

## New Articles

- **Google Lakehouse runtime catalog mirroring in Microsoft Fabric**

  Introduced an overview of mirroring Google Lakehouse runtime catalogs, explaining that only metadata is mirrored (no data movement) with expected propagation latency. Detailed the created mirrored catalog item and an auto-generated read-only SQL analytics endpoint, and outlined supported analytics experiences including T-SQL and Direct Lake. Added end-to-end connection and authentication guidance using Google Cloud Workload Identity Federation with Microsoft Entra OIDC, including required roles and provider settings. Clarified metadata sync behavior, default auto-sync for future tables, and selection rules, with links to setup and limitations.

  https://learn.microsoft.com/en-us/fabric/mirroring/catalog-mirroring/google-lakehouse-runtime

- **Limitations in Microsoft Fabric catalog mirroring for Google Lakehouse runtime catalog**

  Documented hard limits and constraints for Google Lakehouse runtime catalog mirroring, including support only for Apache Iceberg V2 tables with Parquet data and read-only behavior in Fabric. Explained that tables are auto-converted to Delta Lake with existing conversion caveats, access occurs over public internet, and limits apply (for example, up to 500 tables and 1 MB Iceberg metadata.json). Clarified security and identity requirements for Workload Identity Federation and noted that fine-grained Google Cloud access controls aren’t enforced in Fabric—use OneLake security instead. Listed unsupported features such as database/metastore/Iceberg views and provided references to related setup content.

  https://learn.microsoft.com/en-us/fabric/mirroring/catalog-mirroring/google-lakehouse-runtime-limitations

- **Tutorial: Configure mirrored Google Lakehouse runtime catalog**

  Provided a step-by-step tutorial to configure a mirrored Google Lakehouse runtime catalog, from prerequisites to verification. Guided users through setting up Workload Identity Federation in Google Cloud, assigning required roles, configuring storage access, and collecting connection parameters. Walked through creating the mirrored catalog in Fabric, enabling sync options, querying via the SQL analytics endpoint, and creating lakehouse shortcuts to mirrored tables. Included links to conceptual guidance and limitations for deeper context.

  https://learn.microsoft.com/en-us/fabric/mirroring/catalog-mirroring/google-lakehouse-runtime-tutorial

- **Blend measures using Infobridge**

  Added a how-to guide for blending measures across planning sheets and Infobridge queries to enrich planning models. Demonstrated adding measures from other sheets, building an Infobridge query, and composing a visual blend measure with custom aggregation. Included screenshots and step-by-step instructions to speed adoption.

  https://learn.microsoft.com/en-us/fabric/iq/plan/infobridge-how-to-blend-measures

- **Scenario planning in Microsoft Fabric**

  Introduced core concepts for scenario planning, distinguishing the Base plan from independent scenarios. Explained how to simulate changes, compare outcomes via variance, and manage scenarios with locking, resets, bulk edits, and pivots. Covered applying scenario values back to Base with governance via Writeback and scenario security, along with a recommended step-by-step process. Highlighted when to use scenarios and the decision-making benefits they unlock.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-concept-scenario-planning

## Major Changes

- **Collect Apache Spark applications logs and metrics using Azure Event Hubs**

  Added certificate-based authentication via Microsoft Entra service principal using Azure Key Vault, including detailed prerequisites and a complete Spark properties example. Clarified configuration specifics such as using the namespace FQDN as hostName, the Event Hub name as entityPath, and the distinction between the signed-in user retrieving the certificate and the service principal sending to Event Hubs. Updated the configuration table to refine certificate-related fields and Key Vault requirements to reduce setup errors and strengthen security.

  https://learn.microsoft.com/en-us/fabric/data-engineering/azure-fabric-diagnostic-emitters-azure-event-hub

- **Enable workspace monitoring for eventstreams (preview)**

  Reframed the setup as a two-step process: enable workspace-level monitoring by creating an Eventhouse monitoring database and then enable monitoring at the eventstream level. Added a new section with item-level settings to toggle monitoring on, and expanded UI-driven guidance for workspace enablement. Removed outdated notes about temporary disablement and the need to republish existing eventstreams, reflecting simplified and current behavior.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/enable-fabric-workspace-monitoring

- **Eventstream workspace monitoring overview**

  Removed the preview designation and significantly expanded the monitoring reference. Added emission frequencies, a comprehensive set of common base dimensions, and detailed schemas for EventStreamNodeStatus, EventStreamMetrics, and EventStreamErrorMetrics with clear metric names, aggregations, units, and meanings. Streamlined related content by consolidating links and removing the separate monitoring tables page, improving discoverability and implementation clarity.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/fabric-workspace-monitoring

- **Create Forecasts Using Predictions and Historical Data**

  Substantially expanded the forecasting how-to with an end-to-end P&L scenario and clear task-based sections. Added procedures for building forecasts from historical actuals, zero-based planning, and top-down/bottom-up allocations across hierarchies. Introduced rules for locking values, a richer Predict feature workflow (evaluation mode, seasonality, preview, and apply), and guidance for creating deviation measures between budget and forecast. Updated images and step-by-step instructions to improve execution accuracy and learning.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-forecasting/planning-how-to-build-forecasts

## Moderate Changes

- **Collect your Apache Spark applications logs and metrics using Azure Storage account**

  Introduced certificate-based authentication using a Microsoft Entra service principal with Azure Key Vault, with clear prerequisites, required role assignments, and a Spark configuration example. Clarified identity separation for certificate retrieval versus storage access, refined the URI format, and updated parameter guidance to reduce misconfiguration and improve security posture.

  https://learn.microsoft.com/en-us/fabric/data-engineering/azure-fabric-diagnostic-emitters-azure-storage

- **Collect logs and metrics with Azure Log Analytics**

  Expanded certificate-based authentication guidance, including Key Vault setup, public certificate registration on the app, and required user permissions to retrieve the private key. Updated configuration to use the DCR immutable ID and enhanced property descriptions, improving reliability and reducing configuration errors.

  https://learn.microsoft.com/en-us/fabric/data-engineering/data-collector-api-to-log-ingestion-api

- **Azure OpenAI for big data**

  Streamlined instructions to align with the Fabric workflow by updating navigation, simplifying notebook import to Fabric, and directing SynapseML installation to a dedicated guide. Standardized terminology and clarified batching guidance by referencing DataFrame partitions, improving consistency and execution.

  https://learn.microsoft.com/en-us/fabric/data-science/open-ai