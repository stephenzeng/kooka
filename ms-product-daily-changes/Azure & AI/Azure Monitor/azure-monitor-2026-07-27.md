# Azure Monitor
**Date created:** 2026-07-27 UTC  
**Tags:** AI, Agent, Analytics, Monitoring, Programming  

## New Articles

- **Mirror Azure Monitor Data in Microsoft Fabric (Preview)**

  Introduces a new preview capability that mirrors Azure Monitor Logs into Microsoft Fabric without copying data, enabling analytics over operational telemetry alongside business data in OneLake. Explains the architecture using OneLake shortcuts to Delta Parquet with dual access paths: Eventhouse for KQL/dashboards/operations and Lakehouse for Spark and Power BI. Clarifies governance continuity via Azure Monitor retention policies and distinguishes this approach from DCR-based direct-to-Fabric ingestion. Outlines cost implications—no extra ingestion costs, with Fabric billed for query capacity.

  https://learn.microsoft.com/en-us/azure/azure-monitor/fundamentals/monitor-cross-domain-fabric

## Major Changes

- **Add and Modify OpenTelemetry in Application Insights**

  Added guidance to capture end-user feedback for GenAI agents and send it to Application Insights as custom events via OpenTelemetry logs using a reserved event name. Defined a standardized attribute schema for feedback (evaluation metadata, score, explanation, correlation IDs, and provider/actor) and highlighted PII handling considerations. Provided implementation examples for ASP.NET Core, .NET, Node.js, and Python with pointers for Java emitters, plus a Kusto example to analyze feedback in customEvents and correlate it to traces. These updates help teams measure AI quality, trace outcomes end-to-end, and operationalize feedback-driven improvements.

  https://learn.microsoft.com/en-us/azure/azure-monitor/app/opentelemetry-add-modify