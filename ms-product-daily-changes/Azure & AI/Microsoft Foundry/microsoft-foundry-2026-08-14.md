# Microsoft Foundry
**Date created:** 2026-08-14 UTC  
**Tags:** Best Practices, Billing, Compliance, Configuration, Consumption, Get Started, Governance, Guidance, Identity, Monitoring, Performance, Security, Troubleshooting  

## New Articles

- **Use multi-agent orchestration with the Azure OpenAI Responses API**

  Introduced a new how-to covering when and how to enable multi-agent orchestration in the Responses API, with end-to-end examples in Python and REST. Explained agent coordination, subagent concurrency, hosted actions, developer-defined function calls, and inspection of multi-agent outputs. Detailed HTTP vs WebSocket behaviors, streaming flow via response.inject, and security/governance controls and limitations. Included a troubleshooting section for common errors and links to related guidance.

  https://learn.microsoft.com/en-us/azure/foundry/openai/how-to/responses-multi-agent

- **Azure AI Search Preview Terms**

  Added policy and licensing terms for the 2026-05-01-preview Search Service REST API. Clarified responsibilities and data flow considerations when connecting to Microsoft and third-party services, including potential compliance-boundary implications. Highlighted limitations in recognizing permission changes, CORS-related security risks, and the need for responsible AI practices and application testing. Linked to Azure preview supplemental terms and the Azure AI Search Transparency Note.

  https://learn.microsoft.com/en-us/azure/search/search-preview-terms

## Major Changes

- **Author azure.yaml for hosted agents**

  Raised prerequisite versions for azd and the azure.ai.* extensions and standardized environment variables to MICROSOFT_FOUNDRY_MODEL_DEPLOYMENT_NAME. Added guidance for split-service projects, clarified entryPoint behavior, and introduced an advanced capabilities section covering networking, deployment modes, RAI policies, memory stores, endpoints/protocols, and identity. Updated troubleshooting to reflect the new variable name, helping authors avoid configuration drift and deployment issues.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/author-azure-yaml

- **Foundry Agent Service feature availability in Azure Government**

  Updated Azure Government support to include MCP servers and the OpenAPI tool, enabling broader tool coverage. Removed prior statements that publishing to Teams and Microsoft 365 Copilot isn’t supported, aligning guidance with current capabilities. These changes expand integration options and clarify publishing paths in Gov environments.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/azure-government

- **azure.yaml reference for hosted agents**

  Significantly expanded the reference with versioning requirements, provider lifecycle mapping, private-network settings, agent metadata, RAI policy binding, memory stores, endpoint protocols/authorization, deploy modes, and emitted outputs. Clarified connection timing, toolbox consumption in split-service projects, skills/routines lifecycles, and file include patterns. Standardized environment variables and updated azd behaviors, with comprehensive YAML examples to accelerate correct, secure deployments.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/azure-yaml-reference

- **Enable incoming A2A on a Foundry agent**

  Added Python SDK-based configuration for both agent cards and A2A protocol, replacing earlier guidance that lacked SDK support. The new sample shows end-to-end setup with AgentEndpointConfig and skill metadata, streamlining how teams enable A2A and document agent capabilities programmatically. This reduces manual portal steps and ensures consistent, repeatable configuration.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/enable-agent-to-agent-endpoint

- **Manage hosted agents**

  Expanded Python SDK coverage to create draft versions, enable/disable agents, and stream session logs via SSE, and standardized the client variable naming. Updated examples for listing, creating, deleting, and updating agents and versions, plus endpoint updates. These improvements enable richer automation and observability for managing hosted agents at scale.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/manage-hosted-agent

- **Manage hosted agent sessions**

  Updated SDK usage with breaking changes: removed isolation_key from session operations, introduced VersionRefIndicator for version pinning, changed file upload to accept bytes content, and renamed/standardized session file APIs. These revisions align code with current SDK behavior and reduce confusion around parameters and outputs.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/manage-hosted-sessions

- **Set up MCP server authentication**

  Added detailed OAuth consent and continuation flows with language-specific guidance for Python and C#. Step-by-step instructions and code illustrate obtaining the consent link, prompting authorization, and resuming the conversation with streaming support. This clarifies authentication workflows and accelerates secure tool integrations.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/mcp-authentication

- **Model router for Microsoft Foundry**

  Updated router guidance and regions support across related content: clarified supported regions with a deployment-type matrix, and noted unavailability in select regions for Data Zone Standard. Expanded routing to allow eligible OpenAI, open-source, and Anthropic models for agentic requests based on tool compatibility, supplanting prior OpenAI-only guidance. These changes help teams configure accurate routing pools and plan for regional availability constraints.

  https://learn.microsoft.com/en-us/azure/foundry/openai/concepts/model-router

- **What is Microsoft Foundry Control Plane?**

  Clarified scope and navigation: operational capabilities remain under Operate, while project-scoped settings (Quota and AI Gateway) moved under Manage. Added detail for Project/Resource details, Users, Connected resources, and Projects within Manage. This reorganization helps admins locate controls faster and apply settings at the right scope.

  https://learn.microsoft.com/en-us/azure/foundry/control-plane/overview

