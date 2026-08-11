# Microsoft Fabric
**Date created:** 2026-07-25 UTC  
**Tags:** Agent, Administration, AI, Analytics, Automation, Monitoring, Programming, Security  

## New Articles

- **Quickstart: Query and consume OneLake data**

  Introduced a guided walkthrough for querying the same OneLake Delta table across multiple engines without copying data. The quickstart covers running T-SQL via the SQL analytics endpoint, building a Power BI Direct Lake semantic model and report, and analyzing the table in a Spark notebook with PySpark. It highlights the OneLake “one copy of data” pattern, and includes prerequisites, cleanup steps, and related references.

  https://learn.microsoft.com/en-us/fabric/onelake/quickstart-consume-data

- **Fix Copilot unavailable after a trial expires in Power BI**

  Added troubleshooting guidance for scenarios where Copilot becomes unavailable after a Fabric trial ends or when workspaces run on unsupported capacity. The article provides a clear checklist to verify trial status, workspace capacity, Copilot capacity assignment, and licensing, along with steps to restore access. It outlines options to move workspaces to supported capacity, start a new trial or purchase capacity, and resolve licensing issues, with links to related Copilot setup documentation.

  https://learn.microsoft.com/en-us/fabric/fundamentals/troubleshoot-copilot-unavailable-after-trial

- **Outbound Access Protection for Operations Agent (Preview)**

  Published a concept guide explaining how Outbound Access Protection governs the Operations Agent’s external actions during preview. It clarifies which actions are governed versus unaffected, documents preview limitations, and describes what users see when actions are blocked. The article also details configuration dependencies, how to monitor and troubleshoot via Activity Log, and provides FAQs and recommendations for testing and rollout.

  https://learn.microsoft.com/en-us/fabric/security/workspace-outbound-access-protection-operations-agent

## Major Changes

- **Known Limitations in Plan (Preview)**

  Expanded and clarified limits and behaviors for Plan (preview) so teams can plan deployments confidently. New guidance covers how renaming semantic models or workspaces can break connected items, how to recover PowerTable DMTS connections, and caps such as 1 million rows for bulk data input, up to 25 sheets and 50 visuals per item, and 1.2 million cells per query/writeback (with recommendations to split across sheets). It also notes that effective limits depend on client resources, capacity, and Power BI XMLA constraints, and reiterates requirements and unsupported capacities for XMLA-driven scenarios.

  https://learn.microsoft.com/en-us/fabric/iq/plan/overview-limitations

- **Pricing for Dataflow Gen2**

  Removed Mapping Data Flow transforms compute pricing information and related examples to prevent outdated guidance from causing confusion. This change eliminates the prior CU rate description, the MDF transforms pricing row, and the detailed consumption calculations section, aligning the page with current pricing coverage.

  https://learn.microsoft.com/en-us/fabric/data-factory/pricing-dataflows-gen2

## Moderate Changes

- **Multivariate Anomaly Detection with Isolation Forest**

  Reworked the article into a practical Fabric how-to with updated prerequisites, cleaner code samples, and clearer type casting and imports. It clarifies inference-time parameters, makes MLflow registration optional for same-notebook scenarios, and directs users to Real-Time Intelligence given the retirement of Azure AI Anomaly Detector, with updated references.

  https://learn.microsoft.com/en-us/fabric/data-science/isolation-forest-multivariate-anomaly-detection

- **Browse pipeline runs in the Monitoring hub**

  Added a hierarchical pipeline view to help track upstream and downstream jobs directly in Monitoring Hub. The update explains how to enable the columns, interpret the hierarchy, and distinguishes run relationships from artifact parent-child structures.

  https://learn.microsoft.com/en-us/fabric/data-factory/monitoring-hub-pipeline-runs

- **Quickstart: Get data into OneLake**

  Updated the flow to explicitly include downloading sample data and using Lakehouse Get data > Upload files. Added screenshots and a next step that guides readers to querying and consuming the loaded data.

  https://learn.microsoft.com/en-us/fabric/onelake/quickstart-get-data

- **Fabric Runtime 1.2 (EOS)**

  Clarified that Starter Pool isn’t available for deprecated runtimes. Sessions on Runtime 1.2 use an on-demand pool, which can add a few minutes to startup time.

  https://learn.microsoft.com/en-us/fabric/data-engineering/runtime-1-2

- **Schedule a User Data Function**

  Strengthened scheduling guidance by requiring the FunctionName parameter and showing how to pass additional inputs that match the function signature exactly. Examples and parameter tables help avoid case and naming mismatches.

  https://learn.microsoft.com/en-us/fabric/data-engineering/user-data-functions/schedule-functions

- **What is Fabric User data functions?**

  Expanded capabilities to include variable libraries for central configuration, Cosmos DB connections, and business events for event-driven scenarios. Introduced generic connections that leverage the item owner’s Microsoft Entra ID token for flexible access to Fabric items or Azure resources, with a link to detailed setup guidance.

  https://learn.microsoft.com/en-us/fabric/data-engineering/user-data-functions/user-data-functions-overview

- **What is workspace monitoring (preview)?**

  Updated monitoring categories to use Real-Time Intelligence for Eventhouse and added Eventstream monitoring (Node Status, Metrics, Error Metrics). This expands visibility into real-time components within the workspace.

  https://learn.microsoft.com/en-us/fabric/fundamentals/workspace-monitoring-overview