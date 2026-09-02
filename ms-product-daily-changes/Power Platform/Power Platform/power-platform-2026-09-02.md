# Power Platform
**Date created:** 2026-09-02 UTC  
**Tags:** Compliance, Configuration, Deprecation, Governance, Guidance, Licensing, Troubleshooting  

## Major Changes

- **Power Platform environments overview**

  Removed the entire Preferred environment location guidance, including related PowerShell instructions, ADR/macro region requirements, and multi-geo considerations. Updated the environment location table to eliminate references to modifying location via the removed feature and clarified entries (including Developer) to reflect tenant home location or creation-time selection. This streamlines environment location guidance and avoids pointing admins to settings that are no longer supported, reducing confusion in deployment planning.

  https://learn.microsoft.com/en-us/power-platform/admin/environments-overview

- **Licensing requirements for managed environments**

  Expanded and restructured guidance to define the managed environments licensing compliance initiative with a two-stage approach: notifications followed by enforcement. Starting February 2027, users without appropriate licenses will be blocked from opening apps in managed environments after the final notification stage, with notifications for users and admins continuing post-enforcement. Clarified scope (all active app users in managed environments), qualifying licenses across apps, flows, and agents, and recommended that admins proactively review and assign licenses ahead of enforcement to prevent access loss.

  https://learn.microsoft.com/en-us/power-platform/admin/managed-environment-licensing

- **Power Apps licensing FAQs**

  Significantly expanded and reorganized the FAQ, adding a Licensing compliance for Power Apps section detailing stricter enforcement starting February 2027 and impacted scenarios (managed environments, model-driven apps, and apps used outside a licensed Dynamics 365 context). Clarified how to identify users who need licenses, premium capability requirements, and Power Automate nuances (including child vs. parent flow and Process license behavior). Added practical guidance on purchasing and trials, per app capacity allocation, developer environment use, and environment access expectations to help admins prepare for enforcement.

  https://learn.microsoft.com/en-us/power-platform/admin/powerapps-licensing-faq

## Moderate Changes

- **Connect to GitHub (preview)**

  Updated guidance to use preview maker portals and endpoints for GitHub integration and refreshed step-by-step instructions and URLs. Clarified authentication by allowing a GitHub PAT as an alternative to a GitHub connection, which is especially useful when VNET restrictions prevent creating connections. Noted that the same GitHub app and Azure Key Vault configuration can be reused across multiple repositories and environments to simplify setup.

  https://learn.microsoft.com/en-us/power-platform/alm/git-integration/connecting-to-github

- **Recover a recently deleted environment**

  Clarified recovery windows: a standard 7-day soft-delete period and a 28-day exception for production environments with Dynamics 365 apps, with links to detailed restore guidance. Streamlined admin center steps and expanded post-recovery validation, including re-enabling solution-aware flows, verifying connections and application users, and testing apps and integrations to ensure full functionality after recovery.

  https://learn.microsoft.com/en-us/power-platform/admin/recover-environment