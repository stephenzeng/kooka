# Microsoft Fabric
**Date created:** 2026-09-01 UTC  
**Tags:** Analytics, Best Practices, Billing, Compliance, Configuration, Consumption, Deprecation, Get Started, Governance, Guidance, Licensing, Monitoring, Performance, Security, Troubleshooting  

## New Articles

- **OpenAI as a subprocessor in Microsoft Fabric**

  Introduced guidance for enabling OpenAI-operated models as a Microsoft subprocessor, clarifying when this applies versus Azure OpenAI and the associated governance and contractual considerations. Explains data residency implications, including potential processing outside regional boundaries and unavailability in sovereign clouds. Provides tenant- and capacity-level configuration steps, including scoping and data residency controls, plus current compliance limitations and links to related security/privacy resources.

  https://learn.microsoft.com/en-us/fabric/fundamentals/copilot-openai-subprocessor

- **Add a Markdown Visual to a Real-Time Dashboard**

  Added a step-by-step tutorial to insert and configure a Markdown visual in Real-Time Dashboards. Covers embedding images using GitHub Flavored Markdown, previewing changes, and saving the visual. Includes links to visual gallery, customization guidance, and supported visuals.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/dashboard-markdown-visual

- **Real-Time Dashboard supported data sources**

  Published a reference for all supported data sources in Real-Time Dashboards, including Eventhouse (Fabric KQL database), Azure Data Explorer, and Azure Monitor services. Details how to connect each source via the Add data source flow with specific configuration options. Provides links to overview and creation steps to streamline setup.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/dashboard-supported-data-sources

- **Real-Time Dashboard supported visuals**

  Documented the complete set of visuals supported in Real-Time Dashboards, highlighting dashboard-specific visuals like funnel and heatmap. Provides use cases, descriptions, and example imagery to help choose the right visual. Links to customization and troubleshooting topics to accelerate authoring and maintenance.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/dashboard-supported-visuals

- **Real-Time Dashboard Visual Gallery**

  Introduced a gallery that helps authors select and configure visuals effectively, including layout organization and Copilot-assisted authoring. Details customization options such as colors, axes, legends, aggregation, reference lines, time ranges, and conditional formatting. Highlights specialized visuals (KPI, Time Series, Markdown) with pointers to deeper guidance.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/dashboard-visual-gallery

- **Enrich Events with Reference Data in Fabric Eventstreams**

  Added a concept/how-to article on joining real-time streams with reference data from Lakehouse Delta tables to enrich events. Explains supported sources (native and shortcut-based), optional scheduled refresh, and Join operator configuration (inner and left outer). Includes verification steps, schema outcomes, and key limitations to ensure reliable enrichment.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/enrich-events-with-reference-data

## Major Changes

- **OneLake security roles, permissions, and scopes**

  Substantially restructured the OneLake security model article to center on roles, permissions, and scopes, and clarified deny-by-default behavior and default roles. Added detailed guidance for ReadWrite permissions, including capabilities, limitations (no RLS/CLS for ReadWrite roles), and single-engine enforcement. Expanded coverage of enforcement, inheritance, metadata visibility, table validity, and shortcuts (passthrough vs delegated), plus formalized role evaluation across multiple roles and updated limitations and latency expectations.

  https://learn.microsoft.com/en-us/fabric/onelake/security/data-access-control-model

- **Data security in OneLake**

  Rewrote the OneLake security overview to distinguish control plane (workspace/item roles) from data plane (OneLake security) with a new comparison and when-to-use guidance. Consolidated navigation into task-focused articles and clarified engine enforcement, shortcuts, authentication, audit logs, and networking/encryption. This improves understanding of how access is granted and audited across Fabric and connected services.

  https://learn.microsoft.com/en-us/fabric/onelake/security/get-started-security

- **Retention and recovery in Fabric**

  Updated defaults so item recovery is enabled by default with a minimum three-day retention (previously disabled, minimum seven). Refreshed comparisons, clarified tenant behavior when settings were never configured, and explained that admins can adjust retention (3–90 days) or turn item recovery off. Expanded billing guidance to note no separate meter, standard OneLake storage costs for soft-deleted items, and potential small CU usage.

  https://learn.microsoft.com/en-us/fabric/admin/retention-recovery

## Moderate Changes

- **Planning in Fabric Billing and Pricing Model**

  Standardized terminology from “Fabric Plan” to “Planning in Fabric,” aligning roles and FAQs with the new naming. Clarified references to billing behavior under the updated branding without changing features or pricing.

  https://learn.microsoft.com/en-us/fabric/iq/plan/resources/billing-fabric-plan

- **Consume a Fabric data agent with the Python client SDK (preview)**

  Updated guidance for the OpenAI Assistants API sunset, directing readers to migrate to the MCP endpoint. Simplified authentication by initializing FabricDataAgentClient with tenant_id and data_agent_url and clarified the client’s source and where to find required IDs and URLs.

  https://learn.microsoft.com/en-us/fabric/data-science/consume-data-agent-python

- **Enable and configure Copilot in Microsoft Fabric**

  Added instructions to enable tenant and delegated capacity settings for using OpenAI as a Microsoft subprocessor and for allowing processing outside regional boundaries when applicable. Included references to the new article on OpenAI as a subprocessor to help admins make informed decisions.

  https://learn.microsoft.com/en-us/fabric/fundamentals/copilot-enable-fabric

