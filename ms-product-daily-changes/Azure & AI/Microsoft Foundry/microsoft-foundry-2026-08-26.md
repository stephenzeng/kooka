# Microsoft Foundry
**Date created:** 2026-08-26 UTC  
**Tags:** Compliance, Configuration, Deprecation, Get Started, Governance, Guidance, Monitoring, Security  

## New Articles

- **Customer-Managed Key Encryption in Microsoft Foundry**

  Introduced core concepts for using customer-managed keys (CMK) to control encryption for Foundry data at rest, including supported capabilities and key lifecycle governance. Clarifies coverage across persistent stores versus ephemeral runtime compute, with explicit behavior for model hosting, inference, training, caching, and data deletion. Details service-by-service support and prerequisites such as bring-your-own storage for specific workloads and regional constraints. Explains operational impact of key revocation and links to configuration and bring-your-own storage guidance.

  https://learn.microsoft.com/en-us/azure/foundry/concepts/customer-managed-keys

- **Microsoft Foundry Toolkit for Visual Studio Code overview**

  Introduced an overview for the unified Foundry Toolkit in VS Code, consolidating prior AI Toolkit and Foundry experiences. Describes end-to-end workflows for model discovery, evaluation, fine-tuning, and profiling; agent development and debugging with MCP support; and deployment and operations through Foundry Agent Service. Outlines workspace areas (My Resources, Developer Tools, Help and Feedback) and links to install, setup, and changelog resources, noting preview experiences where applicable.

  https://learn.microsoft.com/en-us/azure/foundry/how-to/develop/get-started-projects-visual-studio-code

- **Install Microsoft Foundry Toolkit for Visual Studio Code**

  Added a step-by-step installation guide covering prerequisites, the recommended DevPack path, and alternatives via Marketplace or the Extensions view. Provides post-install verification of the Toolkit view, pointers to What’s New, and cleanup/uninstall instructions. Directs users to next steps for setting up a Foundry project.

  https://learn.microsoft.com/en-us/azure/foundry/how-to/develop/install-foundry-toolkit-visual-studio-code

- **Set up a Microsoft Foundry project in Visual Studio Code**

  Added a how-to for configuring a Foundry project in VS Code, including Azure sign-in, selecting or creating a Foundry account and project, and switching the default project. Clarifies RBAC needs and offers guidance for both basic and customized setups, with cleanup steps and related links.

  https://learn.microsoft.com/en-us/azure/foundry/how-to/develop/set-up-foundry-project-visual-studio-code

## Major Changes

- **Bring your own cross-resource capacity in Content Understanding**

  Expanded setup guidance with explicit prerequisites, permissions, and supported authentication modes. Reworked connection steps to require resource-level Management Center access and replaced “Microsoft Entra ID” with “Account Managed Identity” terminology. Added sections for IAM role assignments and network configuration, including public access and trusted services requirements. Updated architecture, defaults, and examples to clarify authentication paths and deployment configuration.

  https://learn.microsoft.com/en-us/azure/ai-services/content-understanding/how-to/bring-your-own-cross-resource-capacity

- **Azure Content Understanding in Foundry Tools region and language support**

  Removed North Europe (northeurope) from the supported regions list, signaling that the region is no longer available for Content Understanding. This change helps customers avoid deploying to unsupported locations and plan migrations where needed.

  https://learn.microsoft.com/en-us/azure/ai-services/content-understanding/language-region-support

- **What is Microsoft Foundry?**

  Substantially expanded and reorganized the overview to emphasize building AI agents, models, and apps, with guidance on choosing a development approach. Increased the stated model catalog scope and clarified preview features for tools, observability, and platform capabilities with a link to GA scope. Added sections to help new users start with agents, select a developer surface (portal, SDKs, AZD, VS Code, coding agents/MCP), and follow a recommended onboarding path from first model call to adding tools and knowledge.

  https://learn.microsoft.com/en-us/azure/foundry/what-is-foundry

## Moderate Changes

- **Elevated-role tasks in Microsoft Foundry**

  Clarified that small teams must assign the Foundry Account Owner role on the Foundry resource to deploy models and manage quotas, guardrails, and blocklists. Noted upcoming changes to agent publishing and pointed to migration guidance for the new endpoint and experience.

  https://learn.microsoft.com/en-us/azure/foundry/concepts/administrator-guide

- **Agent identity concepts in Microsoft Foundry**

  Added guidance on the transition to the new agent publishing model and directed readers to migration steps. Expanded RBAC details, including assignment methods and corrections for Cosmos DB data-plane roles, and removed a preview label for Logic Apps Standard Operator. Emphasized that published agents have distinct identities with behavior differences in the newer object model.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/agent-identity

- **How to configure network isolation for Microsoft Foundry**

  Updated the firewall allowlist with clearer headers and expanded endpoints for Evaluations & Traces with Application Insights. Added the AzureMachineLearning service tag and provided region-based AML endpoint alternatives, with examples. Clarified entries related to hosted agents.

  https://learn.microsoft.com/en-us/azure/foundry/how-to/configure-private-link

- **Configure Customer-Managed Keys for Microsoft Foundry**

  Retitled and refocused the article on configuring CMK encryption via portal, Bicep, or CLI using Azure Key Vault or Managed HSM. Streamlined the introduction to define CMK scope and referenced a separate coverage overview, removing outdated regional availability notes.

  https://learn.microsoft.com/en-us/azure/foundry/concepts/encryption-keys-portal

- **How to use function calling with Microsoft Foundry Models**

  Shifted guidance from Azure OpenAI specifics to Foundry Models and directed readers to model catalogs to verify capabilities. Clarified support via Chat Completions or Responses API, highlighted tool-related capabilities, and updated notes on tool_choice and description limits.

  https://learn.microsoft.com/en-us/azure/foundry/openai/how-to/function-calling

- **Microsoft Foundry portal general availability overview**

  Refined GA scope to highlight supported enterprise scenarios while noting that monitoring, alerting, and some networking features remain in preview. Updated the readiness table, adding Manage > AI Gateway (Preview) and Manage > Project and resource details (GA), and moved Quota under Manage.

  https://learn.microsoft.com/en-us/azure/foundry/concepts/general-availability

- **Quickstart: Set up Microsoft Foundry resources**

  Raised the minimum Azure CLI version to 2.80.0 and explained new az cognitiveservices account project commands and common error handling. Simplified deployment flow with updated models, regional listing, improved provisioning checks, endpoint retrieval via CLI, and enhanced cleanup verification.

  https://learn.microsoft.com/en-us/azure/foundry/tutorials/quickstart-create-foundry-resources

- **Supported regions for Azure Speech**

  Adjusted the regional support matrix by removing certain feature checkmarks for centralus, eastasia, and westcentralus. This clarifies current feature availability to prevent misconfiguration.

  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/regions

- **Retrieval augmented generation (RAG) and indexes**

  Restructured the guidance to present a clearer RAG workflow and recommended using the Foundry SDK for end-to-end applications. Streamlined sections and terminology, retaining references to agent file search tools.

  https://learn.microsoft.com/en-us/azure/foundry/concepts/retrieval-augmented-generation

- **What's new in Azure Content Understanding in Foundry Tools?**

  Added an August 2026 update announcing the 2026-06-01-preview SDKs with agentic mode, synchronous Read and Layout operations, and analyzer enhancements, plus package links. Also removed North Europe from the regions supporting GPT-5.2 in Content Understanding Studio.

  https://learn.microsoft.com/en-us/azure/ai-services/content-understanding/whats-new