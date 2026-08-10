# Microsoft Foundry
**Date created:** 2026-07-11 UTC  
**Tags:** Administration, Agent, AI, Governance, Programming, Security  

## Major Changes

- **Quickstart: Build a toolbox and use it with a hosted agent**

  Added detailed pivots for Python and .NET showing how to build a toolbox with the Foundry SDK, including package setup, retrieving the project endpoint from azd, and complete code samples that add web search and the Microsoft Learn MCP server. Clarified how to set the MCP endpoint as the TOOLBOX_ENDPOINT environment variable. These updates give developers clearer, end-to-end steps to get a toolbox running with a hosted agent and verify the versioned MCP endpoint. Minor improvements in the VS Code flow make the setup more predictable.

  https://learn.microsoft.com/en-us/azure/foundry/agents/quickstarts/quickstart-toolbox-agent

## Moderate Changes

- **Workspace managed virtual network isolation**

  Added guidance to use managedNetworkKind v1 when enabling managed virtual networks and to avoid v2 because it remains in preview. This steers production deployments toward a stable configuration and reduces risk from preview features.

  https://learn.microsoft.com/en-us/azure/machine-learning/how-to-managed-network?view=azureml-api-2

- **Instant access to models in Microsoft Foundry (preview)**

  Removed the static list of example instant models and directed readers to the Supported models section for an authoritative, up-to-date catalog. Refined portal navigation steps, including paths from Home, Explore models/Discover > Models, selecting an instant access model, opening its playground, and using the Model dropdown to switch between instant access and deployed models, making the workflow clearer and easier to follow.

  https://learn.microsoft.com/en-us/azure/foundry/concepts/instant-models

- **Quickstart: Set up your first Foundry resource**

  Expanded the introduction to define the Foundry resource as the primary, managed boundary for identity, access, networking, security, billing, and monitoring with a unified endpoint and key for Azure OpenAI and Foundry Tools. Reworked Access and Verify to focus on Azure portal, CLI, and PowerShell, adding step-by-step verification and commands to confirm provisioning and endpoint details, and removed SDK-based verification. Clarified least-privilege RBAC guidance and streamlined role assignment instructions for the Azure portal, with minor description cleanups in the bundled services table.

  https://learn.microsoft.com/en-us/azure/ai-services/multi-service-resource

- **Publish agents to Microsoft 365 Copilot and Microsoft Teams in the Foundry portal**

  Added an IMPORTANT notice highlighting Early Access Preview terms and data-handling responsibilities, including third-party services and compliance considerations. Updated role requirements to explicitly include the Azure Bot Service Contributor role for creating and configuring bot resources, and aligned troubleshooting to resolve authorization errors by assigning this role when needed.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/publish-copilot

- **Publish agents to Microsoft 365 Copilot and Microsoft Teams by using the REST API + VNet Guidance**

  Added an IMPORTANT notice covering Early Access Preview licensing and data responsibilities, including third‑party and compliance implications. Clarified required permissions and examples (Azure Bot Service Contributor, Contributor, Owner) for creating the bot resource and channels, and refined troubleshooting for 403 AuthorizationFailed errors to recommend assigning the appropriate role on the target resource group.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/publish-copilot-virtual-network