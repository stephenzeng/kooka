# Power Platform
**Date created:** 2026-08-14 UTC  
**Tags:** Analytics, Billing, Configuration, Consumption, Governance, Guidance, Identity, Monitoring, Security  

## New Articles

- **Manage costs for agents powered by the GitHub Copilot harness**

  Introduced comprehensive guidance for controlling and monitoring Copilot Credit consumption for agents using the GitHub Copilot harness. Explains environment-level controls (credit allocation, disable tenant capacity draw) and agent-level monthly limits with notifications and stop-usage. Covers programmatic allocation via APIs/SDK, pay-as-you-go cost management with Azure budgets, and multi-level monitoring (tenant, environment, agent, reports). Details how to identify GitHub Copilot harness agents and coordinate capacity across Power Platform and Microsoft 365. Highlights key actions to prepare for end-of-preview billing ahead of September 1, 2026.

  https://learn.microsoft.com/en-us/power-platform/admin/manage-usage-github-copilot-harness

## Moderate Changes

- **Continuous access evaluation**

  Updated the article from preview to general availability with clear availability timelines: GA for Dataverse in public cloud and phased rollout to sovereign clouds from August to mid-September 2026. Clarified that no enablement steps are required, removed prior “contact support” guidance, and removed the prerelease disclaimer to streamline adoption.

  https://learn.microsoft.com/en-us/power-platform/admin/continuous-access-evaluation

- **Geo-to-geo migrations**

  Added a prerequisite requiring the Advanced Data Residency (ADR) SKU add-on for new environments created under macro region geography before requesting a migration. Refined migration guidance with clearer pre- and post-migration actions, component handling (inside and outside solutions), and clarified cutover impacts on accessibility and lifecycle operations without changing core procedures.

  https://learn.microsoft.com/en-us/power-platform/admin/geo-to-geo-migrations

- **Power Platform inventory sample queries**

  Revised the sample to classify agents by harness using isCLIAgent, model, and createdIn, and to summarize counts per harness (GitHub Copilot, Copilot Chat, Standard) in order of volume. This shifts from filtering and listing to a concise, count-focused report suitable for usage analysis.

  https://learn.microsoft.com/en-us/power-platform/admin/inventory-sample-queries