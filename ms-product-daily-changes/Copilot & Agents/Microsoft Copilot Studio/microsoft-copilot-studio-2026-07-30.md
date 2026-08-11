# Microsoft Copilot Studio
**Date created:** 2026-07-30 UTC  
**Tags:** Administration, AI, Agent, Automation  

## New Articles

- **Attach files to a conversation (preview)**
  
  Introduced documentation for end users to attach files to agent conversations, clarifying how this differs from maker-configured knowledge sources. Covers supported inputs (images, PDFs, documents, URLs), availability across Copilot Studio preview and channels like Teams and Microsoft 365 Copilot, and how attachments are processed per turn. Specifies URL handling requirements (public access and a 30-second download timeout) and retention/limits (16 MiB per file, 28 days per conversation). Notes that failed items are skipped so conversations continue, with links to related testing and knowledge articles.
  
  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/attachments-overview

- **Files the agent creates (preview)**
  
  Added guidance on when agents generate files (documents, charts, images, code, edited attachments) and how users access them via created-file cards with previews and downloads across supported channels. Explains that users can reference created files in follow-up turns and documents retention and limits (10 MB per created file, stored with conversation, 28-day retention), including behavior when files exceed limits. Provides practical recommendations to split large outputs and links to related attachments, tools, and testing topics.
  
  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/created-files-overview

- **Add a Model Context Protocol (MCP) server to your agent as a tool (preview)**
  
  New how-to describes connecting an MCP server as a tool, including prerequisites and step-by-step setup from the Build tab (naming, description, URL, authentication). Explains server handshake and tool discovery, how to review tool metadata, and how the tool appears in the Tools list for testing and iteration. Covers post-add management (enable/disable, edit to refresh credentials and tools) and documents limits on concurrent MCP servers and tool counts to aid planning and governance.
  
  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/tools-add-mcp-server

- **Add a workflow to your agent as a tool (preview)**
  
  Introduces a guided process to add workflows as tools, including required nodes (“When an agent calls the flow” and “Respond to the agent”), save/publish steps, and surfacing in the agent’s Tools list and Workflows page. Provides testing guidance via the Preview tab with activity traces for debugging and operational tips for managing, disabling, or removing the workflow. This streamlines connecting automation to agent experiences using standard tool management.
  
  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/tools-add-workflow

## Moderate Changes

- **Add a tool to an agent (preview)**
  
  Reworked instructions to highlight supported custom tool types and direct readers to dedicated MCP server and workflow articles for step-by-step guidance. Simplified the page by removing duplicated in-line procedures and refining tips for clearer naming. This improves navigation and keeps canonical how-to details in focused topics.
  
  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/add-tools-custom-agent

- **Test an agent (preview)**
  
  Added guidance for editing an agent while testing: the current turn runs with the prior configuration, and subsequent turns pick up edits automatically. Clarifies that structural changes (like tools, model, or Memory) apply on the next turn and recommends starting a new conversation if updates don’t apply after a couple of turns. This enables rapid iteration without leaving the test experience.
  
  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/authoring-test-bot

- **Available knowledge sources for agents (preview)**
  
  Clarified the difference between maker-provided knowledge sources (shared design-time grounding) and end-user attachments for one-off conversations. Added a link to the attachments page for deeper guidance.
  
  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/knowledge-sources-overview

- **Manage and delete tools in an agent (preview)**
  
  Updated to emphasize managing connector and workflow configurations rather than generic tools. Added steps for viewing and updating MCP server settings, inspecting exposed tool descriptions, toggling individual tools, and refreshing authentication credentials. This strengthens operational control and governance for tool configurations.
  
  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/tools-manage

- **Tools overview for agents (preview)**
  
  Introduced a Limits section detailing constraints: a 10 MB cap per file created by the agent during a turn and counting MCP servers toward the agent’s total tool limit, with a cap on concurrent MCP server instances. Includes references to related guidance to help plan implementations and avoid runtime issues.
  
  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/tools-overview