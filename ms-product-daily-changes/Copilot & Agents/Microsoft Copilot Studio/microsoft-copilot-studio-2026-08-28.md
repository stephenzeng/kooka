# Microsoft Copilot Studio
**Date created:** 2026-08-28 UTC  
**Tags:** Automation, Best Practices, Billing, Configuration, Get Started, Governance, Guidance, Identity, Licensing, Security, Troubleshooting  

## New Articles

- **Migrate Copilot Studio agents to Microsoft Entra Agent ID (preview)**
  
  New how-to guidance explains optional manual migration from legacy Azure app registrations to Microsoft Entra Agent IDs, including benefits like agent-scoped conditional access and notes on future automated migration. It provides prerequisites, planning tips for staged rollouts, and step-by-step migration using the Power Platform admin center with validation via Entra sign-in logs. It also documents API endpoints and PowerShell examples to automate migration and rollback, plus troubleshooting and related resources.
  
  https://learn.microsoft.com/en-us/microsoft-copilot-studio/govern-migrate-api-entra-agent-identity

## Major Changes

- **Extend Microsoft 365 Copilot with the Copilot chat harness**
  
  The setup flow now creates the agent first and moves configuration into a streamlined basic settings experience. Knowledge sources expand beyond SharePoint and connectors to include Teams chats/meetings, Outlook emails, websites, and admin-configured Copilot (Graph) connectors, with a new search-and-filter experience and quick-add options. New toggles control scope (for example, Search all websites and Only use specified sources) and referencing org data, while the former Tools section is replaced with Capabilities for generating code, graphs, documents, and images. Publishing guidance is refreshed and simplified to reflect the new experience.
  
  https://learn.microsoft.com/en-us/microsoft-copilot-studio/microsoft-365-copilot-extend-with-agents

## Moderate Changes

- **Manage Entra Agent IDs**
  
  Updated governance and timeline guidance clarifies that, starting May 2026, new agents use Entra Agent IDs and existing agents will be migrated by Microsoft. Admins can optionally migrate earlier via the Power Platform admin center, PowerShell, or APIs, and governance applies to both identity models during transition. The opt-out option for automatic identity creation is removed from May 2026.
  
  https://learn.microsoft.com/en-us/microsoft-copilot-studio/admin-use-entra-agent-identities

- **Add other agents overview**
  
  The page now uses a centralized include to present the connected agents concept, replacing the older banner and intro. Core guidance remains intact with minor cleanup.
  
  https://learn.microsoft.com/en-us/microsoft-copilot-studio/authoring-add-other-agents

- **Configure agent details and instructions**
  
  Guidance now covers both GitHub Copilot and Copilot chat harnesses with clear when-to-use explanations for Build versus Configure. It adds harness-specific configuration details such as name limits and icon requirements, and clarifies how to enter and save instructions with updated best practices and links.
  
  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/authoring-instructions

- **Create a new agent**
  
  The creation guidance points to Agent Details in Settings for changing language, solution, and schema, simplifying the initial flow. It adds post-save next steps for adding knowledge, tools, skills, and connected agents; configuring the model and memory; and testing, evaluating, sharing, publishing, and monitoring.
  
  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/build-new-agent

- **Configure suggested prompts for Teams and Microsoft 365**
  
  The introduction is refocused on configuring up to 10 suggested prompts for Teams and Microsoft 365 Copilot Chat, noting that prompts can’t be tested in Copilot Studio. Legacy details about automatic generation and welcome-page display were removed, while best practices remain.
  
  https://learn.microsoft.com/en-us/microsoft-copilot-studio/configure-starter-prompts

- **App registration, agent identities, and authentication**
  
  The article is renamed and reorganized to emphasize governance for agent identities and authentication. It clarifies that agents created before May 2026 use legacy app registrations that will migrate without downtime, expands scope behavior and enforcement (including Conditional Access for Teams), and refines limits for Entra Agent ID creation.
  
  https://learn.microsoft.com/en-us/microsoft-copilot-studio/govern-agents-identities-overview

- **Harnesses in Copilot Studio**
  
  Content is split into dedicated sections for GitHub Copilot, standard, and Copilot chat harnesses, plus a comparison to guide selection. Billing guidance links are made explicit per harness, and capability descriptions are refined to clarify when to choose each option.
  
  https://learn.microsoft.com/en-us/microsoft-copilot-studio/harnesses-overview

- **Knowledge sources summary**
  
  The page now uses a centralized explanation of how knowledge sources power generative answers and notes they can be attached directly to a topic node. Deprecated content (such as the Excel semantic search code interpreter include) was removed and wording streamlined.
  
  https://learn.microsoft.com/en-us/microsoft-copilot-studio/knowledge-copilot-studio

- **Agents powered by the GitHub Copilot Harness overview**
  
  The introduction is clarified and a new section explains how the Build tab emphasizes natural-language-first authoring, reduced branching, and orchestration to use instructions, knowledge, and tools compared to the standard harness.
  
  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/overview