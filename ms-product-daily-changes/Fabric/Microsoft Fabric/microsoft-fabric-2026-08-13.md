# Microsoft Fabric
**Date created:** 2026-08-13 UTC  
**Tags:** Analytics, Best Practices, Billing, Compliance, Configuration, Consumption, Deprecation, Get Started, Guidance, Monitoring, Performance, Security, Troubleshooting  

## New Articles

- **Query Acceleration in Fabric Data Warehouse (Preview)**

  Introduced GPU-accelerated query execution to speed up joins, aggregations, and scans, improving throughput and consistency for eligible T-SQL workloads. Explained how the acceleration engine works, eligibility constraints, regional availability, and how to enroll and enable it. Detailed monitoring via the Fabric portal and Query Insights (including is_accelerated indicators), viewing operators in execution plans, and separate billing through a dedicated Capacity Units meter. Included links to performance guidelines and an FAQ to help teams evaluate and adopt the feature.

  https://learn.microsoft.com/en-us/fabric/data-warehouse/query-acceleration

## Major Changes

- **Fabric operations**

  Updated billing equivalence for Data Warehouse from two Fabric Capacity Units to 0.538 CUs, aligning cost expectations with current metering. Added a Warehouse Snapshot Query operation under standard usage for clearer categorization. Introduced Query acceleration billing details, defining that one Data Warehouse core with acceleration equals 3.446 CUs and separating meters for Warehouse Query, SQL Endpoint Query, and Warehouse Snapshot Query to improve transparency.

  https://learn.microsoft.com/en-us/fabric/enterprise/fabric-operations

- **How to Observe Fabric Data Warehouse Utilization Trends**

  Reworked utilization guidance to correlate compute consumption with workloads using billing interval start/end times instead of Operation Id mapping. Added a step-by-step method to filter by Warehouse, sort by Total CUs, and capture interval timestamps. Included a new T-SQL example against queryinsights.exec_requests_history to identify requests active within a billing interval, and removed legacy approaches tied to Operation Id.

  https://learn.microsoft.com/en-us/fabric/data-warehouse/how-to-observe-utilization

- **Optimize Input Values for Target KPIs in Fabric Plan**

  Expanded the “Optimize overview” with clearer definitions, examples, and a structured workflow for setting up independent variables, managing visibility, and creating dependent measures. Clarified optimization modes (target-based and direction-based) and strengthened constraint guidance with refined examples and updated images. Improved parameter tuning (strategy, tolerance, iterations) with step-by-step instructions and a sample outcome to help users achieve reliable optimization results.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-optimize/optimizer-overview

- **SQL Audit Logs in Fabric Data Warehouse**

  Added comprehensive guidance on reducing audit noise using predicate expressions that filter events before they’re written and only for enabled action groups. Documented configuration via the Fabric portal and REST API, including syntax, supported fields/constraints, and length limits. Provided practical examples such as excluding service principal activity or repetitive SELECT statements to improve audit relevance and lower storage overhead.

  https://learn.microsoft.com/en-us/fabric/data-warehouse/sql-audit-logs

- **Warehouse Consumption and Utilization in Microsoft Fabric**

  Overhauled the article to explain a vNode-based consumption model with per-second reporting and a simple formula: Active vNodes × Active Time. Updated operation categories (Warehouse Query, SQL Endpoint Query, Warehouse Snapshot Query) and clarified the roles of Capacity Metrics and Query Insights for monitoring. Added step-by-step investigation guidance, example T-SQL to connect high-consumption intervals to queries, and an FAQ to address vNodes, background activity, and concurrency implications.

  https://learn.microsoft.com/en-us/fabric/data-warehouse/usage-reporting

## Moderate Changes

- **Configure SQL Audit Logs in Fabric Data Warehouse**

  Added portal steps to configure predicate filtering, including screenshots and a note that predicates only apply to selected events. Expanded REST API coverage to support predicateExpression in PATCH/GET, clarified behavior when omitting or clearing predicates, and refined auditing enablement and retention defaults to reduce noise and improve control.

  https://learn.microsoft.com/en-us/fabric/data-warehouse/configure-sql-audit-logs

- **Fabric data agent runtime**

  Improved Advanced DAX generation in preview: better reasoning across steps for complex questions and enhanced ambiguity resolution. Strengthened filter generation by searching semantic model values to select correct filters, resulting in more reliable queries.

  https://learn.microsoft.com/en-us/fabric/data-science/data-agent-runtime

- **Experience-specific disaster recovery guidance**

  Added DR guidance for Fabric Apps, noting apps aren’t replicated to secondary regions and remain unavailable during primary region outages. Provided a manual recovery process using stored source and Rayfin CLI, with prerequisites, step-by-step deployment, dependency recovery, role reapplication, and validation steps.

  https://learn.microsoft.com/en-us/fabric/security/experience-specific-guidance

- **Maximize or Minimize a Target Value in Fabric Plan**

  Expanded how-to for using Optimize to maximize/minimize a target value with multiple independent variables, including a concrete Profit Forecast example. Clarified objective selection, variable updates, and multi-constraint setup; explained parent-level distribution and locked cell behavior, and refreshed images and flow.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-optimize/planning-how-to-maximize-minimize-target-value

- **Use Optimize to Meet Target Key Performance Indicators in Fabric Plan**

  Streamlined guidance around target-based optimization with a clear workflow: set objectives, select variables, add range constraints, run optimization, and apply results. Moved prerequisites and parameter details to the overview, clarified parent-level distribution and locked cell behavior, and updated screenshots for easier adoption.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-optimize/planning-how-to-optimize-input-values

- **Fabric region availability**

  Updated the US East region to reflect availability of Fabric App (preview) by removing it from the Not available list. This change signals that teams can now plan deployments of Fabric App (preview) in this region.

  https://learn.microsoft.com/en-us/fabric/admin/region-availability

- **Fabric Runtime 2.0 (GA)**

  Promoted Runtime 2.0 to GA, updated labels in selection UI, and removed preview notices and limitations. Noted that Runtime 2.0 is GA but not yet the default, requiring opt-in until it becomes the default in late September 2026.

  https://learn.microsoft.com/en-us/fabric/data-engineering/runtime-2-0

- **Security feature availability in Microsoft Fabric**

  Updated the availability table by adding Operations agent (Preview) under Fabric IQ, removing the duplicate entry later in the page, and changing Map from Not available to Preview. These changes clarify current security feature status across experiences.

  https://learn.microsoft.com/en-us/fabric/security/security-feature-availability

- **What's New?**

  Added August 2026 entries announcing GPU query acceleration for Fabric Data Warehouse (Preview) with enablement details and expected performance gains. Also highlighted predicate filtering for SQL audit logs, enabling teams to capture only relevant audit events with T-SQL expressions and linking to detailed guidance.

  https://learn.microsoft.com/en-us/fabric/fundamentals/whats-new