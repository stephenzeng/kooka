# Microsoft Copilot Studio
**Date created:** 2026-07-25 UTC  
**Tags:** Administration, Agent, Analytics, Monitoring, Security  

## Major Changes

- **Monitor agents using Agent Inventory in Copilot Agent Kit**

  Rebranded the article to Copilot Agent Kit and expanded coverage to include declarative agents. Added a new “Take actions on agents” section detailing how to view details, reassign, quarantine, and unquarantine agents, with clear rules for when actions are available. Introduced data collection modes, recommending One Inventory with Power Platform admin center integration and documenting a Standard fallback, including required connectors and access. Expanded usage metrics guidance to a 180‑day window with clearer refresh behavior and configuration steps for the HTTP with Microsoft Entra ID connector using cloud-specific endpoints, plus notes on live vs. synced status and related connector requirements.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/kit-agent-inventory

- **Troubleshoot errors in Copilot Agent Kit**

  Updated product naming to Copilot Agent Kit and significantly expanded data policy guidance with a connector-to-feature mapping and a link to connector requirements. Clarified authentication setup for KitAuthApp and CopilotStudioAuthApp with detailed checklists for redirect URIs, flows, scopes/permissions, client secrets, and custom scopes. Improved agent configuration guidance (token endpoint, Entra ID v2, channel security), reinforced tenant alignment, and refined publish/test steps, along with an updated note on the kit’s open-source support and licensing.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/kit-troubleshoot

## Moderate Changes

- **Monitor agent performance with Agent Insights Hub in Copilot Agent Kit**

  Updated troubleshooting to remove the instruction to import the AgentInventoryUsage solution and to require configuring the HTTP with Microsoft Entra ID (preauthorized) connection to the Power Platform licensing API with a cloud-specific Base Resource URL. Added a reference to viewing usage metrics while keeping role requirements unchanged, streamlining setup and reducing unnecessary steps.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/kit-agent-insights-hub

- **Install Copilot Agent Kit**

  Rebranded all references from Copilot Studio Kit to Copilot Agent Kit across titles, descriptions, and in-product steps. Removed the “Enable usage metrics” subsection that previously covered connector allowance, managed package import, and licensing host configuration, simplifying the installation guidance without introducing new procedures.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/kit-install

- **Copilot Agent Kit prerequisites**

  Overhauled connector requirements to mandate that data policies allow all Copilot Agent Kit connectors and that connections are provided during solution import. Added a comprehensive, feature-mapped connector list (including Power Platform for Admins V2, Microsoft Teams, Office 365 services, Approvals, SharePoint Online, Power Apps for Makers, HTTP with Microsoft Entra ID, Microsoft Copilot Studio) and clarified Microsoft Dataverse usage across kit components.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/kit-prerequisites