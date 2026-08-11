# Microsoft 365 Copilot Extensibility
**Date created:** 2026-08-06 UTC  
**Tags:** Governance  

## Moderate Changes

- **Work IQ MCP tool reference**

  Clarified the authentication and permission model: Work IQ MCP uses Microsoft Entra authentication and the signed-in user's Microsoft 365 permissions for Microsoft Graph access. Documented a tenant policy layer that evaluates each tool request and blocks mutation operations by default, allowing admins to enable supported create, update, delete, and action requests as needed. Added a link to policy governance for configuration details.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/work-iq/mcp/tool-reference