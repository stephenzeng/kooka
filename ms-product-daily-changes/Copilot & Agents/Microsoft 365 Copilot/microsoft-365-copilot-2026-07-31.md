# Microsoft 365 Copilot
**Date created:** 2026-07-31 UTC  
**Tags:** Administration, Governance, Monitoring, Programming  

## Moderate Changes

- **Build plugins for Copilot Cowork**

  Clarified that API key authentication isn’t supported for Copilot Cowork plugins. Updated guidance directs developers to use OAuthPluginVault or Dynamic Client Registration, or to expose an endpoint that accepts None when an MCP server expects an API key. This helps prevent authentication failures and aligns implementations with supported security models.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/cowork-plugin-development

- **Managing AI experiences enabled by usage-based billing**

  Expanded admin guidance for spending policies, including navigation, policy priority logic, and movement between groups, emphasizing that policies set limits rather than allocate credits. Clarified billing behavior when prepaid credits run out (automatic pay-as-you-go), interactions with capacity packs and P3 credits, and added advanced pay-as-you-go settings for billing region and resource groups. Strengthened reporting guidance with active user definitions, a 2-hour refresh cadence, point-in-time export behavior, and handling of overages without auto-switching users between policies.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/usage-based-billing-manage-copilot-credits