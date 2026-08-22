# Microsoft Scout (Frontier)
**Date created:** 2026-08-22 UTC  
**Tags:** Automation, Configuration, Get Started, Guidance, Identity, Security, Troubleshooting  

## New Articles

- **Troubleshoot Microsoft Scout in managed environments**

  Introduced a deep-dive guide for running Scout in managed or hardened environments, with a quick symptom-to-cause reference and actionable admin checks. Clarifies network requirements, including allow-listing GitHub Copilot endpoints and excluding them from TLS/SSL inspection, and provides fixes for the “Unable to verify access” screen with policy and fallback options. Covers protocol handler registration, Microsoft Defender/AppLocker/WDAC rules, VDI/RDP and Citrix HDX considerations, and handling non‑persistent images and controlled folders. Includes guidance for workspace/cache locations and step-by-step log collection across Windows and macOS, with links to related admin setup and FAQ content.

  https://learn.microsoft.com/en-us/microsoft-scout/managed-troubleshoot

- **What's new in Microsoft Scout**

  Added a consolidated “What’s new” page capturing July and August 2026 updates. Highlights August additions such as GitHub Enterprise Cloud sign-in, Teams meeting transcripts and room booking, SharePoint Lists, Outlook inbox rules, OneDrive/SharePoint sharing and access management, and cloud-backed Co‑Create workspaces. Summarizes July enhancements including new Co‑Create editors and formats, per‑message model and reasoning controls, conversation compaction, richer chat organization, broader file access, and OneDrive-based session history. Also notes UI, reliability, and accessibility improvements plus a redesigned, searchable Settings experience.

  https://learn.microsoft.com/en-us/microsoft-scout/whats-new

- **Work with Microsoft 365 in Microsoft Scout**

  Added a dedicated how‑to for using Scout with Microsoft 365, covering Outlook mail and calendar, Teams chats and channels, Microsoft To Do, directory/content search, Teams meeting transcripts, meeting room booking, SharePoint Lists, and file sharing/access management. Emphasizes approval prompts, scope and permission requirements, and key limitations such as no anonymous links or removing existing access. Provides troubleshooting tips and pointers to related Scout documentation for setup and governance.

  https://learn.microsoft.com/en-us/microsoft-scout/work-with-microsoft-365

## Major Changes

- **Microsoft Scout common questions**

  Expanded the FAQ with new capabilities, clearer admin guidance, and broader scenarios. Added details for Teams channels and To Do tasks, GitHub Enterprise Cloud sign‑in, Copilot seat and policy requirements, meeting transcripts and room booking, SharePoint Lists, Outlook inbox rules, and OneDrive/SharePoint file sharing and access management with noted limitations. Streamlined admin controls to focus on Group Policy and Microsoft Intune, introduced a feedback section, and refreshed related links while removing outdated content.

  https://learn.microsoft.com/en-us/microsoft-scout/faq

- **Use Microsoft Scout**

  Reorganized and expanded guidance to reflect major product updates. Added open‑ended answer input, conversation compaction, per‑message model selection, default reasoning effort, context window controls, and improved chat organization. Broadened file access beyond workspaces with explicit permission prompts and significantly enhanced Co‑Create with local or OneDrive/SharePoint storage, in‑app editors, and support for common data and diagram formats. Condensed Microsoft 365 coverage to a high‑level summary and moved detailed workflows to a new dedicated page; automations now support configurable reasoning effort and context size, with improved session history and related links.

  https://learn.microsoft.com/en-us/microsoft-scout/use-microsoft-scout

## Moderate Changes

- **Admin access overview for Microsoft Scout**

  Expanded troubleshooting for GitHub Copilot access, clarifying that users need both an eligible Copilot license and an enabled GitHub Copilot app policy. Added a “symptoms and fixes” table plus step‑by‑step admin guidance for configuring policies at enterprise and organization levels, with version notes for pre‑1.1 and a reminder to restart the app after policy changes.

  https://learn.microsoft.com/en-us/microsoft-scout/admin-access-overview

- **Get started with Microsoft Scout**

  Updated sign‑in instructions to support GitHub Enterprise Cloud with enterprise host selection and browser-based completion, and clarified the need for a Business or Enterprise Copilot license. Emphasized Microsoft 365 identity for authentication and enhanced Settings documentation with grouped window/search, default reasoning effort, and Integrations options.

  https://learn.microsoft.com/en-us/microsoft-scout/get-started

- **Microsoft Scout (Frontier) overview**

  Expanded Microsoft 365 capabilities, specifying Outlook, Teams, SharePoint Lists, and files across OneDrive/SharePoint/Teams, with links to a new Microsoft 365 guide. Refined Co‑Create guidance to clarify simultaneous editing and storage in OneDrive or SharePoint, and added new links in Next steps and Related content. Performed minor cleanups, including removing Playwright references and unnecessary introductory text.

  https://learn.microsoft.com/en-us/microsoft-scout/overview