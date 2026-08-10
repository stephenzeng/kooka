# Microsoft Fabric
**Date created:** 2026-07-16 UTC  
**Tags:** Administration, Agent, Analytics, Governance, Programming, Security  

## New Articles

- **Understand dependency binding in cross-workspace deployment**
  
  Introduced a concept article explaining how dependency binding works with Git-integrated, cross-workspace deployments in Fabric. It clarifies logical ID versus object ID, which references auto-bind within the same workspace, and that cross-workspace references and connections do not auto-bind. Compatibility matrices outline which dependencies auto-bind, partially bind, or require manual steps across items like Notebooks, Reports, Pipelines, Semantic models, Lakehouses, and more. The guidance highlights when to use parameterization or environment-specific values to ensure successful deployments.
  
  https://learn.microsoft.com/en-us/fabric/cicd/cross-workspace-dependency-binding

- **Apply IBCS Formats in Intelligence Sheets**
  
  Added a how-to guide for enabling IBCS-compliant charts via the Visualizations pane or by applying an IBCS theme from Canvas settings. It explains how to map comparison measures (previous year, plan/target, forecast) and provides an overview of available IBCS templates. The article covers strict versus flexible standards and how to customize visuals using the Minimal theme to balance compliance with design needs.
  
  https://learn.microsoft.com/en-us/fabric/iq/plan/intelligence-ibcs/how-to-apply-ibcs-formatting

- **Configure IBCS Column and Bar Charts**
  
  Published detailed configuration guidance for IBCS column and bar charts, including C01 stacked column, C02 stacked bar, C03 multi-tier column with variance, and C04 multi-tier bar with variance. It provides data well mappings, chart selection tips, and best practices such as assigning forecast/target to specific comparison wells for correct patterns. Illustrative examples help ensure consistent, IBCS-compliant chart configuration.
  
  https://learn.microsoft.com/en-us/fabric/iq/plan/intelligence-ibcs/how-to-configure-ibcs-column-bar-charts

- **Unify data with OneLake shortcuts and mirroring**
  
  Added an overview describing how OneLake shortcuts and mirroring unify data access without traditional pipelines. It compares when to use shortcuts versus mirroring, including supported formats and common scenarios, and explains how mirroring exposes data via replication or shortcuts. The article outlines shortcut transformations (file-to-Delta, AI text processing) and reference architectures that combine mirroring with shortcuts, along with security inheritance, read-only behavior, and operational considerations.
  
  https://learn.microsoft.com/en-us/fabric/onelake/unify-data

## Moderate Changes

- **Anomaly detection in Real-Time Intelligence (Preview)**
  
  Added setup steps to enable anomaly detection at the workspace level, including licensing or trial requirements and enabling the preview feature in the Admin portal. Updated imagery and guidance help administrators configure the feature correctly and avoid onboarding issues.
  
  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/anomaly-detection

- **Create an Ontology Agent with Foundry IQ**
  
  Introduced a new prerequisite requiring the AI Search resource to grant the Search Index Data Contributor role to the Foundry project's managed identity, with Azure portal IAM steps. This prevents 403 errors and ensures the ontology can access required indexes.
  
  https://learn.microsoft.com/en-us/fabric/iq/ontology/how-to-create-agent-foundry-iq

- **Choose the best Fabric CI/CD workflow option for you**
  
  Clarified how dependencies are handled across workspaces during deployment and Git sync. Some items auto-bind via logical IDs, while others require post-deployment updates or parameterization, with steps updated to reflect these behaviors.
  
  https://learn.microsoft.com/en-us/fabric/cicd/manage-deployment

- **Refresh Materialized Lake View activity in Fabric Data Factory pipelines**
  
  Documented a known limitation: the activity refreshes all materialized lake views in the selected lakehouse and does not support selective refresh. This helps planners avoid unexpected workload and design pipelines accordingly.
  
  https://learn.microsoft.com/en-us/fabric/data-factory/refresh-materialized-lake-view-activity

- **Use Python experience on Notebook**
  
  Updated kernel options to include three built-in versions (3.10, 3.11, 3.12) and set Python 3.12 as the default. Clarified support for native IPython features, including iPyWidget and magic commands, to streamline authoring and interactivity.
  
  https://learn.microsoft.com/en-us/fabric/data-engineering/using-python-experience-on-notebook