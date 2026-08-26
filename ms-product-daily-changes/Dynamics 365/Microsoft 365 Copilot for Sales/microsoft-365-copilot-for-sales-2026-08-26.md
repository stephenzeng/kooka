# Microsoft 365 Copilot for Sales
**Date created:** 2026-08-26 UTC  
**Tags:** Best Practices, Configuration, Guidance  

## New Articles

- **Update Sales agent custom tools and knowledge in the Microsoft 365 admin center**

  Introduced a new how-to explaining how admins can update Sales agent custom tools and knowledge to the latest source-agent version using Update from store. Details when the option appears, step-by-step update flow, and what changes during an update, including preserving assigned users and security groups while replacing copied content without removing the extension. Clarifies scenarios where updates are unavailable, behavior on failures, expected propagation delays, and limitations such as always pulling the latest version, admin initiation, size limits, audience preservation, and required external permissions. Includes related links to extending Sales agent and managing connected agents.

  https://learn.microsoft.com/en-us/microsoft-sales-copilot/update-sales-chat-custom-tools

## Moderate Changes

- **Extend Sales agent with custom tools and knowledge in the Microsoft 365 admin center**

  Repositioned the extensibility guidance to center on using custom declarative agents as the source for tools and knowledge, and clarified tool capabilities (data retrieval, CRUD, and business actions) and grounding sources. Added guidance on building agents, configuring citations and source links via response_semantics, and updating copied tools/knowledge with clear versioning behavior and preserved assignments. Streamlined terminology to consistently reference Sales agent, added a related link to managing connected agents, and removed duplicate content.

  https://learn.microsoft.com/en-us/microsoft-sales-copilot/extend-sales-chat-custom-tools

- **Manage connected agents in the Microsoft 365 admin center**

  Clarified that citations from tools used by connected agents are not preserved in responses to the parent agent. Recommended preserving citations by copying the connected agent’s tools and knowledge into the parent agent using Copy custom tools & knowledge, with a link to the configuration guidance.

  https://learn.microsoft.com/en-us/microsoft-sales-copilot/manage-connected-agents

- **Set up Sales agent in Microsoft 365 Copilot**

  Added an optional step introducing how to extend Sales agent with custom tools and knowledge to integrate data, improve insights, and ensure accurate responses. Included a link to the detailed extension guide.

  https://learn.microsoft.com/en-us/microsoft-sales-copilot/set-up-sales-chat