# Microsoft Foundry
**Date created:** 2026-08-29 UTC  
**Tags:** Automation, Best Practices, Configuration, Deprecation, Governance, Guidance, Monitoring, Security, Troubleshooting  

## New Articles

- **Evaluation datasets in Microsoft Foundry**

  Introduced a new concept article explaining how to use reusable evaluation datasets across scenarios, including how Foundry interprets JSONL data for messages, roles, and responses. Describes evaluation granularity (turn-level vs. conversation-level) and when to choose each. Provides multiple data preparation paths—upload curated data, generate synthetic datasets, convert traces, simulate conversations, or evaluate by response IDs—with a comparison of approaches and links to schema and workflows. Helps teams standardize evaluations and accelerate iterative improvement.

  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/evaluation-datasets

- **Evaluation dataset schema in Microsoft Foundry**

  Added a detailed schema reference covering supported scenarios and required columns for model/agent evaluation and conversation simulation. Clarifies the messages structure (roles, content arrays, tool_call/tool_result) aligned with OpenAI Responses, plus examples for tool calls and content arrays. Documents evaluator-specific column needs, separate query/response formats (including CSV), and guidance on applying data mappings. Enables consistent dataset design and smoother integration with built-in evaluators.

  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/evaluation-dataset-schema

## Major Changes

- **Evaluate Semantic Kernel with prompt flow**

  Reoriented guidance from planner-based evaluation to evaluating plugins and orchestration code, reflecting the removal of Semantic Kernel planners (Stepwise, Handlebars). Introduces automatic function calling as the recommended approach, with updated examples and batch testing flows. Strengthens recommendations on using function-calling-capable models, clearer plugin descriptions, and better request instructions. This helps teams modernize implementations and avoid deprecated planner workflows.

  https://learn.microsoft.com/en-us/azure/machine-learning/prompt-flow/how-to-evaluate-semantic-kernel?view=azureml-api-2

- **Publish agents to Microsoft 365 and Teams by using the REST API**

  Overhauled PNA (public network access) guidance to enable Microsoft 365 access while keeping most endpoints private. Adds enable_m365_public_endpoint to expose only the Activity Protocol route via a service-managed, source IP-filtered public path with explicit authorization (BotServiceRbac or BotServiceTenant). Updates identity usage to client_id, refactors step flow, and expands security details on ingress, TLS, filtering limits, and troubleshooting (including 403 NetworkAccessDenied). This improves security posture and simplifies publishing for private-network projects.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/publish-copilot-virtual-network

- **Agent tracing overview**

  Aligned multi-agent observability with OpenTelemetry GenAI conventions and called out their Development status. Replaced the prior conventions with updated span and attribute names (for example, invoke_agent, plan, execute_tool, memory operations, and tool-related attributes). This standardizes tracing semantics for agents and tools, improving interoperability and analysis across systems.

  https://learn.microsoft.com/en-us/azure/foundry/observability/concepts/trace-agent-concept

- **Troubleshoot guidance**

  Corrected Azure OpenAI rate-limit error handling (409 to 429) and clarified the explanation. Updated vulnerability guidance to note prompt flow images are frozen and no longer receive security or package updates, urging dependency updates, rebuilding custom images from supported bases, and migrating to Microsoft Agent Framework ahead of retirement. Warns not to rely on newer runtime images for fixes, helping teams mitigate risk and plan migrations.

  https://learn.microsoft.com/en-us/azure/machine-learning/prompt-flow/troubleshoot-guidance?view=azureml-api-2

## Moderate Changes

- **Agent evaluators**

  Updated evaluator guidance to use explicit query and response message arrays aligned with OpenAI-style schemas and added tool_call_id linkage in examples. Simplified tool_definitions by removing the OpenAI function wrapper in favor of a tools list with JSON Schema parameters, and referenced centralized message schema docs. This clarifies data structures and improves interoperability with tool calls.

  https://learn.microsoft.com/en-us/azure/foundry/concepts/evaluation-evaluators/agent-evaluators

- **Configure and share your agent**

  Added instructions for allowing Microsoft 365 traffic to a private-network agent by enabling protocol_configuration.activity.enable_m365_public_endpoint. Included a REST PATCH example for configuring Activity protocol and required authorization schemes, plus security considerations and updated property reference. Helps securely reach Microsoft 365 while keeping other surfaces private.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/configure-agent

