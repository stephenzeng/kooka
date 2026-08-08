# Microsoft 365 Copilot Extensibility
**Change date:** 2026-08-07 UTC  
**Tags:** AI, Agent, Programming  

## Major Changes

- **Share and manage agents**

  Expanded guidance for sharing and managing agents, introducing multi-owner support with clear roles for editors and chat-only users. Updated the share experience to list current access, manage roles, provide dedicated chat/edit links, and enable organization-wide chat access via a new toggle. Clarified governance and admin controls, SharePoint knowledge source requirements, and how sensitivity labels affect access. Documented ownership reassignment options and refined troubleshooting to align with the new sharing model, helping teams manage access more securely and efficiently.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/agent-builder-share-manage-agents

- **Work IQ MCP tool reference**

  Added the fetch_blob tool to retrieve binary files (for example, documents, images, Office files) from a Work IQ path and return them as Base64 with metadata. Documented required and optional parameters, response schema, and operational limits, including the default 4 MB raw-file limit and the need to decode Base64 from structuredContent. Provided example requests and responses to help developers implement reliable file retrieval and handle errors gracefully.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/work-iq/mcp/tool-reference

## Moderate Changes

- **Write effective instructions for declarative agents**

  Generalized the guidance by removing specific GPT 5.x references and reframing notes to account for model updates broadly. Updated stabilization recommendations to focus on literal-execution headers and renamed the prior migration-focused pattern to a general stability evaluation pattern for auditing inconsistent behavior.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/declarative-agent-instructions