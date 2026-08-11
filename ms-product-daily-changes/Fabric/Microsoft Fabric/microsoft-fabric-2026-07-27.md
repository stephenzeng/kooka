# Microsoft Fabric
**Date created:** 2026-07-27 UTC  
**Tags:** Administration, Analytics, Monitoring  

## New Articles

- **Mirror Azure Monitor Data in Microsoft Fabric (Preview)**

  Introduced an overview for mirroring Azure Monitor Log Analytics data in Fabric without replicating storage, enabling real-time analytics on the same Delta Lake used by Azure Monitor. Clarifies supported analytics paths, including Eventhouse/KQL for real-time dashboards and OneLake shortcuts into Lakehouse for Spark and Power BI. Details architecture, security and permissions, and authentication options, and explains how Azure RBAC and Fabric permissions relate. Outlines preview constraints and a cost model that avoids duplicated storage, with links to setup and next steps.

  https://learn.microsoft.com/en-us/fabric/mirroring/catalog-mirroring/azure-monitor

- **Troubleshoot the Mirror Azure Monitor Feature in Fabric (Preview)**

  Added a troubleshooting guide covering connection errors, table discovery issues, data freshness expectations, and lifecycle status indicators with suggested fixes. Highlights preview limitations, system column omissions, and known authentication workarounds (for workspace identity), plus guidance for OneLake/Lakehouse shortcut issues.

  https://learn.microsoft.com/en-us/fabric/mirroring/catalog-mirroring/azure-monitor-troubleshoot

- **Tutorial: Configure the Mirror Azure Monitor Feature in Fabric (Preview)**

  Provides step-by-step instructions to configure a mirrored Azure Monitor item, including prerequisites, authentication options, and table selection. Shows how to access data through the Eventhouse endpoint with KQL, create real-time dashboards and alerts, and expose data to Lakehouse for Spark and Power BI scenarios. Explains preview behaviors (no backfill, initial delays), offers troubleshooting pointers, and includes cleanup steps and related links.

  https://learn.microsoft.com/en-us/fabric/mirroring/catalog-mirroring/azure-monitor-tutorial

- **Best Practices and Supported Date Formats for Time Intelligence Hierarchies**

  Introduces best practices for automatic time intelligence detection, including detection precedence and recommended import practices. Details supported hierarchy levels and label formats, composite labels, and valid/invalid patterns to ensure reliable detection and ordering. Includes troubleshooting advice for common issues such as missing members, parsing ambiguities, and two‑digit years.

  https://learn.microsoft.com/en-us/fabric/iq/plan/resources/best-practices/time-intelligence

## Moderate Changes

- **Create a OneDrive or SharePoint shortcut**

  Corrected the Microsoft Graph sites endpoint in the PowerShell sample by adding the required slash after the domain and clarified how to derive the SITE_NAME from different SharePoint URL patterns. These updates reduce setup errors and make the shortcut creation steps more reliable.

  https://learn.microsoft.com/en-us/fabric/onelake/shortcuts/create-onedrive-sharepoint-shortcut

- **Explore Fabric capacity overview events in Fabric Real-Time hub**

  Updated the Summary events table by renaming categories and clarifying descriptions to better reflect capacity consumption: “Kusto” is now “Eventhouse,” and “OneRiver” is now “Azure, Fabric, and Business events.” This improves interpretation of capacity usage for Eventhouse/KQL workloads and event-driven operations.

  https://learn.microsoft.com/en-us/fabric/real-time-hub/explore-fabric-capacity-overview-events