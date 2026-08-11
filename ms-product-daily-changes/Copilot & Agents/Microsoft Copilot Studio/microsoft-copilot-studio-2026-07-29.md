# Microsoft Copilot Studio
**Date created:** 2026-07-29 UTC  
**Tags:** AI, Agent, Monitoring, Programming  

## New Articles

- **Environment-level telemetry with Application Insights (preview)**

  Introduced a new how-to for exporting Copilot Studio agent telemetry at the environment level to Azure Application Insights via the Power Platform admin center. The article explains exported spans (InvokeAgent, ExecuteTool, OutputMessages), how traces align with OpenTelemetry semantics, and key customDimensions. It provides prerequisites, end-to-end setup steps, validation guidance, and extensive Kusto query examples for analyzing runs, tools, models, and multi-agent conversations. Known limitations and preview considerations are documented to guide adoption and troubleshooting.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/advanced-environment-level-agent-telemetry

- **Telemetry with Application Insights overview**

  Added a conceptual overview that contrasts agent-level and environment-level telemetry for Copilot Studio. It clarifies configuration scope, ownership, required privileges, target audiences, operating models, telemetry models, and primary Application Insights tables, highlighting when to use each approach. The article notes that Application Insights is part of Azure Monitor and requires an Azure subscription, and links to detailed configuration for both scopes to help teams choose the right observability model.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/telemetry-overview

## Moderate Changes

- **Add tools to custom agents**

  Clarified what counts as “tool-like” by explicitly referencing Azure Bot Service skills and client tools. Added guidance on differences between classic agent skills and coding agent skills, emphasizing that only coding agent skills can be added in the new agent experience to prevent configuration errors.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/add-tools-custom-agent

- **Agent-level telemetry with Application Insights**

  Retitled and refreshed terminology from bot to agent, and consolidated guidance for viewing telemetry and running Kusto queries. Added step-by-step instructions to disable agent-level telemetry using a Power Platform data policy by blocking the “Application Insights in Copilot Studio” connector, with links to related telemetry resources for broader context.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/advanced-bot-framework-composer-capture-telemetry

- **Configure Azure Bot Service skills for use in Copilot Studio agents**

  Updated the page to consistently reference Azure Bot Service skills and clarified that existing bots can be converted into skills and registered with a Copilot Studio agent. Language was standardized from singular to plural “skills” to reduce ambiguity, without introducing new procedures.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/configuration-add-skills

- **Overview of the Microsoft Copilot Studio extension for Microsoft Visual Studio Code**

  Streamlined the page by removing general platform background, focusing the content on the VS Code extension. Section headings and brief framing text were refined to better guide local development and team workflows, with no new features or steps added.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/visual-studio-code-extension-overview