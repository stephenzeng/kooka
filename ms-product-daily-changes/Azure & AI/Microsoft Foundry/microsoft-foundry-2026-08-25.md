# Microsoft Foundry
**Date created:** 2026-08-25 UTC  
**Tags:** Automation, Best Practices, Configuration, Get Started, Guidance, Identity, Monitoring, Security, Troubleshooting  

## Major Changes

- **Connect an Azure AI Search index to Foundry agents**
  Updated end-to-end integration guidance and samples across Python, .NET, JavaScript/TypeScript, and Java to adopt new Foundry toolbox patterns and authentication. Clarified RBAC by requiring the Foundry account’s managed identity on the search service with explicit role assignments, and updated REST and SDK request schemas (for example, agent_reference). These changes align samples to current SDKs, simplify auth, and improve security posture.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/ai-search

- **Use Azure Functions with Foundry Agent Service**
  Overhauled Azure Functions integration to the queue-based pattern with clear prerequisites, storage queue setup via Azure CLI, and required role assignments. Renamed types, refreshed multi-language samples, and modernized REST examples (agent_reference payloads, openai/v1/responses endpoint). These updates streamline configuration, improve security, and align samples with the latest SDK versions.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/azure-functions

- **Automate browser tasks with the Browser Automation tool (preview)**
  Strengthened prerequisites and security guidance (token storage, rotation, and revocation) and clarified role assignment using the Foundry project identity. Rewrote hosted agent samples to adopt Foundry toolbox integrations in Python and .NET, reducing custom auth and client code. These changes improve secure operations and simplify integration.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/browser-automation

- **Code Interpreter tool for Microsoft Foundry agents**
  Replaced legacy MCP-based patterns with streamlined Foundry toolbox integrations in Python and .NET, removing custom token providers and server wiring. Updated hosting to use AddFoundryToolboxes/AddFoundryResponses and simplified agent initialization. The new approach reduces boilerplate and standardizes how agents attach and invoke tools.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/code-interpreter

- **Deploy a steerable agent (preview)**
  Reworked the how-to to use a Responses protocol agent with resilience and steering, removing prior client-based workflows. Simplified setup with azd commands and consolidated provisioning/deployment, and added scenarios for stored background responses, session reuse, and monitoring. This modernizes the example, reduces prerequisites, and demonstrates steering with reliable background execution.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/deploy-steerable-agent

- **Use the image generation tool (preview)**
  Tightened prerequisites (Foundry User role) and updated Python version requirements. Standardized request schemas to use agent_reference and documented Java client limitations, advising REST for invocation; also bumped Java SDK versions. These changes clarify required permissions, improve sample accuracy, and align with current APIs.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/image-generation

- **Connect agents to OpenAPI tools**
  Added region/model support checks and comprehensive security best practices for credential handling and rotation. Replaced custom MCP and auth code with Foundry toolbox integrations in Python and .NET, and aligned role guidance to least privilege. The updates improve security, simplify setup, and modernize hosted agent patterns.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/openapi

- **Web search tool**
  Rebuilt hosted agent examples to use FoundryToolbox in Python and Microsoft Agent Framework integrations in .NET, removing custom auth and MCP client wiring. Standardized package guidance and minimal hosting setup to streamline discovery and invocation. This modernizes integration and reduces complexity for tool use in hosted agents.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/web-search

## Moderate Changes

