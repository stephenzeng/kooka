# Microsoft 365 Copilot
**Date created:** 2026-07-11 UTC  
**Tags:** Administration, Agent, Governance, Monitoring  

## Major Changes

- **Use Microsoft 365 Admin agent**

  Reworked the article into a practical how-to and clarified that the Admin agent is available only in Microsoft 365 Copilot Chat and the Microsoft 365 admin center, removing references to specialized admin centers. Added step-by-step instructions for launching and using the agent, emphasized RBAC-driven permissions, and reinforced that explicit confirmation is required before any write or execute action. Clarified auditing behavior and updated FAQs to focus on governance options to block or scope access rather than enablement steps. Streamlined headings and wording, including renaming sections to reflect the Microsoft 365 admin center as the primary entry point.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/copilot-ai-admin-agent

- **Managing AI experiences enabled by usage-based billing**

  Added guidance for CSPs, partner-managed, and MACC customers, including how to link Azure subscriptions to the correct billing account and how MACC applies to Copilot consumption. Clarified spending policy behavior: the default tenant policy sets tenant-level limits, and additional policies maintain independent limits. Referenced a centralized list of services covered by usage-based billing and documented data refresh cadences (Overview tab every 4 hours; Consumption tab every 2 hours). Explained why group and user-level spending can differ due to users belonging to multiple groups and overlapping policies.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/usage-based-billing-manage-copilot-credits

## Moderate Changes

- **OpenAI as a subprocessor in Microsoft Online Services**

  Removed guidance that enabling OpenAI operated models is required to use GPT 5.6. This clarifies prerequisites and reduces confusion for administrators planning model enablement and governance.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/openai-subprocessor