# Microsoft 365 Copilot
**Date created:** 2026-08-19 UTC  
**Tags:** Automation, Best Practices, Compliance, Configuration, Get Started, Governance, Guidance, Licensing, Security  

## New Articles

- **Add Microsoft Copilot endpoints to your allow list**

  Introduced a new guide to allow-list the Microsoft Copilot client (version 152+) with required domains for update checks, configuration, and downloads, recommending a wildcard such as *.dl.delivery.mp.microsoft.com. Documented optional Delivery Optimization endpoints (*.do.dsp.mp.microsoft.com) and port 7680 for peer-to-peer updates. Listed sign-in and service endpoints for Microsoft accounts and Microsoft Entra ID scenarios, including Graph and Office substrate services. Noted that endpoints may evolve and linked to related resources to keep network policies current.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/add-copilot-endpoints-allowlist

## Major Changes

- **Microsoft Copilot app**

  Overhauled the article to reflect the Microsoft Copilot app, separating personal (Microsoft account) and work or school (Microsoft Entra ID) experiences with guidance on account switching and data separation. Clarified client availability across web, desktop (Windows, macOS), and mobile (Android, iOS), and that Copilot licenses unlock the full experience. Added admin and deployment guidance, including the ability to limit personal account access via Tenant Restrictions. Introduced client app requirements and network allow-list guidance for Unified Domains and Copilot endpoints, with links to deployment and management for desktop and mobile.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/microsoft-365-copilot-app-overview

- **Use Copilot Cowork**

  Added detailed guidance on how Cowork evaluates skills, covering evaluation depths (Minimal, Standard, Full, Maximal), static and behavioral checks, scoring dimensions, gating criteria, and the Skill Report outputs. Included common evaluation issues to help authors troubleshoot and improve skills before deployment. Updated UI terminology by renaming the “Scheduled” status/category to “Automations” across the experience.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/use-cowork

## Moderate Changes

- **Copilot Cowork common questions**

  Removed references to the “effort level” setting next to the model picker to align with current UI and behavior. This reduces confusion by eliminating guidance for a control that’s no longer applicable.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/cowork-faq

- **Choose a model for Copilot Cowork**

  Removed guidance about setting the effort level (Light through Max) and where those controls appear. The page now focuses on model selection without describing deprecated effort options.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/cowork-models

- **Cowork network endpoints**

  Updated entry points to reference Microsoft Copilot Chat and changed the chat host to copilot.cloud.microsoft. Standardized allow-list guidance, including a recommended wildcard (*.gateway.prod.island.powerapps.com:443), and refreshed destination tables while retaining required Microsoft Entra ID and Graph endpoints. Adjusted minimum requirements to reflect correct application ID formatting and updated URLs.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/cowork-network-endpoints

- **Build plugins for Copilot Cowork**

  Added guidance that SKILL.md is limited to 20,000 characters and recommends keeping instructions under ~5,000 tokens, moving details to referenced files. Clarified that custom plugins using an MCP connector aren’t supported on mobile, while skills-only packages continue to work.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/cowork-plugin-development

- **Data, privacy, and security for web search in Microsoft Copilot and Microsoft Copilot Chat**

  Expanded coverage to include Cowork alongside Researcher and Analyst and clarified which experiences have a Web search toggle. Updated policy behavior so that disabling web search in Copilot Work mode also disables it for Researcher and Cowork.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/manage-public-web-access

- **Application card: Microsoft Copilot (for organizations)**

  Rebranded from Microsoft 365 Copilot to Microsoft Copilot (for organizations) and aligned terminology across all sections without changing feature scope. Added a privacy/rebrand include and a note clarifying organizational applicability with a link to transparency guidance for individuals; updated references to new product names and experiences.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/microsoft-365-copilot-application-card

- **How does Microsoft Copilot work?**

  Updated naming from “Microsoft 365 Copilot” to “Microsoft Copilot” throughout the page, including headings and related links. Technical architecture and data flow explanations remain unchanged.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/microsoft-365-copilot-architecture

- **License options for Microsoft Copilot**

  Rebranded the licensing article to “Microsoft Copilot,” aligning titles, headings, and references. Licensing options and guidance are unchanged.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/microsoft-365-copilot-licensing

- **Microsoft 365 app and network requirements for Microsoft 365 Copilot**

  Expanded network guidance to explicitly allow *.cloud.microsoft and copilot.cloud.microsoft, and updated WebSockets requirements. Added recommendations to avoid legacy blocks, use Tenant Restrictions to control personal accounts, coordinate with security teams, and validate connectivity using the Microsoft 365 Connectivity Test tool.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/microsoft-365-copilot-requirements

- **Microsoft Copilot Search**

  Rebranded from “Microsoft 365 Copilot Search” to “Microsoft Copilot Search,” updating titles, descriptions, and comparison tables. Adjusted references to licensing and app access; no feature changes were introduced.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/microsoft-365-copilot-search