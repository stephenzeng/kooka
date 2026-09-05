# Microsoft Foundry
**Date created:** 2026-09-05 UTC  
**Tags:** Automation, Best Practices, Billing, Compliance, Configuration, Consumption, Governance, Guidance, Identity, Monitoring, Performance, Security, Troubleshooting  

## New Articles

- **Provisioned throughput for Foundry Models in Azure Government**

  Introduced a new concept article explaining provisioned throughput for Foundry Models in Azure Government. It details fungible PTU quota, hourly billing via Azure Reservations, and model eligibility for provisioned deployments. The guidance helps government customers plan capacity, cost, and deployment options aligned to compliance needs.

  https://learn.microsoft.com/en-us/azure/foundry/openai/concepts/provisioned-throughput-gov

- **Retrieve diagnostics from Azure Content Understanding in Foundry Tools**

  Added a new how-to showing how to fetch diagnostics using the REST API, including submitting asynchronous analysis and polling the Operation-Location. Clarifies that GA (2025-11-01) requires the x-ms-diagnostics: true header to return result.infos, while the 2026-06-01-preview includes diagnostics by default. Provides cURL examples and guidance to interpret LLMStats and other diagnostic codes to troubleshoot and branch logic reliably.

  https://learn.microsoft.com/en-us/azure/ai-services/content-understanding/how-to/retrieve-diagnostics

## Major Changes

- **Run agent evaluations with the azd CLI (preview)**

  Overhauled evaluation guidance to use the Azure Developer CLI agent extension, moving from legacy azd ai eval to azd ai agent eval commands. Introduces a hosted-agent lifecycle (init, provision, deploy, eval generate, eval run, eval update) with optional optimization and improved reproducibility via eval.yaml. Adds new capabilities such as interactive/scripted generation, --no-wait for jobs, run inspection (list/show), update flows for local changes, and reset/repair options, while removing older start/gating patterns.

  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/azure-developer-cli-evaluation

- **Azure OpenAI reasoning models - GPT-6 Astra and GPT-5**

  Added GPT-6 Astra with a full feature matrix and availability details, and expanded support tables to cover GPT-6 alongside GPT-5. Clarified tool-calling constraints and combined Chat Completions behavior, including when tools can be used with reasoning_effort settings. Extended reasoning features with new parameters (reasoning.context, reasoning.mode), expanded options (including max), and clarified unsupported parameters, including logprobs support for GPT-6 Astra and ongoing restrictions for other models.

  https://learn.microsoft.com/en-us/azure/foundry/openai/how-to/reasoning

## Moderate Changes

- **Create a SharePoint (Remote) Knowledge Source**

  Reorganized limitations into distinct Copilot Retrieval API and Azure AI Search sections, explaining their respective impacts. Documented Azure AI Search concurrency limits for remote SharePoint, including Dedicated vs. Serverless (preview) behaviors, latency implications, and guidance to add replicas for throughput on Dedicated.

  https://learn.microsoft.com/en-us/azure/search/agentic-knowledge-source-how-to-sharepoint-remote

- **Query Knowledge Base via API or MCP**

  Clarified request controls: maxRuntimeInSeconds limits retrieval runtime and maxOutputSizeInTokens caps response size. Added parameter specifics, including a 10–600s range with a 90s default, noting the 600s cap applies to the Azure AI Search retrieve request.

  https://learn.microsoft.com/en-us/azure/search/agentic-retrieval-how-to-retrieve

- **Connect to an A2A agent endpoint from Foundry Agent Service (preview)**

  Added end-to-end Azure Developer CLI steps to create agent-to-agent connections with examples for multiple auth types (none, custom-keys, OAuth2, user Entra token, project managed identity, agentic identity). Included a reference mapping auth types to required flags, RBAC role guidance for identity-based scenarios, and audience guidance for Foundry targets.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/agent-to-agent

- **Agent2Agent (A2A) authentication**

  Added a prerequisite to set the active Foundry project with azd ai project set. Provided CLI examples for agentic-identity and project-managed-identity connections with audience configuration, plus minor text refinements.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/agent-to-agent-authentication

- **Connect an Azure AI Search index to Foundry agents**

  Introduced an Azure Developer CLI tab with steps to configure a cognitive-search connection using managed identity or API key. Added RBAC role assignment guidance for managed identity and secure handling practices for API keys to keep secrets out of source control.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/ai-search

- **Connect agents to Microsoft Fabric with Fabric IQ (preview)**

  Replaced declarative azure.yaml instructions with CLI-based connection creation using azd ai connection create. Added steps to set project and workspace endpoints and to authenticate with a user Entra token and audience for the Fabric IQ remote tool.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/fabric-iq

- **Microsoft Foundry in Azure Government**

  Added a Provisioned throughput section covering fungible PTU quota, eligible models, and Azure Reservation requirements. Updated related links to include the Azure Government provisioned throughput guidance.

  https://learn.microsoft.com/en-us/azure/foundry/concepts/foundry-azure-government

- **Set up authentication for Model Context Protocol (MCP) tools**

  Added a prerequisite to set the active project before creating identity-based MCP connections. Provided examples for agentic and project managed identities with audience configuration, and clarified that only remote MCP endpoints are supported with deployment guidance to Azure services.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/mcp-authentication

- **Connect agents to Model Context Protocol servers**

  Added OAuth examples using Foundry-managed connectors via --connector-name and clarified bring-your-own OAuth parameters. Included a table of supported MCP servers and connectors, and guidance to use custom app registrations for other OAuth-enabled servers.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/model-context-protocol

- **Service limits in Azure AI Search**

  Documented retrieve request runtime limits for maxRuntimeInSeconds, including 10s minimum, 90s default, and 600s maximum across tiers. Clarified that the maximum applies to the Azure AI Search retrieve request and referenced configuration examples for overriding defaults.

  https://learn.microsoft.com/en-us/azure/search/search-limits-quotas-capacity

- **Web search tool**

  Added steps to create a Bing Custom Search connection via azure.yaml when azd ai connection create doesn’t support the category. Included YAML configuration, provisioning steps, and secure handling guidance for API keys.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/web-search

- **Connect agents to Microsoft 365 with Work IQ (preview)**

  Added Azure Developer CLI instructions to create a Work IQ connection with OAuth2 endpoints, client credentials, and scopes. Included setup for environment variables and app registration redirect URL, and updated references to the Entra app setup guidance.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/work-iq