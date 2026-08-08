# Microsoft 365 Copilot
**Change date:** 2026-08-07 UTC  
**Tags:** Administration, Agent, Monitoring  

## New Articles

- **Check your credit usage for Cowork tasks with `/Cost`**

  Introduced a how-to article for using `/Cost` in Copilot Cowork to see estimated credits for the current task and remaining monthly balance. Explains how credits aggregate within a session, monthly reset behavior, and differences between individual and group usage plans. Clarifies that `/Cost` is for estimates only—not for billing reconciliation, policy management, or historical analytics. Includes FAQs on delayed balance updates, no credit carryover, what happens when credits run out, and the lack of pre-run cost checks, with links to related licensing and usage-based billing resources.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/ubb-cost-skill

## Moderate Changes

- **Managing AI experiences enabled by usage-based billing**

  Clarified spending policy behavior when users change Entra ID groups mid-period: prior usage remains billed to the previous policy, the dashboard shows the current Monthly limit, and Total credits used aggregates usage across all policies for the period; also refined chart definitions so Prepaid credits include Message/Capacity Packs and Pay-as-you-go usage includes credits from a Pre-Purchase Plan. Added a user-facing note on using `/Cost` in Copilot Cowork to view approximate credit usage, with a link to detailed guidance.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/usage-based-billing-manage-copilot-credits

- **Release notes, known issues, and limitations for the Employee Self-Service agent**

  Updated release notes to clarify that package versions are independent and to label Core, HR, IT, and ServiceNow integration packages. Reworked the table to “Package versions” and mapped features to specific package-version groups. Refined the GPT-5.5 upgrade entry to list package-specific versions across SuccessFactors, Workday, and ServiceNow integrations, helping admins track capabilities by package.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/employee-self-service/known-issues-limitations