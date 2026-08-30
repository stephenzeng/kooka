# Power Platform
**Date created:** 2026-08-30 UTC  
**Tags:** Billing, Configuration, Consumption, Governance, Guidance, Troubleshooting  

## Moderate Changes

- **Rules for environment groups**

  Added a new “Cost controls - Draw from tenant credit pool” rule to help admins control whether environments can consume tenant Copilot Credits, expanding the list to 24 rules and renumbering items. Moved “Content security policy” to the final position to reflect the updated ordering and governance guidance.

  https://learn.microsoft.com/en-us/power-platform/admin/environment-groups-rules

- **Power Platform white papers**

  Updated the white paper catalog by removing the “Migrating apps and flows from the default environment” entry. This keeps the guidance list current and avoids directing readers to retired content.

  https://learn.microsoft.com/en-us/power-platform/guidance/white-papers/

- **Manage costs for agents powered by the GitHub Copilot harness**

  Updated guidance clarifying how the environment group rule “Draw from tenant credit pool” governs consumption of tenant Copilot Credits, including default behavior for eligible environments and how to cap usage at environment allocations. Explained that publishing the rule enforces it across all environments (making the environment-level setting read-only) and outlined options to retain environment-level control or rely on a linked pay-as-you-go plan.

  https://learn.microsoft.com/en-us/power-platform/admin/manage-usage-github-copilot-harness

- **Manage Copilot Credits allocations programmatically**

  Added a warning that programmatic attempts to override the “Draw from the available capacity in my tenant” setting are rejected with TenantPoolLockedByPolicy when governed by an environment group rule. Provided steps to change and republish the rule or remove the environment from the group to manage the setting independently, noting the last applied value persists after removal.

  https://learn.microsoft.com/en-us/power-platform/admin/programmability-tutorial-manage-copilot-credit-allocations