- **Connect to an A2A agent endpoint from Foundry Agent Service (preview)**
  Updated hosted agent samples to adopt FoundryToolbox (Python) and AddFoundryToolboxes (C#), replacing custom HTTP auth and client wiring. This streamlines toolbox discovery and invocation while preserving existing A2A functionality.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/agent-to-agent

- **Work with chat completion models**
  Added a JavaScript/TypeScript section with prerequisites (Node.js 22+, Entra authentication via Azure CLI, environment variables) and code samples via include. Python and C# guidance remains unchanged.
  https://learn.microsoft.com/en-us/azure/foundry/openai/how-to/chatgpt

- **Use the computer use tool for agents (preview)**
  Introduced a required safety-approval flow that pauses execution until pending checks are acknowledged, with updated code enforcing this behavior. Added region/model prerequisites and updated API examples to carry acknowledged_safety_checks; also upgraded Java dependencies. These changes strengthen safety controls for action execution.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/computer-use

- **Add managed MCP servers powered by connector namespaces (preview)**
  Modernized the Python hosted agent sample to use FoundryToolbox, removing custom httpx auth and token handling. The simplified setup reduces boilerplate and aligns with the new toolbox integration model.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/connectors

- **Custom code interpreter tool for agents (preview)**
  Added region prerequisites for Foundry Agent Service and Azure Container Apps Dynamic Sessions, and adopted Foundry toolbox integrations for Python and .NET. Strengthened security guidance for running untrusted code with least privilege, restricted egress, and approved images; also updated Java dependency versions. These changes improve reliability, security, and ease of integration.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/custom-code-interpreter

- **Deploy a crash-resilient long-running agent (preview)**
  Refocused the how-to on stored background responses with checkpointed stages and crash recovery, simplifying setup via azd commands. The example demonstrates recovery logic, local invocation, and streamlined deployment and monitoring. This makes resilience patterns easier to adopt in production.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/deploy-resilient-agent

- **Connect agents to Microsoft Fabric with Fabric IQ (preview)**
  Replaced manual MCP HTTP tooling with Foundry toolbox integrations in Python and .NET, adopting standard hosting patterns. These updates simplify authentication and reduce custom client code.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/fabric-iq

- **File search tool for agents**
  Updated hosted agent integrations to use AddFoundryToolboxes in .NET and FoundryToolbox in Python, removing custom auth and helper code. The guidance now reflects the standardized toolbox approach for simpler setup.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/file-search

- **What are hosted agents?**
  Clarified toolbox guidance: use FoundryToolbox in Python and AddFoundryToolboxes in .NET, while other runtimes should use standard MCP libraries. This sets clear expectations for supported integration patterns.
  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/hosted-agents

- **Import custom models with Fireworks**
  Added a LoRA requirements section explaining automatic weight merging and unsupported bases, and clarified related guidance. Streamlined model requirements and pointed to Fireworks documentation for current model availability.
  https://learn.microsoft.com/en-us/azure/foundry/how-to/fireworks/import-custom-models

- **Connect agents to Model Context Protocol servers**
  Migrated Python and .NET samples to Foundry toolbox integrations, simplifying dependencies and hosting setup. Updated instructions and environment variables to match the new approach.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/model-context-protocol

- **Use a SharePoint indexer to ingest permission metadata and filter search results based on user access rights (preview)**
  Clarified which Entra IDs to use by aligning both data source and index definitions to the managed identity’s application (client) ID. Updated tables, examples, and troubleshooting to remove incorrect mappings and provide steps to locate the correct ID. This reduces configuration errors and improves security trimming accuracy.
  https://learn.microsoft.com/en-us/azure/search/search-indexer-sharepoint-access-control-lists

- **Security filters for trimming results in Azure AI Search**
  Added a note that non-retrievable fields are not a security mechanism and do not obfuscate content. Reinforced applying document-level security filters on every query.
  https://learn.microsoft.com/en-us/azure/search/search-security-trimming-for-azure-search

- **Search indexes in Azure AI Search**
  Clarified the behavior of the retrievable attribute and documented best practices for handling sensitive fields. The guidance helps avoid unintended disclosure and encourages explicit, minimal attribute configuration.
  https://learn.microsoft.com/en-us/azure/search/search-what-is-an-index

- **Use SharePoint tool with the agent API (preview)**
  Added authentication guidance: use DefaultAzureCredential locally (user sign-in), avoid managed identity/service principal for local runs, and use delegated identity with OBO in production. Documented Microsoft 365 Copilot Retrieval API limits and updated Java dependency guidance. This improves secure, compliant usage across environments.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/sharepoint

- **Customize agent behavior at runtime with structured inputs**
  Added an IMPORTANT notice to avoid passing secrets in structured inputs and to use project connections or secret stores. Improved cURL examples, added validation guidance for OData filters, removed auth_token from schemas, and updated Java dependencies. These changes enhance security and reduce configuration pitfalls.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/structured-inputs

- **How toolbox authentication works in Microsoft Foundry**
  Simplified Python authentication by using FoundryToolbox and DefaultAzureCredential, removing custom HTTP clients and token plumbing. The example now connects via the consumer endpoint to the default toolbox version for a cleaner, more secure setup.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/tool-authentication

- **Tool best practices for Microsoft Foundry Agent Service**
  Emphasized using toolboxes for organizing tools and connections and added a prerequisite for region/model support. Strengthened security by validating structured outputs, restricting operations, and requiring user approval for consequential actions, with reorganized guidance for clarity.
  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/tool-best-practice

- **Create and manage a toolbox in Foundry**
  Updated Python and .NET integrations to use FoundryToolbox and Microsoft.Agents.AI.Foundry.Hosting with AddFoundryToolboxes and hosted responses. Revised environment variables, packages, and troubleshooting (send_ping) to reflect the new approach and reduce custom configuration.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/toolbox