# Microsoft Foundry
**Date created:** 2026-08-01 UTC  
**Tags:** Administration, Agent, AI, Automation, Governance, Programming, Security  

## New Articles

- **Toolbox authentication in Microsoft Foundry**

  New guidance explains how toolbox authentication centralizes connection management and separates per-user versus agent identities. It documents supported auth types (none, custom keys, managed identity, agentic identity, OAuth2, and user Entra token) and when to use each. The article includes Azure Developer CLI commands and an end-to-end OAuth passthrough walkthrough integrating a private MCP server and Work IQ, highlighting consent handling, token isolation, and guardrails.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/tool-authentication

- **What is Toolbox in Microsoft Foundry?**

  Introduces Toolbox as a single MCP-compatible endpoint to manage tools centrally for reuse, authentication, governance, observability, and versioning. It outlines the tool lifecycle (Build, Discover, Consume, Govern), previews capabilities like Tool search and Skills, and provides a supported tools matrix. The article helps teams standardize integration and accelerate adoption with links to getting started resources.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/toolbox-overview

- **Use a toolbox with a hosted agent in Microsoft Foundry**

  Provides a step-by-step guide to connect hosted agents to toolboxes over MCP using Entra authentication. It shows implementation across Python (Agent Framework), LangGraph, and .NET, plus general guidance for REST/JavaScript. The article covers endpoint selection, approval enforcement, environment setup with Azure Developer CLI, and troubleshooting common startup and authorization issues.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/use-toolbox-hosted-agent

## Major Changes

- **Connect to an A2A agent endpoint from Foundry Agent Service (preview)**

  Overhauled guidance to recommend using the A2A tool via toolboxes and MCP integration, replacing older direct patterns. Added migration notes and streamlined samples across Python, C#, TypeScript, REST, and hosted agents, including toolbox creation/attachment and remote-tool connections with user Entra tokens. The update improves clarity on targeting Foundry agents, audience settings, auto-negotiation, and enabling incoming A2A, while modernizing models and workflows.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/agent-to-agent

- **Connect an Azure AI Search index to Foundry agents**

  Shifted to a toolbox-first approach with MCP endpoints for integrating Azure AI Search. Added end-to-end samples across SDKs and REST showing toolbox creation, remote-tool connections, and agent attachment. The restructure standardizes patterns across agent types and clarifies private networking considerations.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/ai-search

- **Automate browser tasks with the Browser Automation tool (preview)**

  Rewrote guidance to promote reusable toolboxes and MCP endpoints for Browser Automation. Added Azure Developer CLI steps, explicit tool definitions, and full samples for Python, C#, TypeScript, REST, and Java integration patterns. The changes consolidate setup, authentication, and attachment into a consistent, toolbox-based workflow.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/browser-automation

- **Code Interpreter tool for Microsoft Foundry agents**

  Adopted a toolbox-based pattern across languages to package and attach Code Interpreter via MCP endpoints. Expanded hosted-agent samples, REST workflows (including resource-level file upload and step ordering), and added a note that user isolation isn’t supported for hosted agents using toolboxes. The update simplifies integration and aligns patterns across Python, .NET, TypeScript, Java, and REST.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/code-interpreter

- **Add managed MCP servers powered by connector namespaces (preview)**

  Introduces toolbox patterns to add managed MCP servers from connectors and reuse them across agents. Provides Python examples for both prompt and hosted agents, highlights Azure Developer CLI flows, and emphasizes preferring toolboxes when connecting to MCP servers. This enables centralized authentication and simpler lifecycle management.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/connectors

- **Custom code interpreter tool for agents (preview)**

  Refactors to a toolbox-first workflow for hosting the custom code interpreter MCP server. Adds multi-language samples to create the toolbox, derive MCP endpoints, configure auth, and attach to agents, including hosted-agent patterns. The guidance streamlines setup and aligns with standardized remote-tool connections.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/custom-code-interpreter

- **Document translation SDKs**

  Major expansion of the Document Translation SDK overview with updated prerequisites and supported languages. Adds Java SDK 2.0.0 alongside .NET and Python, with installation, client builders, and examples for batch and single-document translation. Updates Python to 2.0.0 and refreshes code snippets, default API versions, and storage guidance for more reliable end-to-end scenarios.

  https://learn.microsoft.com/en-us/azure/ai-services/translator/document-translation/document-sdk-overview

- **Connect agents to Microsoft Fabric with Fabric IQ (preview)**

  Recommends toolbox-based integration via MCP endpoints for Fabric IQ and documents environment variables, URL patterns, and auth. Adds comprehensive samples for prompt and hosted agents across Python, .NET, JavaScript, and REST, including remote-tool connections using user Entra tokens. The update clarifies setup, multi-step workflows, and where annotations are returned.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/fabric-iq

- **File search tool for agents**

  Moves to a toolbox-first model that creates a vector store, packages File Search in a toolbox, exposes an MCP endpoint, and attaches it to agents. Adds full samples across Python, .NET, TypeScript, Java, and REST, plus guidance for resource-level uploads and runtime vector store selection. Notes limitations (no user isolation for hosted agents using toolboxes) and emphasizes data control with Azure AI Search.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/file-search

