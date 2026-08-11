# Microsoft Viva
**Date created:** 2026-07-31 UTC  
**Tags:** Administration, Agent, Analytics, Governance  

## Major Changes

- **Connect to the Agent Dashboard**

  Introduced two distinct reporting views—Copilot Agent Dashboard and Agent 365 Dashboard—clarifying scope, core metrics (Agent responses vs. Sessions), and reporting history. Added an Overview page with top-level adoption cards, agent creation insights by creator type, and a shared user agents metric, alongside clearer licensing requirements and aligned filters across pages. Enhanced Adoption and deep-dive experiences with view-specific metrics (including Sessions in the Agent 365 view and Copilot Credit visibility constraints), expanded “View by” options, and refined metric definitions and availability. Expanded the Agent snapshot with per-view default ordering, new optional columns (Versatility and Shared across orgs), hover descriptions in Agent 365, and guidance when insights are unavailable due to privacy thresholds or inactivity.

  https://learn.microsoft.com/en-us/viva/insights/org-team-insights/agent-dashboard

- **Roles in Viva Amplify**

  Simplified admin role requirements by removing the Microsoft 365 Groups admin role, clarifying that only the SharePoint admin role is required to configure and set up Viva Amplify. The admin roles table and accompanying descriptions were updated to reflect this change and to streamline guidance across introductory and user roles sections. This reduces permissions overhead and clarifies who is responsible for setup and configuration.

  https://learn.microsoft.com/en-us/viva/amplify/viva-amplify-roles

## Moderate Changes

- **Manage settings for the Microsoft Copilot Dashboard, Agent Dashboard, and Viva Insights web app**

  Added a VFAM control to determine whether the Agent 365 Dashboard includes non-public agents or only public agents, with the default set to include all agents. Clarifies definitions of non-public (Your org or user) versus public (Microsoft or third-party) agents and allows AI admins to scope the setting at tenant, group, or user level. Includes a PowerShell example referencing FeatureId Agent365DashboardNonPublicAgentsVisibility for automated configuration.

  https://learn.microsoft.com/en-us/viva/insights/advanced/admin/manage-settings-copilot-dashboard

- **Advanced analysis metrics**

  Added a new “Sessions (Agent measurement)” metric that defines a session as a continuous interaction starting anew after 30 minutes of inactivity. The metric reports the number of agent sessions with at least one active user over the last 28 days, helping teams assess agent engagement and usage patterns.

  https://learn.microsoft.com/en-us/viva/insights/advanced/reference/metrics