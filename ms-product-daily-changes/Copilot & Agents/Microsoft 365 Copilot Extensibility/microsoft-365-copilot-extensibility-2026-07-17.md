# Microsoft 365 Copilot Extensibility
**Date created:** 2026-07-17 UTC  
**Tags:** Administration, Agent, AI, Analytics, Governance, Programming, Security  

## New Articles

- **Configure API key authentication**

  Introduced a dedicated guide for setting up API key authentication for API plugins, covering bearer, custom header, and query parameter schemes. Explains how to create and store an authentication configuration in the Microsoft Enterprise token store and reference it from the plugin manifest. Provides step-by-step options using Microsoft 365 Agents Toolkit or the Teams developer portal, with guidance on secrets management and manifest updates. Clarifies that API keys are not supported for MCP plugins and points to alternative OAuth/Entra options.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/plugin-authentication-api-key

- **Configure dynamic client registration**

  Added a how-to for enabling Dynamic Client Registration (DCR) for MCP plugins, detailing required OAuth metadata endpoints and constraints such as client secret and PKCE. Provides setup paths via Agents Toolkit or the declarative agent developer skill that auto-create the Enterprise token store configuration and update the manifest. Explains how runtime authentication is wired using OAuthPluginVault with a reference_id, with links to supporting references.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/plugin-authentication-dynamic-client-registration

- **Configure Microsoft Entra SSO authentication**

  Published a step-by-step guide to configure Microsoft Entra SSO for MCP and API plugins. Covers app registration, creating the Enterprise token store auth configuration, required redirect URIs, and updating identifierUris and client permissions. Details how to reference the auth configuration in the plugin manifest and how to adjust the MCP server or API to accept the new audience and client.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/plugin-authentication-entra-sso

- **Configure anonymous authentication**

  Added guidance for using anonymous authentication during development by setting the plugin manifest runtime authentication type to None. Clarifies applicability to both MCP and OpenAPI-based API plugins and cautions that it is intended only for testing. Includes references to other authentication options and troubleshooting.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/plugin-authentication-none

- **Configure OAuth 2.0 authentication**

  Introduced a comprehensive OAuth 2.0 guide (authorization code flow with optional PKCE) for MCP and API plugins. Explains creating and storing auth configurations in the Enterprise token store, configuring OpenAPI securitySchemes for API plugins, and updating manifests with OAuthPluginVault. Provides setup options using Agents Toolkit, the declarative agent developer skill (including DCR support), or the Teams developer portal, plus notes on sign-out behavior and required redirect URIs.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/plugin-authentication-oauth

- **Troubleshoot MCP and API plugin authentication**

  Added a consolidated troubleshooting resource for plugin authentication failures. Covers common misconfigurations (Base URL, redirect URI, reference_id), unsupported redirects, consent and audience settings for Entra SSO, and organization policy restrictions. Includes guidance for popup issues, debugging window.opener conditions, resolving credential mismatches, forcing reauthentication, and links to related setup guides.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/plugin-authentication-troubleshooting

## Major Changes

- **Build a plugin for a declarative agent from an MCP server**

  Overhauled the guide to focus on building an MCP “plugin” rather than an “action,” with a complete GitHub MCP server walkthrough. Raised the Agents Toolkit requirement to 6.12.0+ and shifted guidance to dynamic tool discovery with pinned tool options. Expanded authentication coverage (OAuth, Dynamic Client Registration, Entra SSO) and streamlined the setup flow, UI considerations, and usage steps for clarity and speed.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/build-mcp-plugins

- **copilotReportRoot: getMicrosoft365CopilotUsageUserDetail**

  Added an optional version parameter and updated request syntax for both v1.0 and beta, making period required and version-dependent. Introduced a Report versions section that defines v1 fields and v2 enhancements such as app-specific prompt counts, active usage days, and expanded last activity dates. Clarified response formats (v1 CSV stream, preview JSON) and refreshed examples to match versioned endpoints.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/api/admin-settings/reports/copilotreportroot-getmicrosoft365copilotusageuserdetail

- **copilotReportRoot: getMicrosoft365CopilotUserCountSummary**

  Enabled a version query parameter with version-specific period values and documented defaults. Added a Report versions section detailing v1 fields and v2 additions like Edge, Microsoft 365 Copilot, and Copilot Chat user metrics, plus total and average prompts. Updated examples and response behaviors, with v1 returning CSV and beta providing JSON.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/api/admin-settings/reports/copilotreportroot-getmicrosoft365copilotusercountsummary

- **copilotReportRoot: getMicrosoft365CopilotUserCountTrend**

  Introduced versioned requests and adjusted the required period parameter per version. Documented v1 versus v2 report fields, including expanded user and prompt metrics in v2. Aligned examples to versioned endpoints and clarified response formats for v1 (CSV) and preview (JSON).

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/api/admin-settings/reports/copilotreportroot-getmicrosoft365copilotusercounttrend

- **Plugins for Microsoft 365 Copilot**

  Expanded guidance on dynamic tool discovery for MCP plugins and clarified when to pin tools versus using runtime discovery. Enhanced response customization with MCP apps, Adaptive Cards usage, and automatic citation inference. Updated diagrams, URL rendering behavior, limitations (including semantics-based selection and token window), and related references for a more predictable plugin experience.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/overview-plugins

- **Configure authentication for MCP and API plugins in agents in Microsoft 365 Copilot**

  Rewrote the authentication overview to centralize guidance and direct readers to focused articles per scheme. Added a support matrix (including DCR for MCP) and explained how authentication configurations are created and stored in the Enterprise token store, then referenced from plugin manifests. Clarified runtime token acquisition and provided a single troubleshooting entry point, removing redundant procedural content.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/plugin-authentication

- **Dynamic tool discovery for MCP plugins in Microsoft 365 Copilot**

  Reframed content around “pinned tools” versus dynamic discovery and extended coverage to MCP apps with UI widgets. Added manifest comparisons with JSON examples, guidance on fetching and selecting tools via Agents Toolkit, and how tool definitions are stored and referenced. Clarified admin governance views in Microsoft 365 admin center and updated comparisons and validation details to reflect the new terminology.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/plugin-dynamic-tool-discovery

## Moderate Changes

- **Agents for Microsoft 365 Copilot**

  Updated the Channels description for custom engine agents to remove references to external app and website hosting. Clarifies that agents run in Microsoft 365 Copilot and Microsoft 365 apps including Teams, Word, Excel, and Edge.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/agents-overview

- **Confirmation prompts for MCP and API plugins for Microsoft 365 Copilot**

  Clarified that custom confirmation text applies only to pinned tools defined in the manifest. For dynamically discovered MCP tools, Copilot uses the tool description from the MCP server’s tools/list response.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/plugin-confirmation-prompts

- **Add MCP apps to declarative agents in Microsoft 365 Copilot**

  Streamlined the creation steps by pointing to a separate agent walkthrough and focusing on MCP app specifics. Added guidance for dynamic tool discovery and development-time authentication and increased the Agents Toolkit minimum version to 6.12.0.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/plugin-mcp-apps

- **Troubleshoot MCP apps in Microsoft 365 Copilot**

  Expanded diagnostics for missing tools, covering both dynamic discovery and pinned tools with validation steps and MCP Inspector usage. Updated manifest examples, added authentication checks, and consolidated auth troubleshooting to a dedicated article.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/plugin-mcp-apps-troubleshooting

- **What's new in Microsoft 365 Copilot extensibility**

  Added the July 2026 entry announcing the new version parameter for three Copilot usage reports. This enables richer, versioned reporting with additional metrics.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/whats-new