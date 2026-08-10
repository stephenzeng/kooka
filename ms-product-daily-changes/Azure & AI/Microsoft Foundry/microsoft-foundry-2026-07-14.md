# Microsoft Foundry
**Date created:** 2026-07-14 UTC  
**Tags:** AI, Agent, Administration, Automation, Azure AI, Programming, Security  

## Major Changes

- **Build a voice agent with hosted agents**

  Removed preview status and updated the WebSocket endpoint to a REST-style path that uses path segments for project and agent plus a required api-version parameter. Increased the maximum WebSocket session duration from about 10 minutes to roughly 30 minutes and updated examples and limits accordingly. Clarified that routing consumes the path segments and api-version at the platform layer. Updated schema references in setup to use protocol_versions and to move image under container_configuration.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/build-voice-agent

- **Hosted agents in Foundry Agent Service**

  Expanded protocol availability, stating that Responses, Invocations, and Invocations (WebSocket) are supported in all regions that offer Hosted agents. Replaced the old query-parameter endpoint with a new REST-style WebSocket path that requires api-version=v1.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/hosted-agents

- **Quickstart: Deploy your first hosted agent**

  Added a complete Python SDK path covering environment setup, packaging source, creating a version from code, configuring routing, invoking via Responses API, and cleaning up. Included guidance for making deployments persistent and new troubleshooting for provisioning failures. Clarified VS Code flow and warnings.

  https://learn.microsoft.com/en-us/azure/foundry/agents/quickstarts/quickstart-hosted-agent

- **Quickstart: Give a hosted agent persistent memory**

  Introduced dual workflows with pivots for Azure Developer CLI and Python SDK. The Python path now provisions a memory store, deploys a hosted agent from code, verifies persisted memory across invocations, and restores routing, with comprehensive cleanup and troubleshooting. Prerequisites and role requirements were clarified to streamline setup.

  https://learn.microsoft.com/en-us/azure/foundry/agents/quickstarts/quickstart-memory-hosted-agent

- **Quickstart: Optimize a hosted agent (preview)**

  Added a full Python SDK workflow including environment setup and a script to create, monitor, and read results from an optimization job, and instructions to apply the best candidate. Clarified differences from the Azure Developer CLI path and expanded troubleshooting and cleanup guidance.

  https://learn.microsoft.com/en-us/azure/foundry/agents/quickstarts/quickstart-optimize-hosted-agent

- **Quickstart: Build a toolbox and use it with a hosted agent**

  Expanded the quickstart with dual paths for Python SDK and VS Code/Azure Developer CLI. Added end-to-end Python scripts to create a toolbox (including MCP endpoints), package and deploy a hosted agent version, route traffic temporarily, invoke it, and restore configuration. Updated verification, cleanup options, and replaced older snippets with current Python SDK APIs.

  https://learn.microsoft.com/en-us/azure/foundry/agents/quickstarts/quickstart-toolbox-agent

## Moderate Changes

- **Add Microsoft Foundry to a network security perimeter**

  Removed the preview notice for Network Security Perimeter support, indicating the feature is no longer in preview. This signals broader readiness and fewer preview-specific limitations.

  https://learn.microsoft.com/en-us/azure/foundry/how-to/add-foundry-to-network-security-perimeter

- **Add a content safety guardrail to a hosted agent**

  Updated API examples to nest the container image under container_configuration.image and renamed container_protocol_versions to protocol_versions. These schema changes align samples with current SDK and REST behavior.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/add-hosted-agent-guardrails

- **Add a new connection to your project**

  Revised the UI flow to start from the Connected resources tab in the bottom section before selecting Add connection. Navigation steps were updated to match the latest interface.

  https://learn.microsoft.com/en-us/azure/foundry/how-to/connections-add

- **Azure OpenAI image generation models**

  Added guidance that listed size constraints apply only when a specific size is set; with size=auto, outputs may not follow those constraints. This helps set expectations for image dimensions.

  https://learn.microsoft.com/en-us/azure/foundry/openai/how-to/dall-e

- **Deploy a hosted agent**

  Removed a preview and region-limitation note for the invocations_ws protocol, indicating broader availability or general release. No procedural changes were required.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/deploy-hosted-agent

- **Deploy a hosted agent from source code (preview)**

  Added guidance and examples for using the Invocations (WebSocket) protocol across SDKs and REST, including Python, .NET, and JSON metadata. Included a note on connecting via WebSocket and a reference to the voice agent documentation.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/deploy-hosted-agent-code

- **Tutorial: Deploy private agentic retrieval for Foundry IQ**

  Updated the model requirement to a GPT-5 family model in the deployment table. Other components, such as text-embedding-3-large for Azure AI Search, remain the same.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/foundry-iq-tutorial-private-overview

- **Validate end-to-end private agentic retrieval**

  Switched prerequisites and examples from gpt-4.1 to a GPT-5 family model, including deployment checks and JSON placeholders. This aligns the tutorial with current model guidance alongside text-embedding-3-large.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/foundry-iq-tutorial-private-retrieval

- **Manage hosted agents**

  Updated REST and Python examples to reflect the current schema: image now resides under container_configuration.image and container_protocol_versions is renamed to protocol_versions. Examples cover both stable and draft version creation.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/manage-hosted-agent

- **Role-based access control for Microsoft Foundry**

  Clarified that agent-scope role assignments control endpoint access for a specific agent and aren’t evaluated for broader control-plane permissions. Reinforced alignment with Azure RBAC mechanics while noting the current evaluation scope.

  https://learn.microsoft.com/en-us/azure/foundry/concepts/rbac-foundry

- **Supported Regions**

  Added the Serverless pricing model to the regional features table, noting pay-per-request billing and preview availability in West Central US, Switzerland North, and Japan East. This helps customers plan deployments using the new pricing model.

  https://learn.microsoft.com/en-us/azure/search/search-region-support

- **Choose a pricing model and service tier in Azure AI Search**

  Added a section listing preview regions for the Serverless pricing model: West Central US, Switzerland North, and Japan East. This clarifies where the model can currently be adopted.

  https://learn.microsoft.com/en-us/azure/search/search-sku-tier