# Visual Studio
**Date created:** 2026-08-20 UTC  
**Tags:** Best Practices, Billing, Configuration, Consumption, Governance, Guidance, Monitoring  

## Major Changes

- **Use custom agents in GitHub Copilot**

  Added guidance for organization-level custom agents, including requirements (the repository must belong to a GitHub organization) and how Visual Studio automatically discovers and lists these agents in the agent picker. Provides steps to review an agent’s description and source organization and to open its definition, with links to GitHub setup guidance for organization and enterprise owners. Removed the prior limitation that the agent picker was exclusive to the Visual Studio 2026 Insiders build, reflecting broader availability and easier team adoption.

  https://learn.microsoft.com/en-us/visualstudio/ide/copilot-specialized-agents?view=visualstudio

- **GitHub Copilot usage and models**

  Expanded guidance on usage-based billing with GitHub AI Credits, including how tokens (input/output/cached) affect costs, pooled credits for Business/Enterprise, and proactive alerts as you approach limits. Clarifies what happens when included usage is exhausted across Individual, Business, and Enterprise plans, and outlines monthly completion limits for Copilot Free. Improves model selection advice with Auto routing, organizing and pinning models, and connecting custom models via API key, plus clearer context-window indicators and tips to optimize cost, performance, and response quality.

  https://learn.microsoft.com/en-us/visualstudio/ide/copilot-usage-and-models?view=visualstudio

## Moderate Changes

- **Customize chat responses**

  Added organization-level custom instruction guidance, including how owners set them up in GitHub, how they appear in References, and how to disable them in Visual Studio. Clarified how user preferences are stored and interact with repository-level instructions, and refined prompt files and slash command behaviors to improve day-to-day prompting workflows.

  https://learn.microsoft.com/en-us/visualstudio/ide/copilot-chat-context?view=visualstudio