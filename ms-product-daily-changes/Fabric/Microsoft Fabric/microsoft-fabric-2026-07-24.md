# Microsoft Fabric
**Date created:** 2026-07-24 UTC  
**Tags:** Administration, AI, Agent, Analytics, Automation, Governance, Security  

## New Articles

- **Agent Integration Options for Ontology (Preview)**

  Introduced guidance on using an ontology as a governed context for AI agents, outlining benefits like consistent business meaning and explainability. Describes five integration paths, including Fabric operations and data agents, Foundry IQ agent with tool calling, Copilot Studio for low-code scenarios, and custom agents via the ontology MCP server. Helps teams choose the right approach and links to how-to guides and tutorials for implementation.

  https://learn.microsoft.com/en-us/fabric/iq/ontology/concepts-agent-integration

- **Optimize Input Values for Target KPIs in Fabric Plan**

  Introduces Optimize in Fabric Plan to tune input measures against target KPIs for planning scenarios such as revenue, margin, and cash flow. Explains prerequisites, two optimization modes (target-based and direction-based), and how to set constraints and tuning parameters when targets aren’t met. Provides examples and tips to accelerate setup and troubleshooting.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-optimize/optimizer-overview

- **Configure approval workflows**

  Adds a how-to for building multi-level approvals in planning sheets using either scripts (On Change Formula) or a no-code configuration. Covers setup of status columns, notifications via Microsoft Teams, and behaviors for submission, approval, rejection, reopening, and completion. Includes examples leveraging SETVALUE and NOTIFY_USER and screenshots to guide configuration and runtime behavior.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-how-to-configure-approval-workflows

- **Use Optimize to Meet Target Key Performance Indicators in Planning**

  Provides a step-by-step guide to run Optimize on calculated fields to maximize, minimize, or meet targets while selecting variables and constraints. Explains tuning (strategy, tolerance, iterations), running on parent cells with proportional distribution, and limiting forecasts to open periods. Notes preview status and includes screenshots to support adoption.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-optimize/planning-how-to-optimize-input-values

- **Reliability in Microsoft Fabric**

  Details Fabric reliability capabilities, including availability zone behavior, cross-region disaster recovery, and business continuity responsibilities. Explains home vs capacity regions, Multi-Geo, and a capacity setting for OneLake geo-replication with scope, cost, and operational considerations. Provides end-to-end disaster recovery setup, failover behavior across experiences, and recovery steps with links to item-specific restoration guidance.

  https://learn.microsoft.com/en-us/fabric/security/reliability-fabric

## Major Changes

- **Manage inbound access to OneLake with Resource Instance Rules**

  Announced general availability by removing the preview designation and added a concrete example using Azure SQL Server to show how trusted resource instance verification works. Introduced a Common scenarios section with step-by-step guidance for Azure SQL Server mirroring and Azure Databricks access via access connector. Includes precise resource ID formats to simplify configuration and reduce misconfiguration risk.

  https://learn.microsoft.com/en-us/fabric/onelake/onelake-manage-inbound-access-trusted-resources

- **OneLake shortcut security**

  Updated delegated shortcut security to support RLS on the producer and clarified CLS is supported on both producer and consumer. Added a constraint that users can belong to only one consumer-side role with CLS when the producer uses RLS, reducing ambiguity in role assignments. Clarified that external shortcut access via Spark or API requires permission to the producer path, tightening access expectations.

  https://learn.microsoft.com/en-us/fabric/onelake/onelake-shortcut-security

- **Tutorial: Use R to predict churn**

  Overhauled the churn tutorial to modernize the R workflow, adding required packages, runtime requirements, and improved dataset handling with validation checks. Refined EDA, class balancing with an updated oversampling approach, and standardized training with explicit LightGBM parameters and clearer evaluation outputs. Clarified saving predictions to Delta and streamlined steps to build a Power BI semantic model, improving reproducibility and end-to-end guidance.

  https://learn.microsoft.com/en-us/fabric/data-science/r-customer-churn

- **What is Real-Time Dashboard?**

  Expanded documentation with a comprehensive list of supported visuals, including anomaly detection, time series, maps, and more. Added descriptions, use cases, and references to customization and Kusto rendering to help users select the right visual for their scenario. This makes capabilities clearer and accelerates dashboard design decisions.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/real-time-dashboards-overview

## Moderate Changes

- **[!INCLUDE [fabric-activator](../includes/fabric-activator.md)] limitations**

  Documented a limit of 500 rules per Data Activator item across all supported data sources. Advises creating additional items when the limit is reached and clarifies this cap is separate from Power BI dashboard data alerts, helping teams plan scale and governance.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/data-activator/activator-limitations

- **OneLake security access control model**

  Clarified that assigning a user to multiple roles with different allowed columns is unsupported when any role includes RLS, and provided an example to illustrate the conflict. This reduces misconfiguration and sets clearer expectations for role design.

  https://learn.microsoft.com/en-us/fabric/onelake/security/data-access-control-model

- **Git integration tenant settings**

  Added guidance on shared tenant settings and how to scope them to all users, specific security groups, or exclusions. Introduced delegated overrides at capacity and workspace levels, explaining precedence from tenant to capacity to workspace to make governance more predictable.

  https://learn.microsoft.com/en-us/fabric/admin/git-integration-admin-settings

- **Use LightGBM models with SynapseML in Microsoft Fabric**

  Added a prerequisite for Fabric Runtime 1.3 or later and guidance for datasets hosted on public Azure Blob Storage. Replaced initial bootstrap code with notes to resolve wasbs authentication errors, including updating URLs or uploading datasets to a lakehouse, and added similar notes in regression and ranking sections.

  https://learn.microsoft.com/en-us/fabric/data-science/how-to-use-lightgbm-with-synapseml

- **Code-first AutoML in Fabric**

  Expanded the MLflow tracking guidance with an example that sets a run_name prefix for child runs and configures an AutoML experiment with explicit settings. Clarified terminology and Spark parallelization details to improve experiment management and traceability.

  https://learn.microsoft.com/en-us/fabric/data-science/python-automated-machine-learning-fabric

- **Inbound network protection in Microsoft Fabric**

  Added Resource Instance Rules to enable workspace admins to allow inbound access from specific Azure resource instances using resource IDs. This supports services with dynamic or shared IPs and aligns with trusted resource guidance for more granular control.

  https://learn.microsoft.com/en-us/fabric/security/security-inbound-overview