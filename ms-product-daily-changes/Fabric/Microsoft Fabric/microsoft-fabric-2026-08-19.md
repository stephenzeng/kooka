# Microsoft Fabric
**Date created:** 2026-08-19 UTC  
**Tags:** Analytics, Automation, Best Practices, Configuration, Governance, Guidance, Monitoring, Performance, Security  

## New Articles

- **Configure Gantt Layout in PowerTable**

  Introduced a step-by-step guide to configure the Gantt layout, including required fields, recommended setup flow, and optional enhancements. Added instructions for hierarchy options, milestone handling (including inferred milestones when only an End Date is provided), progress tracking, and dependency types (FS, SS, SF, FF) using TaskID-ConnectionType. Expanded guidance on advanced options such as estimated effort and filter columns, with examples and visuals to speed successful setup.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-layouts/how-to-configure-gantt-layout

- **Customize Resource Layout**

  Added comprehensive customization guidance for the PowerTable resource layout to improve scheduling clarity and utilization tracking. Covered timescale controls, summary metrics, and detailed layout editing, including Timeline settings (work week, capacity, holidays), milestone styles, color rules, and label configuration. Introduced conditional formatting rules to highlight critical bars and milestones, with best practices for creating, ordering, and managing multiple rules.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-layouts/how-to-customize-resource-layout

- **Add and Manage Tasks in Resource Layout**

  Provided end-to-end instructions for creating and editing tasks, milestones, and backlog items directly in the resource layout. Explained assigning resources, setting dates, drag-and-drop adjustments on the timeline, and saving to the database for reliable tracking. Included guidance on moving and deleting tasks, viewing effort allocation, and auditing change history with search, filter, and export options to support governance and operations.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-layouts/how-to-manage-tasks-resource

## Major Changes

- **What's New?**

  Expanded the product update highlights with new previews and GA capabilities across data engineering, SQL, data science, and real-time intelligence. Added dbt job support for Fabric Lakehouse (Preview) to run models and tests directly against Lakehouse assets. Introduced SQL database skills (Preview) to enable AI coding agents to provide schema- and operation-aware guidance. Announced data source routing for Fabric data agents (GA) to automatically select the most relevant sources, plus per-eventstream monitoring controls (Preview) and new guidance for publishing versioned Business Events from Fabric workloads to improve observability and integration.

  https://learn.microsoft.com/en-us/fabric/fundamentals/whats-new

## Moderate Changes

- **Create and manage event schema sets in Microsoft Fabric**

  Clarified role prerequisites so only Admin, Member, or Contributor can create and manage event schema sets, while Viewer remains read-only. Added a pointer to the permissions reference to help admins set the right governance controls.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/schema-sets/create-manage-event-schema-sets

- **Explore Fabric events in Fabric Real-Time hub**

  Expanded supported event groups to include capacity overview, workspace item, OneLake, job, and anomaly detection events. Streamlined action guidance and added related links to help users find the right event streams faster.

  https://learn.microsoft.com/en-us/fabric/real-time-hub/explore-fabric-events

- **Lifecycle of Apache Spark runtimes in Fabric**

  Updated recommendations to use Runtime 2.0 for production and marked it as GA in the lifecycle table. Added an End of Support date of August 31, 2028 to support long-term planning.

  https://learn.microsoft.com/en-us/fabric/data-engineering/lifecycle

- **What is the Microsoft Fabric Capacity Metrics app?**

  Updated alerting guidance to use Fabric capacity overview events for capacity health alerts, replacing prior Real-Time hub references. Added a related link to help readers quickly configure capacity monitoring.

  https://learn.microsoft.com/en-us/fabric/enterprise/metrics-app

- **Use OneLake file explorer to access Fabric data**

  Clarified the exact tenant setting name required for OneLake File Explorer access and when to also enable external app access. Explained expected app behavior when the setting is disabled, reducing setup confusion.

  https://learn.microsoft.com/en-us/fabric/onelake/onelake-file-explorer

- **Gantt layout**

  Revised milestone behavior so milestones render only when a task has an end date without a start date. Removed previously documented milestone alternatives to ensure consistent visualization.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-concept-gantt

- **Introduction to Microsoft Fabric Real-Time hub**

  Replaced the single “Fabric events” connector with specific event types for capacity overview, workspace item, OneLake, and job events. Clarified how events can be routed via eventstreams and used to trigger workflows for automated responses.

  https://learn.microsoft.com/en-us/fabric/real-time-hub/real-time-hub-overview

- **Roles in workspaces in Microsoft Fabric**

  Added role capabilities for event schema sets, enabling Admin/Member/Contributor to create and manage them while all roles can read. Clarified that publishing and consuming business events is controlled by data access roles, improving security posture.

  https://learn.microsoft.com/en-us/fabric/fundamentals/roles-workspaces

- **Apache Spark runtimes in Fabric**

  Updated guidance to recommend GA Runtime 2.0 and adjusted notes on default workspace runtime (new workspaces currently use 1.3). Kept other component details unchanged to minimize migration friction.

  https://learn.microsoft.com/en-us/fabric/data-engineering/runtime

- **Schema Registry in Fabric Real-Time Intelligence (preview)**

  Added a Permissions section with a role-action matrix and sharing options for event schema sets. Clarified that schema set permissions do not grant data access, which remains governed by deny-by-default data access roles, and added in-page references for quick navigation.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/schema-sets/schema-registry-overview

- **Development and Monitoring**

  Updated development guidance to Fabric Runtime 2.0 (Spark 4.1, Java 21, Python 3.13) and confirmed support for the Native Execution Engine. This aligns tooling and performance recommendations with the latest GA runtime.

  https://learn.microsoft.com/en-us/fabric/data-engineering/spark-best-practices-development-monitoring

- **Spark monitoring and performance optimization best practices**

  Revised runtime recommendations to GA Runtime 2.0 and streamlined messaging to focus on performance and reliability gains. Encourages upgrades to benefit from the latest optimizations.

  https://learn.microsoft.com/en-us/fabric/data-engineering/spark-monitoring-best-practices

- **Customer-managed keys for Fabric workspaces**

  Removed the preview label for CMK enablement and documented operational APIs for admins to assign, get, reset, and list encryption status. This improves transparency and control for regulated environments.

  https://learn.microsoft.com/en-us/fabric/security/workspace-customer-managed-keys