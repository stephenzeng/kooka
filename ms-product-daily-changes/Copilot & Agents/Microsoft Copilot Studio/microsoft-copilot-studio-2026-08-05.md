# Microsoft Copilot Studio
**Date created:** 2026-08-05 UTC  
**Tags:** Administration, Agent, Security  

## New Articles

- **Work IQ in Microsoft Copilot Studio (preview)**

  Introduced a new overview of Work IQ, including its architecture (Data, Memory, Inference) and usage-based billing with Copilot Credits. Highlights enterprise features such as governance, security, continuous evaluation, and an integrated developer experience. Provides admin considerations (default read-only, spending policies, regional availability) and step-by-step setup to connect an agent, authenticate, grant permissions, and validate with an email-context prompt. Includes links for tenant enablement and related guidance.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/add-work-iq

## Moderate Changes

- **Add SharePoint as a knowledge source**

  Clarified how sensitivity labels and encryption affect grounding: only permitted content is surfaced and encrypted items can’t be extracted, which may lead to no response even when users have access. Specified that the agent only searches the registered site or folder and subfolders, and that links within content aren’t crawled. Added a limitations section and noted consistent support for communication and team sites to help plan reliable indexing.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/knowledge-add-sharepoint

- **Calendar reference (preview)**

  Rebranded the page and tooling from “Work IQ Calendar” to “Calendar” and updated headings and reference entries to match the new naming. Terminology now reflects calendar tools and operations without changing scope or capabilities.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/mcp-calendar-tools

- **Copilot reference (preview)**

  Updated naming from “Work IQ Copilot” to “Copilot” across file, headings, and reference table. Simplified terminology to align with the broader Copilot brand without altering features.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/mcp-copilot-tools

- **Mail reference (preview)**

  Rebranded from “Work IQ Mail” to “Mail” and updated the H1 and reference table accordingly. Expanded the tool description to outline Microsoft Graph mail capabilities such as creating, sending, replying, and managing messages.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/mcp-mail-tools

- **OneDrive reference (preview)**

  Removed “Work IQ” branding and aligned names and descriptions with “OneDrive” tools. Refreshed wording and contributors while keeping tool capabilities and parameters unchanged.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/mcp-onedrive-tools

- **SharePoint reference (preview)**

  Renamed the file and content from “Work IQ SharePoint” to “SharePoint” and shifted terminology from “server” to “tools.” Clarified wording in descriptions and updated contributors, with no functional changes to the tools.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/mcp-sharepoint-tools

- **Teams reference (preview)**

  Rebranded from “Work IQ Teams” to “Teams,” added an Overview section, and updated the reference entry. The description now positions these as tools for managing chats, channels, users, and messages.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/mcp-teams-tools

- **User reference (preview)**

  Updated naming from “Work IQ User” to “User” and adjusted titles and descriptions to reflect user-focused tools for organizational context. Added a new contributor while keeping functionality the same.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/mcp-user-tools

- **Quotas and limits**

  Added guidance to plan for throughput and rate limits, including RPM/RPH considerations for high-volume or autonomous agents. Describes how to estimate peaks, understand throttling, design to reduce pressure, and request limit increases, with a link to detailed planning.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/requirements-quotas