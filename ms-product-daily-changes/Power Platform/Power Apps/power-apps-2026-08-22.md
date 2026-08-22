# Power Apps
**Date created:** 2026-08-22 UTC  
**Tags:** Automation, Configuration, Get Started, Guidance, Security  

## New Articles

- **Microsoft Dataverse plugin for AI coding agents (preview)**

  Introduced an overview of the Dataverse plugin that enables AI coding agents to securely work with Dataverse through MCP, CLIs, SDKs, and the Web API. Provided end-to-end setup for popular agents (GitHub Copilot, Claude Code, Cursor, Codex) and connection using dv-connect, including environment discovery, authentication, and MCP registration. Included example prompts for querying data, performing imports and bulk operations, managing metadata and solutions, and handling environment settings and role assignments. Documented safety guardrails, required privileges, confirmation flows, and guidance for high-impact operations, with notes on credentials, data handling, logging, and telemetry.

  https://learn.microsoft.com/en-us/power-apps/developer/data-platform/agents-plugin/

- **Enable the modern, refreshed look for model-driven apps on mobile (preview)**

  Introduced a preview feature to enable the modern mobile experience for model-driven apps, distinct from the web New look. Detailed configuration for the Mobile modern experience (value 2) and optional dynamic font scaling, with steps to enable at the environment and app levels. Provided guidance for testing on devices (including offline scenarios), recommended use of the Power Apps grid, and listed known limitations such as no dark mode, limited theme support, and preview constraints.

  https://learn.microsoft.com/en-us/power-apps/mobile/mobile-new-look

- **Microsoft Dataverse plugin for AI coding agents reference (preview)**

  Published a comprehensive reference for the Dataverse plugin’s skills, including dv-overview, dv-connect, dv-query, dv-data, dv-metadata, dv-solution, dv-admin, and dv-security. Outlined capabilities across reading, writing, bulk operations, metadata management, solution lifecycle, admin safeguards, and security/role assignments, with example prompts and tool selection guidance (MCP, CLI, SDK, Web API). Covered confirmation workflows for environment and solution operations and linked related resources.

  https://learn.microsoft.com/en-us/power-apps/developer/data-platform/agents-plugin/reference

## Moderate Changes

- **Code components for canvas apps  | Microsoft Docs**

  Updated security guidance to emphasize that code components from untrusted sources can access tokens and data when rendered, and to advise installing only from trusted sources. Removed the previous note suggesting the risk didn’t apply when playing the app, clarifying consistent caution for all run modes.

  https://learn.microsoft.com/en-us/power-apps/developer/component-framework/component-framework-for-canvas-apps