- **Quickstart: Deploy your first hosted agent**

  Added a full C#/.NET path using Azure.AI.Projects 2.1.0-beta.4 for source-code deployments, endpoint routing, invocation, and cleanup. Expanded prerequisites, environment setup, and end-to-end Program.cs sample, plus guidance for restoring endpoint configuration and deleting temporary versions. The quickstart now supports both Python and C#, broadening on-ramps for developers.

  https://learn.microsoft.com/en-us/azure/foundry/agents/quickstarts/quickstart-hosted-agent

- **Microsoft Foundry docs: What's new for July 2026**

  Refreshed the monthly roundup with new content across hosted agents, Foundry IQ, models/APIs, observability, and platform notifications. Updated the list of revised topics spanning tool types, A2A connectivity, model endpoints, evaluation, and portal GA overview. This aligns the summary with the latest capabilities and learning paths.

  https://learn.microsoft.com/en-us/azure/foundry/whats-new-foundry

## Moderate Changes

- **Tutorial: Build an Agentic Retrieval Solution**

  Shifted from SharePoint-specific steps to a per-request authorization model using structured inputs and per-user tokens in MCP headers. Added examples for obtaining Azure AI Search tokens and passing them per call, updated Responses API usage, and removed SharePoint-specific code paths. This improves security and reusability by enforcing permissions at invocation time.

  https://learn.microsoft.com/en-us/azure/search/agentic-retrieval-how-to-create-pipeline

- **Bring Your Own Model to Foundry Agent Service**

  Updated portal navigation paths to reflect the new Manage > Resource details flow when adding and verifying Admin-connected model connections. Steps were streamlined across relevant tabs without changing connection specifications. This reduces confusion and aligns instructions with the current UI.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/ai-gateway

- **Connect to your own storage**

  Revised the UI steps to use Manage > Project details > Connected resources before adding a connection. The Azure Storage connection procedure remains the same. This clarifies navigation in the updated portal.

  https://learn.microsoft.com/en-us/azure/foundry/how-to/bring-your-own-azure-storage-foundry

- **Azure Content Understanding skill**

  Standardized preview labeling and disclaimers, marking specific capabilities and parameters as preview and updating tables accordingly. Clarified semantic chunking examples and token-based chunk settings. This makes preview scope explicit for planning and compliance.

  https://learn.microsoft.com/en-us/azure/search/cognitive-search-skill-content-understanding

- **Image Analysis cognitive skill**

  Recommended using the Custom Web API skill for AI Image Analysis API v4+ and removed the prior ImageAnalysisV4 power skill guidance. Minor clarifications improve version selection and implementation paths.

  https://learn.microsoft.com/en-us/azure/search/cognitive-search-skill-image-analysis

- **Configure and share your agent**

  Replaced a placeholder note with a working Python example using AIProjectClient to update agent cards. Demonstrated updating version, description, skills, tags, and examples. This enables scripted, consistent metadata management.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/configure-agent

- **Configure Claude Code for Microsoft Foundry**

  Added claude-opus-4-8 to the Model Router supported models list and adjusted ordering. Keeps the catalog current for routing configurations.

  https://learn.microsoft.com/en-us/azure/foundry/foundry-models/how-to/configure-claude-code

- **How to configure network isolation for Microsoft Foundry**

  Updated the support matrix to show the File Search tool is now supported via private endpoint. Expands private networking coverage for secured deployments.

  https://learn.microsoft.com/en-us/azure/foundry/how-to/configure-private-link

- **Add a new connection to your project**

  Clarified that Copilot Studio Environment connections are created via Manage > Project details > Connected resources, replacing older Operate/Admin paths. Simplifies finding the correct entry point for connections.

  https://learn.microsoft.com/en-us/azure/foundry/how-to/connections-add

- **Deployment types for Microsoft Foundry Models (classic)**

  Refactored deployment-type content into clearer, modular sections with comparisons, selection guidance, workload patterns, and detailed deployment info, incorporating Foundry-specific context where applicable. Improves readability and helps teams choose the right deployment path.

  https://learn.microsoft.com/en-us/azure/foundry-classic/foundry-models/concepts/deployment-types

- **Configure AI Gateway in your Foundry resources**

  Updated navigation to Manage > AI Gateway and aligned troubleshooting with the new pane, including token-limit configuration location and wording improvements. This keeps operational steps consistent with the portal.

  https://learn.microsoft.com/en-us/azure/foundry/configuration/enable-ai-api-management-gateway-portal

- **Use the Microsoft Fabric data agent (preview)**

  Revised navigation for connecting a Fabric data agent to use Manage > Project details > Connected resources. Aligns instructions with the current UI.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/fabric

