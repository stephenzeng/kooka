# Microsoft 365 Copilot Extensibility
**Date created:** 2026-08-22 UTC  
**Tags:** Configuration, Guidance  

## Moderate Changes

- **Overview of the Work IQ REST API**

  Removed an outdated limitation stating that Graph Explorer doesn’t support streamed conversations with the REST API. Updated guidance reflects current capability, enabling developers to validate streaming scenarios directly in Graph Explorer and align their integrations accordingly.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/work-iq/rest/overview

- **Plugins for Microsoft 365 Copilot**

  Clarified that dynamic tool discovery applies by default to plugins, not to agent connectors. Documented that agent connectors require Microsoft 365 app manifest version 1.29 or later and a supported host to use dynamic tool discovery, with a pointer to MCP server registration as agent connectors.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/overview-plugins

- **Dynamic tool discovery for MCP plugins in Microsoft 365 Copilot**

  Clarified the article’s scope as covering dynamic tool discovery for plugins (MCP servers via plugin manifest) and distinguished it from agent connector scenarios. Added requirements for enabling dynamic tool discovery with agent connectors (app manifest v1.29+ and host support) and linked to the agent connector registration guidance.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/plugin-dynamic-tool-discovery