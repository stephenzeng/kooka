# Microsoft Foundry
**Change date:** 2026-08-07 UTC  
**Tags:** Administration, AI, Agent, Automation, Governance, Monitoring, Programming, Security  

## New Articles

- **Use admin-connected models in cloud evaluations**

  Introduced guidance for using admin-connected models (via enterprise AI gateways such as Azure API Management or other gateways) in Foundry cloud evaluations. Explains prerequisites, scope limits (OpenAI Chat Completions API only, preview), and the reference format connection-name/deployment-name. Provides Python examples for using these models as evaluator judges and as targets with sampling parameters, and clarifies they aren’t supported for synthetic data generation.

  https://learn.microsoft.com/en-us/azure/foundry/how-to/develop/evaluate-admin-connected-models

- **Deploy a C# Search App to Azure Container Apps**

  New tutorial to deploy a C# web app that uses Azure AI Search to Azure Container Apps using Azure Developer CLI (azd). Covers identity defaults (managed identity) with an option to switch to key-based auth, provisioning and deployment steps with azd up, how to verify the deployed endpoints, and troubleshooting connectivity and access. Includes cleanup guidance with azd down --purge.

  https://learn.microsoft.com/en-us/azure/search/tutorial-csharp-deploy-web-search

## Major Changes

- **Connect to an A2A agent endpoint from Foundry Agent Service (preview)**

  Updated prerequisites to use Foundry-specific roles and clarified how to target Foundry agents via A2A, including supported protocol versions and modality limits. Improved setup and security guidance, standardized token acquisition and headers across SDK, CLI, and REST examples, and updated APIs (toolboxes create_version, Bearer token provider) and sample payloads (agent_reference). These changes reduce friction, ensure least-privilege access, and align samples with current tooling.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/agent-to-agent

- **How to use Azure AI Search in Foundry Agent Service (classic)**

  Expanded cross-language samples and prerequisites for classic agents using an existing Azure AI Search index. Standardized environment configuration, corrected APIs, and added full lifecycle flows (create agent/thread, run, poll, output, cleanup) plus REST requirements for a newer preview API. This helps maintain legacy scenarios while making samples reliable and production-oriented.

  https://learn.microsoft.com/en-us/azure/foundry-classic/agents/how-to/tools-classic/azure-ai-search-samples

- **Use Custom Bing Search with classic Foundry agents**

  Revamped content with clear prerequisites, deprecation context, and streamlined Python and REST samples using environment-driven configuration and explicit cleanup. Added troubleshooting and related links, and removed redundant steps. This improves reliability and operational clarity for maintaining classic implementations.

  https://learn.microsoft.com/en-us/azure/foundry-classic/agents/how-to/tools-classic/bing-custom-search-samples

- **Grounding agents with Bing Search tools**

  Reorganized guidance with a scenario matrix, refined RBAC using Entra PIM, and clarified networking behavior. Updated Python, C#, TypeScript, REST, and hosted agent samples (event names, agent_reference payloads, response validation, citation handling) and improved Custom Search configuration and troubleshooting. Users can choose the right approach and implement with consistent, current samples.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/bing-tools

- **Automate browser tasks with the Browser Automation tool (preview)**

  Tightened role guidance and least-privilege setup, restored usage/how-it-works structure, and standardized headings. Updated Python, TypeScript, hosted agents, and REST samples to current APIs (toolboxes.create_version, BrowserAutomationPreviewToolboxTool, agent_reference) and authorization practices. These updates make setup safer and examples more accurate.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/browser-automation

- **Code Interpreter tool for Microsoft Foundry agents**

  Overhauled Python, C#, TypeScript, and REST samples to generate/upload temporary CSVs, use toolbox-based tools, and align payloads with agent_reference while standardizing token acquisition and headers. Clarified usage support, normalized labels, and refined prompts and outputs. Developers get cleaner, end-to-end examples that mirror real-world workflows.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/code-interpreter

- **Configure a custom code interpreter for agents**

  Expanded prerequisites, infrastructure outputs, and environment mapping, and clarified toolbox requirements even when using project connections. Updated SDKs to create_version APIs and Toolbox tool types across languages, aligned REST payloads to agent_reference, and added version cleanup steps. Better guidance reduces deployment errors and streamlines version management.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/custom-code-interpreter

- **How to use the Deep Research tool (classic)**

  Reworked content to focus on maintaining classic agents, added retirement timelines, and directed users to current alternatives. Updated language-specific prerequisites, corrected schemas, improved polling and output handling, and added thorough troubleshooting. This helps teams keep legacy paths functional while planning migrations.

  https://learn.microsoft.com/en-us/azure/foundry-classic/agents/how-to/tools-classic/deep-research-samples

