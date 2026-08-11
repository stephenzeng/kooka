# Microsoft Fabric
**Date created:** 2026-07-31 UTC  
**Tags:** AI, Agent, Analytics, Governance, Monitoring  

## New Articles

- **Get started with data governance**

  Introduced a step-by-step guide to establish governance in Microsoft Fabric, starting with the OneLake catalog. The guidance covers organizing your estate with domains and tags; classifying and protecting sensitive data with sensitivity labels, protection policies, and DLP (Purview-licensed). It explains tracing dependencies via lineage and impact analysis, and securely sharing OneLake data across tenants. It also outlines how to extend governance with metadata scanning, Defender for Cloud Apps controls, auditing, and standards compliance, including prerequisites and licensing notes.

  https://learn.microsoft.com/en-us/fabric/governance/get-started-with-fabric-governance

- **Maximize or Minimize a Target Value**

  Added a how-to guide for using Optimize in Fabric Plan to maximize or minimize a target value based on calculated measures. It walks through selecting a target, setting the objective, choosing editable variables, applying constraints, reviewing results, and applying updates, with an example that maximizes Profit per unit by adjusting projections. The article also covers optimizing at parent (aggregate) levels, including proportional distribution to child rows and honoring locked cells.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-optimize/planning-how-to-maximize-minimize-target-value

## Moderate Changes

- **Data Factory limitations overview**

  Removed a limitation that warned of intermittent failures when consuming Dataflow Gen2 output via the Dataflows connector and the workaround to route through Lakehouse or Warehouse. This update signals improved reliability in the underlying APIs and simplifies downstream consumption guidance.

  https://learn.microsoft.com/en-us/fabric/data-factory/data-factory-limitations

- **End-to-end tutorials in Microsoft Fabric**

  Updated the Data Science tutorial to use a 10,000-customer banking dataset and focus on predicting customer churn, replacing the prior taxicab trip duration scenario. This refresh aligns the tutorial with a more common business use case.

  https://learn.microsoft.com/en-us/fabric/fundamentals/end-to-end-tutorials

- **Create OneLake shortcuts in a KQL database**

  Expanded guidance on automatic schema sync for eventhouse database shortcuts, distinguishing between database-level sync (adds/removes subitems when Include all subitems is selected) and shortcut table-level sync (column add/delete/rename and type changes by default). Clarified how to disable shortcut table schema sync via KQL (AutoUpdateSchema=false) and reiterated that consumers only see explicitly shared subitems.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/onelake-shortcuts

- **Create and configure operations agents**

  Removed the section on monitoring agent activity, including activity log details, event types, timestamps, and the operation details page. Users should refer to alternative monitoring guidance where available.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/operations-agent

- **Operations Agent Capacity and Billing**

  Updated the billing table to rename the Azure metric for Investigation agent reasoning to “Operations agents autonomous reasoning capacity usage CU” and added a capacity unit rate of 0.46 CUs per vCore hour. This change clarifies metering terminology and expected cost calculations.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/operations-agent-billing

- **What's new in Microsoft Fabric?**

  Added a preview feature entry for Change event streaming (CES) in Fabric SQL database, enabling row-level DML capture and near real-time publishing to Fabric Eventstream or Azure Event Hubs as CloudEvents, with an overview link. Also added a July 2026 timeline entry under SQL database updates.

  https://learn.microsoft.com/en-us/fabric/fundamentals/whats-new