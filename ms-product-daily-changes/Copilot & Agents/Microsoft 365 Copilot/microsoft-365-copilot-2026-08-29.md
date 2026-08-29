# Microsoft 365 Copilot
**Date created:** 2026-08-29 UTC  
**Tags:** Best Practices, Configuration, Governance, Guidance, Licensing  

## Major Changes

- **Build plugins for Copilot Cowork**

  Added comprehensive guidance for accepting workspace files in plugin tools using JSON Schema parameters with contentEncoding: base64. Clarifies how Cowork maps top-level file parameters to direct_attachment_file_paths, handles nested parameters, and what the connector receives without schema changes. Documents limits (file count, size, nesting) and provides practical recommendations on descriptions, formats, annotations, $ref usage, and parameter counts, plus a new FAQ entry confirming file input support. This enables developers to reliably accept files from the Cowork workspace and design resilient, predictable tools.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/cowork-plugin-development

- **Get started with Word, Excel, and PowerPoint Agents in Microsoft Copilot**

  Updated guidance to confirm these Agents are premium capabilities available only with a paid Microsoft 365 Copilot license. Clarifies visibility in the Copilot app depends on Anthropic being enabled and that admins can manage or block the Anthropic provider in the admin center. Strengthens enterprise data and Work IQ descriptions for licensed users and explicitly excludes unlicensed Copilot Chat users in the limitations. These changes help admins deploy and govern Agents correctly while setting clear expectations for access and language availability.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/wordexcelppt-agents

## Moderate Changes

- **Use the local browser with Copilot Cowork**

  Added admin policy guidance to enable browser automation in Microsoft Edge starting with Edge 152 via the copilotcoworktoolactionsenabled policy. Clarified requirements, behavior for sensitive actions, and handoff points to the user, and refined task flow wording. These updates improve setup clarity and governance control for local browser automation.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/cowork-local-browser

- **Microsoft Copilot overview**

  Introduced Microsoft Copilot Cowork with availability via usage-based billing and clarified that Microsoft Agents use web and work data (Microsoft Graph and Work IQ). Removed redundant content to streamline the overview. This provides a clearer picture of capabilities and how they’re accessed.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/microsoft-365-copilot-overview

- **Use Copilot Cowork**

  Increased the maximum number of scheduled prompts a user can create from 5 to 25. This expands automation capacity for recurring tasks and workflows.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/use-cowork

- **What's new in Copilot Cowork**

  Refreshed the page for August 2026 and added an Enhancements section. Highlights include workspace file inputs for plugin tools using base64-encoded parameters and the local browser moving to general availability for all tenants. These updates surface newly available capabilities and direct readers to implementation guidance.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/whats-new