- **Connect a Foundry IQ knowledge base to Foundry Agent Service**

  Replaced SharePoint-specific instructions with a generalized, per-request authorization model using structured inputs and x-ms-query-source-authorization. Added Python and REST examples for defining structured inputs, obtaining user tokens, and passing headers per invocation, with guidance on per-request header overrides. This strengthens permission enforcement and avoids hardcoded secrets.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/foundry-iq-connect

- **Enforce token limits for models**

  Updated steps and references to the Manage > AI Gateway pane, replacing prior Admin console navigation. Clarified where to configure and monitor token limits. Reduces friction when applying governance controls.

  https://learn.microsoft.com/en-us/azure/foundry/control-plane/how-to-enforce-limits-models

- **Foundry Agent Service limits, quotas, and regional support**

  Expanded the regional availability table to include additional regions and updated tool availability. Helps planners assess where features are supported.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/limits-quotas-regions

- **Model router for Microsoft Foundry (classic)**

  Added a Supported regions section with deployment-type availability per region and a note that available models depend on underlying regional support. Assists with regional rollout planning and expectations.

  https://learn.microsoft.com/en-us/azure/foundry-classic/openai/concepts/model-router

- **Use model router for Microsoft Foundry**

  Clarified that agentic requests can route to eligible OpenAI, OSS, and Anthropic models based on tool and deployment compatibility, replacing earlier OpenAI-only guidance. Points readers to the tool support matrix, improving routing configuration accuracy.

  https://learn.microsoft.com/en-us/azure/foundry/openai/how-to/model-router

- **Model router for Microsoft Foundry**

  Clarified Supported regions with a matrix showing where Global Standard and Data Zone Standard are available, and added a legend. Helps avoid misconfigurations in regions without Data Zone Standard.

  https://learn.microsoft.com/en-us/azure/foundry/openai/concepts/model-router

- **Use model router with Foundry agents**

  Updated guidance on tool compatibility and routing pools, removing a blanket “all tools” claim and pointing to a compatibility matrix by region and model. Added instructions for including Claude models by deploying them and adding them to the router pool. Aligns expectations and setup for multi-model agent routing.

  https://learn.microsoft.com/en-us/azure/foundry/openai/how-to/model-router-agents

- **Monitor agent health and performance across your fleet**

  Revised navigation to use Manage > Project details and confirmed Application Insights under Connected resources, with updated alt-text. Keeps monitoring steps aligned with the portal.

  https://learn.microsoft.com/en-us/azure/foundry/control-plane/monitoring-across-fleet

- **Migrate from the Foundry (classic) portal**

  Updated the portal map: introduced the Manage section for quota, AI Gateway, and project/resource details; refined Operate’s role; and adjusted the mapping table for quota, users, projects, and connected resources. Eases transition to the new portal layout.

  https://learn.microsoft.com/en-us/azure/foundry/how-to/navigate-from-classic

- **Connect agents to OpenAPI tools**

  Updated the TripAdvisor tool connection steps to use the Foundry UI path Manage > Project details > Connected resources tab. Terminology and navigation now match the current portal.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/openapi

- **Role-based access control for Microsoft Foundry**

  Updated role-assignment steps to the Manage pane, detailing navigation to Project details > Users and Resource details for resource-level roles. Clarified role assignment options across Foundry portal, Azure portal IAM, and Azure CLI. This streamlines access management.

  https://learn.microsoft.com/en-us/azure/foundry/concepts/rbac-foundry

- **Register and manage custom agents**

  Updated Control Plane navigation to Manage > AI Gateway and Manage > Project details > Connected resources for observability setup. Clarified screenshots and labels, reducing confusion in configuration and verification steps.

  https://learn.microsoft.com/en-us/azure/foundry/control-plane/register-custom-agent

- **Try Azure AI Search for free**

  Separated Dedicated vs Serverless pricing models, clarifying Free/Basic tiers under Dedicated and updated Serverless Developer (Preview) guidance to use the Scale + Cost tab once billing starts. Helps users estimate costs accurately and choose the right tier.

  https://learn.microsoft.com/en-us/azure/search/search-try-for-free

- **Optimize costs for the Serverless pricing model in Azure AI Search**

  Expanded compute and billing guidance: active index compute, inactivity window, and storage billing; added orchestration cost note for agentic retrieval. Introduced how index and vector sizes drive compute, replaced the per-request header with x-ms-azs-compute-units-consumed, and recommended combining header data with Azure Monitor metrics and the Scale + Cost tab. Added robust optimization practices for indexers and queries to control spend.

  https://learn.microsoft.com/en-us/azure/search/serverless-cost-optimization

- **Create and manage a toolbox in Foundry**

  Added a Virtual network support section covering how toolbox tools behave under private link, including traffic flows and file I/O, with a link to full isolation setup. Reordered Troubleshoot for better flow. Improves planning for secure, network-isolated deployments.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/toolbox

## Minor Changes

- **Configure and share your agent**

  Updated the Python example to show patching an agent card with the current SDK, replacing a prior unsupported note. Enables quick metadata updates via code.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/configure-agent