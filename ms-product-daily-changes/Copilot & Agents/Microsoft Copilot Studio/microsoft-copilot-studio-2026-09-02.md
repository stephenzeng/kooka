# Microsoft Copilot Studio
**Date created:** 2026-09-02 UTC  
**Tags:** Best Practices, Configuration, Get Started, Guidance, Troubleshooting  

## Major Changes

- **Available knowledge sources for agents**
  
  Expanded the knowledge source catalog to explicitly list Featured (Public websites, SharePoint, OneDrive for Business, Salesforce, ServiceNow) and Advanced (Azure DevOps Wiki, Azure DevOps Work Items, Custom Connector, Enterprise websites) options. Added guidance for preparing Dataverse data using a Power Apps Data Workspace link that appears during table selection when prerequisites are met. Introduced an admin-focused section explaining how environment Dataverse search-and-index settings can block adding or retrieving from Dataverse, Dynamics 365, and uploaded-file sources, with steps to resolve. Removed the Azure AI Search section and related guidance to reflect current capabilities.
  
  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/knowledge-sources-overview

## Moderate Changes

- **Create and delete agents**
  
  Updated to focus on agents powered by the standard harness, adding a prerequisite to turn off the New experience (and dismiss Feedback) to reach the correct Home page. Refreshed creation steps and labels: choose Agent from Start building from scratch, then name the agent, optionally adjust Advanced settings (language, solution, schema), and select Create; removed the previous advanced down-arrow flow. Streamlined deletion guidance and clarified that the Teams app steps apply to classic chatbots, removing the immediate-deletion note.
  
  https://learn.microsoft.com/en-us/microsoft-copilot-studio/authoring-first-bot

- **Quickstart: Create and deploy an agent with the standard harness**
  
  Added a prerequisite to turn off the New experience (and dismiss or submit Feedback) so the Home page matches the standard harness. Refocused testing guidance on changing the agent’s instructions (tone) and comparing results by asking the same question, removing prior knowledge-source imagery and narrative.
  
  https://learn.microsoft.com/en-us/microsoft-copilot-studio/fundamentals-get-started

- **Manage knowledge sources in an agent**
  
  Updated UI instructions to the Build tab with a right-panel Knowledge section where sources are shown as chips and managed directly, including removal via the × button. Web search is now enabled or disabled by adding/removing the “Search all websites” chip. Added troubleshooting explaining how environment Dataverse search-and-index settings can stop Dataverse, Dynamics 365, or uploaded-file retrieval, and that admins can restore functionality without re-adding sources.
  
  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/knowledge-edit-source