- **Use Terraform to create Microsoft Foundry**

  Noted that the azapi provider now supports configuring connections to knowledge and tools. Updated verification steps to use terraform validate with guidance on expected state and configuration checks. This streamlines setup and increases confidence in deployments.

  https://learn.microsoft.com/en-us/azure/foundry/how-to/create-resource-terraform

- **Deploy a flow to online endpoint for real-time inference with CLI**

  Clarified that prompt flow runtime images are frozen and the latest tag will not receive updates; use only to maintain existing deployments while planning migration. Fixed build-context paths, corrected YAML examples (including PROMPTFLOW_SERVING_ENGINE: fastapi), and improved accuracy across steps. This reduces security risk and deployment errors.

  https://learn.microsoft.com/en-us/azure/machine-learning/prompt-flow/how-to-deploy-to-code?view=azureml-api-2

- **How to use streaming endpoints deployed from prompt flow**

  Clarified streaming requires a runtime later than 20230816.v10 and that prompt flow images no longer receive updates. Advised verifying runtime compatibility and migrating to Microsoft Agent Framework if incompatible, with streamlined instructions to check runtime versions. Ensures reliable streaming and a clear migration path.

  https://learn.microsoft.com/en-us/azure/machine-learning/prompt-flow/how-to-enable-streaming-mode?view=azureml-api-2

- **Enable trace and collect feedback for a flow deployment (preview)**

  Updated samples to send feedback to the same trace span and to use AZUREML_ENDPOINT_CREDENTIAL for authorization instead of a hardcoded key. Removed unused imports and clarified Application Insights usage and credential setup. Improves security and trace fidelity.

  https://learn.microsoft.com/en-us/azure/machine-learning/prompt-flow/how-to-enable-trace-feedback-for-deployment?view=azureml-api-2

- **GenAIOps with prompt flow and Azure DevOps**

  Added a least-privilege notice for the service principal and recommended scoping roles narrowly in production. Clarified local .env configuration, including Azure OpenAI connection naming and setting api_version supported by the deployment and Prompt Flow. Strengthens security and reduces configuration errors.

  https://learn.microsoft.com/en-us/azure/machine-learning/prompt-flow/how-to-end-to-end-azure-devops-with-prompt-flow?view=azureml-api-2

- **Integrate LangChain in prompt flows**

  Updated credential conversion guidance and Python snippet to use environment variables for AZURE_OPENAI settings and a generic resource URL. Clarified choosing a compatible API version for the integration and deployment. Improves portability and reduces hardcoded secrets.

  https://learn.microsoft.com/en-us/azure/machine-learning/prompt-flow/how-to-integrate-with-langchain?view=azureml-api-2

- **Integrate prompt flow with DevOps for LLM-based applications**

  Noted the Web Classification demo repo is archived and read-only and directed users to the current GenAIOps Prompt Flow template. Updated pipeline guidance to recommend the new template while retaining the archived project as a reference. Keeps users aligned with supported resources.

  https://learn.microsoft.com/en-us/azure/machine-learning/prompt-flow/how-to-integrate-with-llm-app-devops?view=azureml-api-2

- **Incorporate images into prompt flow (preview)**

  Added a notice that the legacy GPT-4 vision-preview model is retired and advised using supported vision-enabled models. Clarified testing by noting the Test tab does not support image I/O and directing users to send request payloads instead. Prevents reliance on retired models and improves test accuracy.

  https://learn.microsoft.com/en-us/azure/machine-learning/prompt-flow/how-to-process-image?view=azureml-api-2

- **Foundry Agent Service limits, quotas, and regional support**

  Added a new “Private VNet” column to the regional support table and marked support as Yes across all listed regions. Highlights availability of private networking for agents in supported regions.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/limits-quotas-regions

- **Publish agents to Microsoft 365 Copilot and Microsoft Teams in the Foundry portal**

  Expanded guidance for projects with public network access disabled by documenting how to enable a source-IP-filtered public Activity Protocol route via enable_m365_public_endpoint and use the REST API for publishing. Linked to the detailed publishing article that includes the configuration steps and authorization requirements. Enables secure publishing without broad public exposure.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/publish-copilot