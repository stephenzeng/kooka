# Microsoft Fabric
**Date created:** 2026-08-07 UTC  
**Tags:** Administration, Agent, Analytics, Governance, Monitoring, Programming, Security  

## New Articles

- **Anonymous data access in Fabric apps**

  Introduced guidance for enabling anonymous data access in Fabric apps, governed jointly by a tenant setting and data‑model roles. Explained how to define anonymous permissions using the @role('anonymous', ...) decorator with examples for read-only, create-only, and combined scenarios, and how to blend anonymous and authenticated roles with claims-based policies. Provided security best practices (least privilege, field controls, server-side enforcement, validation, monitoring, and testing) and clear steps to enable or disable the feature at app and tenant levels. Included links to related topics to help admins roll out and govern this capability confidently.

  https://learn.microsoft.com/en-us/fabric/apps/anonymous-data-access

- **Visualize Budgets, Forecasts, and Simulations in Fabric Plan**

  Added a concept article showing how to embed planning sheets into intelligence sheets to visualize simulations, budgets, and forecasts on live data. Clarified differences between semantic model measures and live sheet measures, and demonstrated how to blend measures from planning sheets, semantic models, external files, and PowerTable. Highlighted real-time updates to visuals as simulations change and included an FAQ on prerequisites, selecting among multiple planning sheets, editability, and measure types to speed up planning workflows.

  https://learn.microsoft.com/en-us/fabric/iq/plan/infobridge-concept-blend-measures

## Moderate Changes

- **Fabric data agent Python SDK (preview)**

  Updated guidance to migrate data agent querying from the OpenAI Assistants API to the OpenAI Responses API when using the Fabric OpenAI client. Clarified that only querying code paths change—creation, configuration, and publishing remain the same—and provided a sample notebook to streamline migration. This helps ensure compatibility with the latest API model and reduces disruption to existing workloads.

  https://learn.microsoft.com/en-us/fabric/data-science/fabric-data-agent-sdk

- **Fabric operations**

  Added an Operations agent subsection with consumption and billing details, including meters for Operations agent compute, Investigation agent reasoning, and autonomous reasoning. Updated the Real-Time Intelligence overview to include the Operations agent and noted it also consumes the Copilot in Fabric operation for interactive use. This improves cost transparency and planning for teams deploying these capabilities.

  https://learn.microsoft.com/en-us/fabric/enterprise/fabric-operations

- **Operations agent best practices and limitations**

  Clarified limitations: only one data source is supported at a time, and Eventhouse support is limited to regular tables (shortcuts, functions, and materialized views excluded). Renamed and reorganized monitoring guidance to emphasize Ontology monitoring rule constraints, including support for basic property values only and lack of AND-condition support. These updates help teams design reliable monitoring setups and avoid unsupported configurations.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/operations-agent-limitations