- **Use the Microsoft Fabric data agent (preview)**

  Added capacity requirements and tenant settings, clarified regional constraints, and eased permissions by lowering the minimum Power BI semantic model permission to Read. Updated TypeScript samples to use agent_reference and repositioned usage support. This improves deployment planning and reduces permission friction.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/fabric

- **Connect agents to Microsoft Fabric with Fabric IQ (preview)**

  Added a quickstart for first queries, expanded prerequisites and authentication options (including data agent MCP), and modernized code samples across languages. Strengthened governance, data residency, and compliance guidance and documented private endpoint connectivity. These changes make connecting to Fabric more secure, predictable, and aligned with enterprise controls.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/fabric-iq

- **File search tool for agents**

  Introduced an end-to-end quickstart for uploading, ingesting, attaching, verifying, and cleaning up files. Updated role requirements, normalized headings, modernized SDK/REST patterns (toolboxes.create_version, FileSearchToolboxTool, agent_reference, Authorization headers), and clarified tokens. The result is a clearer, safer path to enable file-grounded experiences.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/file-search

- **Use the image generation tool (preview)**

  Updated prerequisites (gpt-image-1 access and regions) and standardized orchestrator examples to gpt-5. Refreshed multi-language samples to current APIs and payloads (agent_reference) with robust image handling and added REST cleanup steps, while clarifying when to prefer the Image API. This brings samples up to date and improves guidance for production use.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/image-generation

- **Create and use memory in Foundry Agent Service**

  Added a scenario-based getting-started path, strengthened RBAC, and broadened examples, including direct remember/forget commands. Updated JavaScript/TypeScript and Python samples to current SDKs (Node.js 22+, @azure/ai-projects 2.4.0, agent_reference) and refined retrieval guidance. These updates make memory usage clearer and easier to implement.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/memory-usage

- **Migrate to the new Foundry Agent Service**

  Added a decision guide and a minimum migration checklist for moving from Assistants API or classic agents. Standardized client usage across languages (project.getOpenAIClient / ProjectOpenAIClient), introduced Node.js 22+ and @azure/ai-projects 2.4.0 guidance, and updated samples to new namespaces and method patterns. This reduces migration risk and accelerates adoption of the new runtime.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/migrate

- **Connect agents to MCP server endpoints**

  Restructured to a task-based flow with clear first-success and secondary paths, updated roles and authentication, and integrated project connections for MCP credentials. Modernized SDK/REST samples to use Toolbox tool types, create_version APIs, agent_reference payloads, and added background mode guidance with updated polling. This improves correctness, security, and support for long-running operations.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/model-context-protocol

- **Connect agents to OpenAPI tools**

  Added an anonymous first-success flow for quick validation, expanded prerequisites and least-privilege identity, and repositioned usage support. Updated hosted, REST, and TypeScript samples (agent_reference, secure env vars, Authorization headers), clarified API key vs bearer token patterns, and improved managed identity guidance. Teams can onboard faster with safer, reproducible configurations.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/openapi

- **Build with runtime components in Foundry Agent Service**

  Reframed the article around agents, conversations, and responses with a relationship table and lifecycle example. Modernized JavaScript, .NET, and Java samples to current clients/APIs (Node.js 22+, @azure/ai-projects 2.4.0, agent_reference request bodies, updated .NET types, refined Java polling). This clarifies component choices and aligns examples with the latest SDKs.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/runtime-components

- **Get started with Microsoft Foundry SDKs and endpoints**

  Overhauled the getting-started flow with updated SDK versions and Node.js 22+ requirement, standardized first-call examples across languages, and clearer OpenAI/Anthropic SDK guidance with bearer token auth. Additionally, the classic SDK page marks Java as retired and directs users to the current Foundry SDK. These changes simplify setup, align examples to modern patterns, and guide users away from deprecated paths.

  https://learn.microsoft.com/en-us/azure/foundry/how-to/develop/sdk-overview

- **Use SharePoint with the Foundry Agent Service API**

  Added delegated user authentication setup and verification steps for permission-trimmed retrieval across users. Updated streaming event names, REST response schema, and TypeScript payloads (agent_reference), and clarified environment variables and single-tool-per-agent guidance. This enables secure, identity-aware SharePoint access with consistent API usage.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/sharepoint

