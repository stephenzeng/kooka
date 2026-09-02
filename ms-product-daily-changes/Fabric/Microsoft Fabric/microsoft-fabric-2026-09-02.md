# Microsoft Fabric
**Date created:** 2026-09-02 UTC  
**Tags:** Analytics, Automation, Best Practices, Billing, Compliance, Configuration, Consumption, Get Started, Governance, Guidance, Licensing, Monitoring, Performance, Security, Troubleshooting  

## New Articles

- **Enable co-publishers for a Fabric data agent in Microsoft 365 Copilot**

  Introduced step-by-step guidance to let multiple co-creators republish a Fabric data agent to Microsoft 365 Copilot. Explains prerequisites and the distinct ownership models between Fabric (editing/first publish) and Microsoft 365 (republish rights). Walks through granting Fabric co-creator access, publishing to Microsoft 365 Copilot, and adding co-publishers in the agent’s Publishing settings. Highlights that republishes can fail if co-publishers aren’t configured and provides related references.

  https://learn.microsoft.com/en-us/fabric/data-science/data-agent-enable-co-publishers

- **Consume Fabric data agent from Microsoft Foundry via Fabric IQ (preview)**

  Describes how to connect published Fabric data agents to Microsoft Foundry using the Fabric IQ (OneLake Catalog) tool. Covers required capacity, regional considerations, roles, and an end-to-end workflow to add agents as MCP endpoints in Foundry for routing queries. Includes UI steps and code paths (Python/C#/JS/REST), guidance for handling long-running queries via background mode, and links to related concepts and observability.

  https://learn.microsoft.com/en-us/fabric/data-science/data-agent-foundry-fabric-iq

- **Create Row Model Templates for Reusable Row Structures**

  Provides a how-to for building reusable row model templates to speed up planning scenarios. Explains enabling Model Builder, creating templates (including bulk inserts and configuration for data sources, aggregations, and KPIs like Net Profit), and applying templates with Append or Replace. Details conditional application via simple/advanced filters and how to manage templates across regions.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-row-model/how-to-create-templates

## Major Changes

- **Subscribe permissions for Azure and Fabric events**

  Reduced the retention window for paused event listeners from up to 7 days to up to 24 hours, tightening recovery expectations. Updated remediation guidance to restore the owner’s subscribe permission or reassign to a user with sufficient permission instead of deleting and recreating the configuration. Clarified that delivery resumes automatically once permissions are fixed, which may take a couple of hours, and refined wording throughout.

  https://learn.microsoft.com/en-us/fabric/real-time-hub/fabric-events-subscribe-permission

- **Limitations in SQL database in Microsoft Fabric**

  Updated the feature matrix to indicate that Transparent Data Encryption (TDE) is now supported for Fabric SQL database. Removed the prior limitation indicating reliance on storage encryption and references that previously stated customer-managed keys weren’t supported. This change signals a stronger at-rest data protection posture and aligns documentation with current capabilities.

  https://learn.microsoft.com/en-us/fabric/database/sql/limitations

- **OneLake compute and storage consumption**

  Added a new section explaining that some Fabric workloads access OneLake during internal processing and consume Capacity Units similar to user actions. Noted that OneLake consumption from certain Spark system-initiated calls was underreported and will begin to be reported and billed starting October 1, 2026. This prepares administrators for more accurate consumption visibility and potential billing changes.

  https://learn.microsoft.com/en-us/fabric/onelake/onelake-consumption

- **Operation list**

  Clarified that OneLake data access and storage auditing should use OneLake diagnostics, and that Fabric audit logs don’t cover all OneLake data-plane activity. Removed numerous OneLake-related operations from the audit operations list to avoid implying full coverage. This helps admins use the right telemetry sources for comprehensive audit scenarios.

  https://learn.microsoft.com/en-us/fabric/admin/operation-list

- **Copilot and Agent tenant settings**

  Moved the setting “Users can use Copilot, AI Agents and other AI experiences powered by OpenAI as a Microsoft Subprocessor” from Enabled by default to Disabled by default, changing the default governance posture. Removed the “Conversation history stored outside your capacity's geographic region...” bullet and its associated section. Reordered data processing/location bullets under Disabled by default for clarity.

  https://learn.microsoft.com/en-us/fabric/admin/service-admin-portal-copilot

- **Tutorial: evaluate RAG performance in Fabric**

  Substantially revised to focus on evaluating RAG within Fabric, with clearer prerequisites (Fabric workspace/lakehouse, Azure AI Foundry project with Azure OpenAI, and Azure AI Search index). Updated setup to use deployment names, current API version, and Fabric’s client initialization, and centralized client configuration. Clarified evaluation metrics and workflow (groundedness, relevance, similarity), added validation checks, improved saving/comparing results in OneLake, and expanded troubleshooting.

  https://learn.microsoft.com/en-us/fabric/data-science/tutorial-evaluate-rag-performance

- **What's new? archive**

  Expanded the archive with comprehensive June 2026 updates spanning platform, data movement, Spark, data science, SQL, mirroring, real-time intelligence, development/CI-CD, Fabric IQ and agents, and community. Introduced a new “Fabric Apps (Preview)” section capturing SDK/CLI developments and app capabilities. The additions provide a consolidated historical view of key releases and previews across the stack.

  https://learn.microsoft.com/en-us/fabric/fundamentals/whats-new-archive

- **Workspace outbound access protection for Azure, Fabric, and Business events (preview)**

  Expanded scope to include Business events alongside Azure and Fabric events and clarified that publisher workspaces must allow the appropriate connector (for example, User Data Functions) when outbound access protection is enabled. Added a detailed Business events example covering source, consumer, and publisher workspaces and specified that allow lists are managed via data connection rules. Updated behavior so configurations resume automatically after required connectors are re-allowed, and noted that managed private endpoints aren’t supported.

  https://learn.microsoft.com/en-us/fabric/security/workspace-outbound-access-protection-real-time-events

## Moderate Changes

- **Install a Private Package as a requirement in Apache Airflow Job**

  Corrected the path for installing private wheel packages to the full /opt/airflow/plugins/libs/<your-wheel-file>.whl location and updated the example. This ensures package resolution works reliably in Airflow jobs.

  https://learn.microsoft.com/en-us/fabric/data-factory/apache-airflow-jobs-install-private-package

- **Microsoft Copilot in Fabric in the Data Factory Workload Overview**

  Expanded Dataflow Gen2 capabilities to include getting data from sources via natural language and undoing the last applied step. Clarified enablement prerequisites and improved descriptions and best-practice references to aid discoverability and usage.

  https://learn.microsoft.com/en-us/fabric/data-factory/copilot-fabric-data-factory

- **How to Get Started with Microsoft Copilot in Fabric in the Data Factory Workload**

  Updated prerequisites to require paid capacity (F2+/P1+), workspace assignment to that capacity, and admin enablement of Copilot, with trials not supported; added a data residency requirement for regions outside US/EU. Streamlined Dataflow Gen2 steps by removing the starter prompt icon, adding a Send message step, and refining the sequence before choosing the OData connector. These changes help admins configure environments correctly and guide users through a clearer setup flow.

  https://learn.microsoft.com/en-us/fabric/data-factory/copilot-fabric-data-factory-get-started

- **Evaluate your data agent (preview)**

  Standardized terminology, added a prerequisite that evaluation requires a published agent in the target stage, and enhanced examples with error handling and sample output. Introduced Diagnostics and a Troubleshooting section to accelerate debugging, and streamlined the API guidance to focus on practical usage. These changes improve reliability and reduce friction when validating agents.

  https://learn.microsoft.com/en-us/fabric/data-science/evaluate-data-agent

- **Paused event configurations in Real-Time hub**

  Clarified that paused configurations automatically resume after underlying issues are resolved, which may take a couple of hours. Updated examples and mitigation guidance to restore/assign subscribe permissions or adjust network/private link settings without deleting and recreating consumers, and noted ongoing permission checks. This reduces operational churn and shortens recovery.

  https://learn.microsoft.com/en-us/fabric/real-time-hub/fabric-events-paused-state

- **Data security in OneLake**

  Directed users to OneLake diagnostics for data-plane access auditing and to Fabric audit logs for control-plane activities. Named the external access tenant setting explicitly and noted it must be enabled to use shortcuts with OneLake security. This helps ensure comprehensive auditing and correct configuration for external access scenarios.

  https://learn.microsoft.com/en-us/fabric/onelake/security/get-started-security

- **Use Azure Language in Foundry Tools text analytics in Fabric with REST API and SynapseML (preview)**

  Fixed the SentimentAnalysis example by changing opinionMining from a string to a boolean to match the API contract. This prevents payload errors and aligns samples with production usage.

  https://learn.microsoft.com/en-us/fabric/data-science/ai-services/how-to-use-text-analytics

- **How to read and write data with Pandas in Microsoft Fabric**

  Added guidance on when to use Pandas vs. Spark/Delta tables and standardized path examples, emphasizing keeping large datasets in Spark. Included an important note about toPandas() memory usage and refreshed read/write samples and Delta guidance. This improves performance choices and reduces memory-related failures.

  https://learn.microsoft.com/en-us/fabric/data-science/read-write-pandas

- **Tutorial: Use R to create, evaluate, and score a fraud detection model**

  Updated package installation instructions to use devtools::install_version() and to install bnlearn and imbalance, replacing previous guidance. This aligns the tutorial with reliable library versions and compatible APIs.

  https://learn.microsoft.com/en-us/fabric/data-science/r-fraud-detection

- **Use sparklyr**

  Updated guidance to connect to a Fabric Spark session, corrected links and minor code issues, and clarified DBI behavior. Corrected the model example to linear regression and streamlined references to transformers and ML docs. These refinements reduce confusion and align examples with current best practices.

  https://learn.microsoft.com/en-us/fabric/data-science/r-use-sparklyr

- **Use SparkR**

  Switched file access guidance to ABFS paths and updated examples and notes accordingly. Clarified how to copy ABFS or relative paths from the Lakehouse explorer, improving reliability when reading and writing data.

  https://learn.microsoft.com/en-us/fabric/data-science/r-use-sparkr

- **Use Tidyverse**

  Replaced the deprecated gather() example with pivot_longer(), updating code and explanation for converting wide to long data. This keeps guidance current with the tidyr API and avoids deprecated patterns.

  https://learn.microsoft.com/en-us/fabric/data-science/r-use-tidyverse

- **Supported scenarios and limitations for workspace-level private links**

  Reduced the retention period for paused Real-Time hub event configurations after workspace-level private link changes from up to 7 days to up to 24 hours. This sets clearer expectations for how long events are retained during pauses.

  https://learn.microsoft.com/en-us/fabric/security/security-workspace-level-private-links-support

- **Tutorial: Validate data using SemPy and Great Expectations (GX)**

  Specified using great-expectations<1.0 to match the sample notebook and APIs, noting that newer versions differ. Clarified that one expectation failure is intentional to support diagnostics. This ensures a consistent setup and smoother tutorial execution.

  https://learn.microsoft.com/en-us/fabric/data-science/tutorial-great-expectations

- **What's New?**

  Added several entries including Advanced DAX generation for semantic models (Preview), a new CI/CD samples subsection, and a Data Warehouse update on using AI functions with Power BI. Earlier additions include Fabric Maps in Real-Time Dashboards, gateway release details, and GA updates such as Migration Assistant to SQL database and Warehouse IDENTITY columns. These updates improve discoverability of new capabilities and guidance.

  https://learn.microsoft.com/en-us/fabric/fundamentals/whats-new

- **Workspace outbound access protection**

  Expanded supported Real-Time Events item types to include Business events in addition to Azure and Fabric events. This enables consistent outbound access governance across more event categories.

  https://learn.microsoft.com/en-us/fabric/security/workspace-outbound-access-protection-overview

- **Workspace private links for Azure and Fabric events**

  Updated behavior so that after private link settings change, consumer configurations pause and then automatically resume once the underlying condition is resolved, which may take a couple of hours. Removed prior guidance to delete and recreate consumers, reducing operational overhead and risk.

  https://learn.microsoft.com/en-us/fabric/real-time-hub/workspace-private-links-real-time-events