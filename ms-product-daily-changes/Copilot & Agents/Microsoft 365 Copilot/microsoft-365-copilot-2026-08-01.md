# Microsoft 365 Copilot
**Date created:** 2026-08-01 UTC  
**Tags:** Administration, AI, Agent, Programming  

## Major Changes

- **Microsoft 365 Copilot release notes**
  Added a July 29, 2026 release wave with richer responses and broader platform coverage. Highlights include inline images in answers, a redesigned OneNote Copilot Notebooks experience, SharePoint Lists grounding via Context IQ, email attachment listing, and a built-in screenshot tool. Extensibility updates let admins edit ServiceNow connector mappings, add SharePoint lists (up to 20,000 items) as Agent Builder knowledge, and refresh adaptive cards for custom engines. SharePoint/OneDrive gains natural language solution building and a floating Copilot button for contextual prompts—improving discoverability and workflow speed across Windows, Web, Mac, iOS, and Android.
  https://learn.microsoft.com/en-us/microsoft-365/copilot/release-notes

- **Release notes, known issues, and limitations for the Employee Self-Service agent**
  Upgraded the Employee Self-Service agent to the GPT-5.5 model with guidance to take the latest package and notes on staged regional rollout. Deprecated GPT-5.3 support and refreshed known issues to reflect GPT-5.5 behaviors, including slightly longer responses and clearer, but still evolving, routing. Added a limitation that Copilot Hub connected-agent paths aren’t in the GPT-5.5 rollout yet; those connections should remain on GPT-4.1.
  https://learn.microsoft.com/en-us/microsoft-365/copilot/employee-self-service/known-issues-limitations

## Moderate Changes

- **Build plugins for Copilot Cowork**
  Expanded developer guidance to accept workspace files in plugin tools using JSON Schema parameters with contentEncoding: base64, including single and multi-file examples. Clarified that Cowork rewrites parameters and resolves files to content at invocation so file data stays out of model context, with limits (up to 8 files, 150 MiB total and per file) and confirmation prompts for file-handling tools. This enables secure, scalable file-driven scenarios like conversions, analysis, and attachments.
  https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/cowork-plugin-development

- **Copilot Cowork common questions**
  Added an FAQ explaining how plugins can operate on user-selected session files with explicit user approval. This clarifies file handling flows and points developers to guidance for accepting files from the Cowork workspace.
  https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/cowork-faq

- **Use plugins with Copilot Cowork**
  Introduced guidance showing that plugin connectors can process files from a user’s session with an approval step. Linked to authoring best practices so builders can enable file-aware tools confidently.
  https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/cowork-plugins

- **What's new in Copilot Cowork**
  Announced “Workspace file input for plugin tools,” enabling plugins to declare base64-encoded file parameters that Cowork resolves before tool invocation. This unlocks scenarios like document conversion, image analysis, and attaching artifacts to external systems, with a link to implementation details.
  https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/whats-new