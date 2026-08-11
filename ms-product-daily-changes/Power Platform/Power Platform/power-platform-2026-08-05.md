# Power Platform
**Date created:** 2026-08-05 UTC  
**Tags:** Administration, Governance, Security  

## Moderate Changes

- **Data storage and governance in Power Platform**

  Expanded data residency guidance to a macro region geography model where admins choose a macro region and the platform selects the optimal datacenter within it. Clarified multi-geo terminology (home vs. remote macro geos) and reinforced that performance and availability are balanced while meeting residency commitments.

  https://learn.microsoft.com/en-us/power-platform/admin/security/data-storage

- **Manage Copilot Studio credits and capacity**

  Added notice that Copilot Studio is a multi-harness platform and that the Power Platform admin center offers unified capacity management across Copilot Chat, Standard, and GitHub Copilot. Administrators can now view capacity and consumption at both the agent and environment levels for clearer oversight and planning.

  https://learn.microsoft.com/en-us/power-platform/admin/manage-copilot-studio-messages-capacity

- **Power Platform URLs and IP address ranges**

  Added https://mem.gfx.ms to the allow-list as a service endpoint for application-to-service communication. This helps ensure required traffic is not blocked in restricted network environments.

  https://learn.microsoft.com/en-us/power-platform/admin/online-requirements

- **On-premises data gateway management**

  Introduced tenant migration guidance requiring full removal of gateways in both home (default) and target regions before migration, with step-by-step actions and visuals. Also clarified gateway installer management details, improving reliability and reducing migration issues.

  https://learn.microsoft.com/en-us/power-platform/admin/onpremises-data-gateway-management

- **Security enhancements for user sessions and access management**

  Clarified default governance by Microsoft Entra session policy, token refresh behavior, and exceptions, and detailed environment-level session timeout controls with min/max values and warning behavior. Expanded inactivity timeout guidance with enforcement details, configuration steps, and prerequisites (including ClientGlobalContext.js.aspx), and noted that portal settings are independent. Refined access management requirements and added outage resilience notes to strengthen operational readiness.

  https://learn.microsoft.com/en-us/power-platform/admin/user-session-management