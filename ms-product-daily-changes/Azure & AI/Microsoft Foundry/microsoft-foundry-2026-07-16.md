# Microsoft Foundry
**Date created:** 2026-07-16 UTC  
**Tags:** Administration, Agent, AI, Automation, Governance, Programming, Security  

## Major Changes

- **Manage hosted agents**
  Replaced the legacy protocols array with a protocol_configuration object across CLI and SDK examples to standardize endpoint setup. Updated Python SDK usage to AgentEndpointConfig with ProtocolConfiguration and ResponsesProtocolConfiguration, and removed AgentEndpointProtocol. Switched the update method from project.beta.agents.patch_agent_details to project.agents.update_details, aligning samples with current APIs. These changes simplify configuration and reduce breaking points as the platform evolves.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/manage-hosted-agent

- **Quotas and limits for Azure Speech**
  Lowered the default real-time text-to-speech throughput for Standard (S0) from 200 TPS to 30 TPS across documentation sections, including standard/custom voices and training scenarios. Adjusted guidance to reflect 30 TPS as the typical default, removing previous references to 32 and 200 TPS. This update helps teams plan capacity and load testing based on the new baseline limits.
  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/speech-services-quotas-and-limits

## Moderate Changes

- **Add a content safety guardrail to a hosted agent**
  Updated code samples to use AgentEndpointProtocol instead of AgentProtocol, and clarified ProtocolVersionRecord usage with AgentEndpointProtocol.RESPONSES when setting responses versions. These updates keep examples aligned with the latest SDK APIs.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/add-hosted-agent-guardrails

- **Bring Your Own Model to Foundry Agent Service**
  Expanded setup guidance for connecting models via enterprise AI gateways, including updated portal navigation, authentication header patterns, and managed identity audience usage. Introduced clearer model configuration fields (Name, Display name, optional Version), added screenshots, and aligned troubleshooting with the Admin-connected models workflow. These improvements reduce setup errors and streamline onboarding multiple models.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/ai-gateway

- **Quickstart: Asynchronous document translation**
  Renamed the option for translating text inside images in Office documents from translateWithinImage to translateTextWithinImage. This clarifies the parameter’s purpose and aligns samples with the current API.
  https://learn.microsoft.com/en-us/azure/ai-services/translator/document-translation/latest/quickstarts/asynchronous

- **Getting started with Browser automation tool (preview) in Hosted agents**
  Refined the setup flow by adding --deploy-mode container to initialization commands, introducing environment-based provisioning of Playwright service settings, and requiring a role assignment for the project’s managed identity. Renamed steps and adjusted numbering to make testing in the Foundry Playground a distinct final step. These changes make provisioning reproducible and permissions explicit.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/browser-automation-hosted-agent-quickstart

- **Configure and share your agent**
  Replaced the protocols array with a protocol_configuration object across REST and Python examples, and updated SDK types and methods (AgentEndpoint -> AgentEndpointConfig, new ProtocolConfiguration classes, agents.update_details). Simplified Entra authorization by removing isolation_key_source and updated documentation tables accordingly. Clarified required Foundry roles to distinguish who can create/manage versus consume agents, improving governance and setup accuracy.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/configure-agent

- **Deploy a hosted agent**
  Updated Python samples to adopt AgentEndpointProtocol in place of AgentProtocol and to set ProtocolVersionRecord using RESPONSES, INVOCATIONS, and INVOCATIONS_WS enums. This aligns deployment examples with the current SDK and protocol versioning scheme.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/deploy-hosted-agent

- **Enable incoming A2A on a Foundry agent (preview)**
  Shifted endpoint configuration from a protocols array to a protocol_configuration object across REST, PowerShell, and Python examples. Updated Python to use AgentEndpointConfig with ResponsesProtocolConfiguration and A2AProtocolConfiguration, changed the update method to agents.update_details, and increased the azure-ai-projects package minimum to >=2.3.0. These updates modernize samples and ensure compatibility with newer SDK versions.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/enable-agent-to-agent-endpoint

- **Hosted agent runtime contract**
  Documented how platform headers are exposed and accessed in AgentServer SDK (.NET and Python) and how to forward custom caller headers using the x-client-* prefix. Added an allowlist for forwarded headers and clarified that credential/proxy headers (e.g., Authorization, Cookie, x-forwarded-*) are never forwarded. This improves security posture and observability when integrating with hosted containers.
  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/hosted-agent-contract

- **Migrate from agent applications to the new agent endpoint and publishing experience**
  Updated terminology to rename the agent property from protocols to protocol_configuration in property lists and legacy descriptions. This aligns migration guidance with the current configuration model and reduces confusion during upgrades.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/migrate-agent-applications

- **Publish agents to Microsoft 365 Copilot and Microsoft Teams in the Foundry portal**
  Replaced the previous notice with a Warning that explains data processing and storage implications when publishing to Microsoft 365 and Teams, including which data types may be processed. Encourages teams to assess compliance, residency, and governance before publishing to reduce regulatory risk.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/publish-copilot

- **Publish agents to Microsoft 365 Copilot and Microsoft Teams by using the REST API + VNet Guidance**
  Updated examples to use agent_endpoint.protocol_configuration and removed isolation_key_source from the Entra authorization scheme; also removed the preview note for the Microsoft 365 publish API. Added a Warning detailing Microsoft 365/Teams data processing considerations to support compliance evaluations.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/publish-copilot-virtual-network

- **Register external agents for observability and evaluation (preview)**
  Added an IMPORTANT advisory outlining responsibilities when integrating external agents, including reviewing compliance/data handling, managing cross-boundary data flow, and applying responsible AI mitigations. This guidance helps teams reduce risk and align with platform transparency practices.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/register-external-agent

- **Start an asynchronous batch translation**
  Updated the REST API example to rename the translateWithinImage parameter to translateTextWithinImage for image text translation in documents. This ensures requests use the correct property and avoids translation failures.
  https://learn.microsoft.com/en-us/azure/ai-services/translator/document-translation/latest/rest-api/translate-asynchronous