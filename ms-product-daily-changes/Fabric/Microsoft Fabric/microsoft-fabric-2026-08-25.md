# Microsoft Fabric
**Date created:** 2026-08-25 UTC  
**Tags:** Best Practices, Configuration, Get Started, Guidance, Monitoring, Performance, Security  

## New Articles

- **Get Started with Fabric IQ**

  Introduced a new getting-started guide that explains Fabric IQ’s purpose and three-layer model spanning OneLake data, Power BI semantic models, and ontologies. The article maps common scenarios to capabilities such as ontology, semantic models, plan, graph, data agent, operations agent, and Microsoft 365 Copilot integrations, helping readers choose the right entry points. It also links to end-to-end tutorials, outlines required tenant settings for ontology and data agent, and provides related references to streamline onboarding.

  https://learn.microsoft.com/en-us/fabric/iq/get-started-with-fabric-iq

## Moderate Changes

- **Configure and manage Automated Table Statistics in Fabric Spark**

  Updated guidance consolidates configuration across Spark SQL, PySpark, and Scala and simplifies disabling by setting values to false. It adds best practices for tables with deletion vectors (use regular OPTIMIZE/REORG with purge and keep statistics injection disabled between maintenance), clarifies differences between Spark catalog statistics and Fabric extended statistics, and shifts recomputation/removal examples to Python using StatisticsStore, including steps after schema changes.

  https://learn.microsoft.com/en-us/fabric/data-engineering/automated-table-statistics

- **Mirroring Azure Database for MySQL (preview)**

  Clarified support to include only publicly accessible servers and those using Private Link/private endpoints; virtual network–enabled servers and high availability configurations aren’t supported. Network requirements were updated accordingly, and prior guidance about virtual network or on-premises data gateways for VNet scenarios was removed to prevent misconfiguration.

  https://learn.microsoft.com/en-us/fabric/mirroring/azure-database-mysql

- **Limitations in Microsoft Fabric mirrored databases from Azure Database for MySQL (preview)**

  Updated the support matrix to allow only MySQL 8.0 (8.0.x from 8.0.21) and explicitly exclude MySQL 8.4. Network isolation guidance now limits connectivity to Private Link/private endpoints, removing support for virtual network or VNET data gateways.

  https://learn.microsoft.com/en-us/fabric/mirroring/azure-database-mysql-limitations

- **Tutorial: Create a mirrored database from Azure Database for MySQL in Microsoft Fabric (preview)**

  Updated the tutorial to reinforce that only MySQL 8.0 is supported and to require Private Link/private endpoints for connectivity. It clarifies that VNet/on-prem data gateways and HA configurations aren’t supported, and adjusts setup steps to select no data gateway while maintaining encrypted connections.

  https://learn.microsoft.com/en-us/fabric/mirroring/azure-database-mysql-tutorial

- **Enable workspace monitoring for eventstreams (preview)**

  Marked the feature as preview with an added notice and updated wording. Expanded cross-references by adding a link to the known limitations to set expectations for current behavior.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/enable-fabric-workspace-monitoring

- **Eventstream Workspace Monitoring Known Limitations (preview)**

  Replaced inline notices with a shared preview include for consistency and easier maintenance. Removed the temporary “feature disabled” notice and its link, while keeping the limitations content intact.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/fabric-workspace-monitoring-known-limitations

- **Create and share a cloud connection for a semantic model**

  Clarified the steps to make a Direct Lake semantic model compatible with plan and separated role requirements for better readability. Added a note instructing users to select a Power BI Semantic Model connection and reuse the connection created earlier when creating a plan, reducing setup errors.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-how-to-create-semantic-model-connection

- **Query Eventstream Monitoring Data with KQL (preview)**

  Designated the capability as preview and specified prerequisites: enable workspace monitoring, turn on Log Eventstream activity, and republish eventstreams to start sending data. Clarified that tables are created in the monitoring database and added a link to known limitations.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/query-fabric-workspace-monitoring-data

- **Create and use managed private endpoints in Microsoft Fabric**

  Added instructions for creating a managed private endpoint to Azure API Management via the Fabric REST API, including prerequisites, supported tiers, required request payload, and the note that only the Gateway subresource supports inbound Private Link. Included portal approval and verification steps, and updated the resource ID reference table to include Azure API Management (REST API only).

  https://learn.microsoft.com/en-us/fabric/security/security-managed-private-endpoints-create