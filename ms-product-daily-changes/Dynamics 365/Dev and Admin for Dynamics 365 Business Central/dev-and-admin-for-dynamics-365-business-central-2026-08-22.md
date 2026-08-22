# Dev and Admin for Dynamics 365 Business Central
**Date created:** 2026-08-22 UTC  
**Tags:** Automation, Configuration, Guidance, Security, Troubleshooting  

## Major Changes

- **ALTool**

  Added a new ALTool command, launchsnapshotmcpproxy, to enable AI agents to capture and debug AL snapshots from Business Central sessions. Updated guidance explains the MCP proxy workflow, usage syntax, and options for environment targeting, authentication (including BC_ACCESS_TOKEN and cached logins), on-prem connectivity, and logging. Clarified token acquisition with Azure CLI and provided steps for both cloud and on-premises scenarios. Included a tip for VS Code agent mode to streamline registration and usage.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/devenv-al-tool

- **Snapshot debugging**

  Introduced MCP-based snapshot debugging with an AI agent as an alternative to keyboard-driven flows, covering initialization, status, and stop/collect operations with optional session targeting. Provided practical guidance for prompting the agent, setting snappoints, and scoping by client type and user. Documented setup and authentication using ALTool launchsnapshotmcpproxy across multiple MCP hosts (Claude CLI, GitHub Copilot CLI, VS Code), including interactive sign-in, access tokens, stdio configuration, and environment variables. Explained required permissions, auditing behavior, time limits, and privacy considerations, and noted compatibility with existing VS Code snapshot debugging.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/devenv-snapshot-debugging