# Microsoft 365 Copilot Extensibility
**Date created:** 2026-07-30 UTC  
**Tags:** AI, Agent  

## Major Changes

- **Show citations with response semantics in Copilot MCP connectors and agents**

  Introduced dynamic, zero-configuration citation inference so Copilot can derive citation metadata when explicit response_semantics are omitted, while honoring explicit mappings when present. Clarified field alias priorities and resolution rules (for example, URL required; title falls back to hostname; subtitle and thumbnail are opportunistic), improving predictable citation output. Added a full MCP example demonstrating inferred citations from stringified results and noted applicability with dynamic tool discovery scenarios. Updated the page title to reference MCP connectors and agents.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/plugin-citations

## Moderate Changes

- **Add knowledge sources to your declarative agent in Microsoft 365 Copilot**

  Added guidance to use OneNote pages as knowledge sources via the file picker—supporting individual pages only, not entire notebooks or direct URLs. Expanded Microsoft Teams data instructions to let authors scope knowledge to specific meetings via the Meetings tab. Clarified that selecting “My Teams chats and meetings” searches all transcripts and calendar unless specific meetings are added.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/agent-builder-add-knowledge

- **Best practices for building declarative agents in Microsoft 365 Copilot**

  Added a best practice to ground responses to configured knowledge by setting discourage_model_knowledge: true in the special_instructions object. Includes references to the Special instructions object and guidance to improve accuracy and traceability.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/declarative-agent-best-practices

- **Write effective instructions for declarative agents**

  Added guidance to ground agent responses by setting discourage_model_knowledge: true in special_instructions to avoid reliance on built-in model knowledge. Explains the rationale for accuracy and traceability and links to the Special instructions object documentation.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/declarative-agent-instructions

- **Add knowledge sources to your declarative agent**

  Added OneNote pages as a supported knowledge source and updated the capabilities table (queryable but not searchable; no special permissions). Clarified that only individual pages can be selected via the file picker and that URL entry and entire notebooks are not supported.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/knowledge-sources

- **Known Issues in Microsoft 365 Copilot Extensibility**

  Expanded limitations for custom engine agents to note that file and image attachments in chats aren’t supported and images uploaded in chat aren’t passed to the agent. Scenarios that require image upload (such as extracting text from an image) aren’t supported.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/known-issues