- **OneLake security roles: create and manage**

  Clarified that RLS and CLS are supported only for roles with Read permission and not for ReadWrite roles. Added guidance to review and potentially modify the DefaultReader role before assigning restricted roles to avoid unintended access.

  https://learn.microsoft.com/en-us/fabric/onelake/security/create-manage-roles

- **Time Series analysis in Real-Time Dashboard**

  Added a new procedure for creating and configuring the Time Series visual, including choosing fields, managing series, using timeline controls, and customizing chart properties. This helps authors quickly build time-based insights with consistent settings.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/dashboard-time-series

- **Customize Real-Time Dashboard visuals**

  Removed embedded time series and Markdown sections, directing readers to dedicated articles for those topics. Expanded related content links to the visual gallery and specialized guidance to streamline discovery.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/dashboard-visuals-customize

- **Source Control, CI/CD, and ALM for Fabric data agent**

  Expanded data source folder naming conventions with clear prefixes and examples across supported sources. Added guidance that additional sources follow the same pattern and linked to the full catalog to improve repo organization and automation.

  https://learn.microsoft.com/en-us/fabric/data-science/data-agent-source-control

- **Data retention in Fabric Data Warehouse (preview)**

  Revised dropped item retention guidance: enabled by default with the minimum retention reduced from seven to three days. Moved the section below Limitations and clarified tenant-level configuration via the Item Recovery setting.

  https://learn.microsoft.com/en-us/fabric/data-warehouse/data-retention

- **Recover or permanently delete items**

  Reflected the new default: item recovery is enabled by default with a three-day minimum retention for new or never-configured tenants. Updated the adjustable range to 3–90 days and clarified how to ensure the setting is enabled before specifying retention.

  https://learn.microsoft.com/en-us/fabric/admin/item-recovery

- **OneLake shortcut security**

  Clarified that Admin, Member, and Contributor roles aren’t restricted by OneLake security roles but still require access to both the shortcut and target paths (including Read to the target for create/update). Refined how Viewer and item-Read users’ access is determined by OneLake security roles and the requirements for shortcut operations.

  https://learn.microsoft.com/en-us/fabric/onelake/onelake-shortcut-security

- **What Is Planning in Fabric?**

  Rebranded “Plan” to “planning in Fabric” across headings, references, and prerequisites for consistency. Terminology cleanup improves clarity without feature changes.

  https://learn.microsoft.com/en-us/fabric/iq/plan/overview

- **Manage workspaces**

  Updated Item retention to indicate item recovery is on by default and changed the default minimum from seven to three days (range now 3–90). Other details remain the same to align admin expectations.

  https://learn.microsoft.com/en-us/fabric/admin/portal-workspaces

- **PowerTable Sheets in Planning**

  Retitled and refreshed descriptions to consistently use “planning” instead of “Plan.” Ensures clarity of context without altering scope or structure.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-overview

- **What is Real-Time Dashboard?**

  Expanded the overview to highlight visual customization and time series analysis, and moved supported data sources/visuals into dedicated pages. Updated related content to guide readers to the new references.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/real-time-dashboards-overview

- **Copilot and Agent admin settings**

  Introduced new tenant settings to allow use of OpenAI-operated models and to control data processing outside the capacity region/compliance boundary (both default to Disabled). Updated terminology and added screenshots and links to the new subprocessor article to aid admin configuration.

  https://learn.microsoft.com/en-us/fabric/admin/service-admin-portal-copilot

- **Microsoft Fabric tenant settings**

  Removed the section “Users can create Plan items” that described creating Plan items and integrated planning references. This aligns the page with the updated planning terminology and information architecture.

  https://learn.microsoft.com/en-us/fabric/admin/service-admin-portal-microsoft-fabric-tenant-settings

- **OneLake security for SQL analytics endpoints**

  Added detailed steps to change OneLake data access mode for SQL analytics endpoints, including warnings about temporary unavailability and query cancellation. Clarified identity mapping requirements for hub-and-spoke scenarios and emphasized that Warehouse SQL policies don’t enforce through OneLake shortcuts, preventing misconfigured data exposure.

  https://learn.microsoft.com/en-us/fabric/onelake/security/sql-analytics-endpoint-onelake-security

- **Tenant settings index**

  Updated Fabric item recovery to reflect default enablement and reduced minimum retention (three days), and clarified that turning it off makes deletions permanent. Maximum retention remains 90 days.

  https://learn.microsoft.com/en-us/fabric/admin/tenant-settings-index

- **Troubleshoot Real-Time Dashboard visual errors**

  Standardized terminology from “tile” to “visual” across the document to match product language. Keeps existing error categories and guidance intact for consistency.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/troubleshoot-dashboard-tile-error

- **What's new in Microsoft Fabric?**

  Added items for Dropped warehouse recovery (GA) with restore guidance and GPU-accelerated Fabric Data Warehouse (Early Access Preview) for eligible T‑SQL queries. Explains enablement at the workspace level and links to deeper documentation.

  https://learn.microsoft.com/en-us/fabric/fundamentals/whats-new

- **Workspaces in Microsoft Fabric and Power BI**

  Updated Workspace recycle bin information to note item recovery is on by default and to adjust the retention range to 3–90 days. Clarified automatic permanent deletion after the retention period.

  https://learn.microsoft.com/en-us/fabric/fundamentals/workspaces