- **Connect agents to Model Context Protocol servers**

  Introduces toolbox-centric integration for MCP servers, with detailed auth configuration across multiple types (none, custom keys, OAuth2, user Entra token, managed identity, agentic identity). Adds YAML toolbox definitions, connection commands, and error handling for consent-required flows, plus preview notes for long-running tasks. Samples across SDKs and REST show creating toolboxes, using MCP endpoints, and attaching tools with approval workflows.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/model-context-protocol

- **Connect agents to OpenAPI tools**

  Reworks guidance to add OpenAPI tools via a toolbox and attach them as MCP tools with standardized auth patterns. Adds hosted-agent samples in Python and C#, TypeScript, and REST workflows that create toolboxes and remote-tool connections, plus an RBAC note for managed identity. Updates the TripAdvisor example to the new toolbox-first flow.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/openapi

- **Document Translation REST API guide (2024-05-01)**

  Repositions 2024-05-01 as a legacy API, clearly separating synchronous single-document and asynchronous batch operations. Clarifies custom domain requirements, refreshes operation tables, and adds discovery operations for formats. Provides migration guidance to the latest 2026-03-01 API and links to related SDKs and overviews.

  https://learn.microsoft.com/en-us/azure/ai-services/translator/document-translation/reference/rest-api-guide

- **Create and manage a toolbox in Foundry**

  Substantially reorganized to cover creation, configuration, agent integration, and version management with a new tools compatibility table and operations matrix. Clarifies RBAC and agent identity prerequisites, endpoint semantics, and approval handling. Adds guardrails configuration, skill attachment, extensive troubleshooting, and consolidates per-tool configuration guidance with links to dedicated articles.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/toolbox

- **Types of tools in Microsoft Foundry Agent Service**

  Retitled and reframed to focus on tool types and a toolbox-first model that centralizes credentials, policy, and reuse via managed MCP endpoints. Clarifies GA versus preview status across tools and replaces direct-attachment examples with a Python sample that creates a toolbox, sets up a remote-tool connection, and attaches it to an agent. The update aligns guidance with modern patterns for scalability and governance.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/tool-catalog

- **Web search tool**

  Overhauls to recommend adding Web Search through a toolbox and attaching it via MCP, with updated samples across Python, C#, TypeScript, REST, and Java guidance. Adds hosted-agent patterns, domain-restricted examples, and a new section describing the MCP response format with URL citations. The changes standardize setup and improve discoverability and governance.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/web-search

## Moderate Changes

- **Agent identity concepts in Microsoft Foundry**

  Corrected the A2A tool configuration to use the auth type AgenticIdentityToken, aligning the documentation with token-based agent identity authentication. This prevents misconfiguration when setting up A2A endpoints.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/agent-identity

- **Tutorial: Idea to prototype - Build and evaluate an enterprise agent**

  Updated dependencies to require azure-ai-projects>=2.3.0 and added azure-identity. Configuration samples now use the new Foundry project endpoint format, reducing setup errors and aligning with current APIs.

  https://learn.microsoft.com/en-us/azure/foundry/tutorials/developer-journey-idea-to-prototype

- **Enable incoming A2A on a Foundry agent**

  Fixed configuration examples by changing authType from "AgenticIdentity" to "AgenticIdentityToken" in REST and PowerShell snippets. This ensures the correct authentication flow for incoming A2A connections.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/enable-agent-to-agent-endpoint

- **Deploy models from Hugging Face hub to Azure Machine Learning online endpoints for real-time inference**

  Updated Python SDK and CLI examples to use correct model identifiers, labels/latest references, and modern MLClient patterns with DefaultAzureCredential. Clarified gated model steps and refined supported model criteria, improving deployment reliability and reducing version pinning issues.

  https://learn.microsoft.com/en-us/azure/machine-learning/how-to-deploy-models-from-huggingface?view=azureml-api-2

- **What is Azure Translator document translation?**

  Expanded SDK guidance by referencing the consolidated client libraries overview and adding Java support alongside .NET and Python. The updates make it easier to choose the right SDK for synchronous and batch scenarios.

  https://learn.microsoft.com/en-us/azure/ai-services/translator/document-translation/overview

- **What is Azure Translator document translation 2026-03-01?**

  Expanded SDK guidance to a consolidated Document Translation client libraries page and added Java support alongside .NET and Python. Updated the synchronous section to reference the client libraries overview for consistent API usage.

  https://learn.microsoft.com/en-us/azure/ai-services/translator/document-translation/latest/overview

- **Quickstart: Build a toolbox and use it with a hosted agent**

  Simplified the sample by constructing the MCP endpoint from the newly created toolbox’s name and version, removing the extra retrieval step. This reduces code and makes versioning behavior explicit in logs.

  https://learn.microsoft.com/en-us/azure/foundry/agents/quickstarts/quickstart-toolbox-agent

- **What's new in Azure Translator?**

  Added a July 2026 entry announcing GA of Document Translation client libraries 2.0.0 for Python and Java with default API version 2026-03-01. Highlights support for both batch and single-document translation and links to SDK guidance.

  https://learn.microsoft.com/en-us/azure/ai-services/translator/whats-new

- **Tutorial 5: Develop a feature set with a custom source**

  Refined the introduction to better describe the managed feature store and corrected the overview of the preceding tutorials and next steps. This clarifies the learning path and improves continuity across the series.

  https://learn.microsoft.com/en-us/azure/machine-learning/tutorial-develop-feature-set-with-custom-source?view=azureml-api-2