- **Use skills with Microsoft Foundry agents (preview)**

  Introduced an end-to-end skill workflow from authoring to version management, updated SDK and REST APIs (toolboxes.create_version, standardized numeric versioning), and clarified CLI replacement behavior. Improved security guidance for hosted agent samples and expanded troubleshooting. This makes skill lifecycle management predictable and easier to automate.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/skills

- **Speech containers overview**

  Added a Fast transcription container entry with capabilities and preview availability, including links to reference tags. This helps teams evaluate high-speed transcription scenarios and plan container deployments.

  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/speech-container-overview

- **Create and manage a toolbox in Microsoft Foundry**

  Major restructuring with a quick path, updated feature tables, and corrected endpoint patterns. Standardized SDK APIs and tool types across languages, added verification workflows using MCP client SDKs, and expanded integration guidance (LangGraph, Agent Framework, Copilot SDK, .NET ResponsesServer). These updates make toolbox creation, validation, and integration more reliable.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/toolbox

- **Tutorial: Add Search to a C# Web App**

  Retargeted deployment to Azure Container Apps with azd, Bicep-based infra, and automatic index seeding. Switched to a containerized Azure Functions API and made managed identity the default for Azure AI Search. This modernizes the deployment path and simplifies secure authentication.

  https://learn.microsoft.com/en-us/azure/search/tutorial-csharp-overview

- **Explore Azure AI Search query integration in a C# app**

  Rewrote the tutorial to emphasize query integration and managed identity defaults, introducing a shared SearchClientFactory using DefaultAzureCredential and user-assigned identity targeting. Clarified environment settings, functions, React client integration, and verification steps, with an option to switch to key-based auth. This improves security and developer ergonomics for local and cloud runs.

  https://learn.microsoft.com/en-us/azure/search/tutorial-csharp-search-query-integration

- **Automate agents with routines (preview)**

  Added a quick-start for scheduled routines, a trigger/action decision guide, and stricter, timezone-aware timer semantics. Standardized SDK requirements and method names, normalized Teams trigger parameters, and expanded action schemas and dispatch behavior, with extensive troubleshooting. The updates make automation more predictable and enterprise-ready.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/use-routines

- **Web search tool**

  Introduced a scenario selector, clarified direct-agent vs toolbox usage, and updated RBAC with Entra PIM. Updated samples across languages to modern APIs (create_version, agent_reference) and added a deep research path using the direct WebSearchPreviewTool. REST examples now include authorization and improved output structures for easier implementation and governance.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/web-search

- **Connect agents to Microsoft 365 with Work IQ (preview)**

  Added a commercial requirements matrix, a dependency map for setup, and expanded prerequisites including PIM-based admin activation and protocol headers. Modernized code samples and strengthened Entra app setup, connection steps, and governance guidance, including data residency and privacy considerations. Troubleshooting now covers billing, consent, audience, and indexing issues for smoother deployments.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/work-iq

## Moderate Changes

- **Agent2Agent (A2A) authentication**

  Added an option to send credentials when fetching the agent card via send_credentials_for_agent_card with clear HTTPS and host-matching constraints. Included a caution on when to enable it and a new troubleshooting entry for 401s that require the flag.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/agent-to-agent-authentication

- **Bring your own model to Foundry Agent Service**

  Expanded configuration guidance for AI Gateway base URLs across protocol styles and clarified routing. Added instructions for selecting API key sources/headers by topology and detailed monitoring in Azure API Management with Application Insights and Kusto queries.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/ai-gateway

- **What are Foundry Tools containers?**

  Added a Speech API Fast transcription container entry with capabilities and preview status, plus a reference link. This enables quicker discovery and evaluation of the new container.

  https://learn.microsoft.com/en-us/azure/ai-services/cognitive-services-container-support

- **Use the computer use tool for agents**

  Reorganized guidance and pointed to maintained samples, adding an approval-based safety workflow with pending_safety_checks and acknowledged_safety_checks in SDK examples. Clarified helper utilities vs. application-owned execution and fixed TypeScript payloads to use agent_reference.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/computer-use

- **What are hosted agents?**

  Clarified that hosted agents access tools via a Toolbox MCP endpoint and expanded the supported tools list. Consolidated authentication options and reinforced connecting via standard MCP client libraries to simplify architecture decisions.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/hosted-agents

- **Enable tool search in a toolbox**

  Updated SDKs to non-beta createVersion APIs and Toolbox tool types, and expanded verification steps to ensure only pinned tools are discoverable alongside tool_search and call_tool. Removed the Foundry-Features header requirement and corrected OAuth consent error code.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/tool-search