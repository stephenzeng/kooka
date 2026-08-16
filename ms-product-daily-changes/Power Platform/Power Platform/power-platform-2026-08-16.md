# Power Platform
**Date created:** 2026-08-16 UTC  
**Tags:** Analytics, Automation, Best Practices, Configuration, Consumption, Deprecation, Governance, Guidance, Licensing, Monitoring, Security  

## Major Changes

- **Exchange Online cross-tenant authentication**

  Announced the phased retirement of Exchange Web Services (EWS) in Exchange Online, with allowlisting requirements starting October 2026 and full retirement by April 2027. Power Platform cross-tenant email synchronization will transition to Microsoft Graph by April 2027. Admins must allowlist tenants/apps for EWS during the transition and configure Microsoft Graph application permissions using either a provided PowerShell script or manual Azure portal steps. The article specifies the necessary Graph application permissions to ensure continuity.

  https://learn.microsoft.com/en-us/power-platform/admin/connect-exchange-online-server-profile-oauth

- **Elastic compute for finance and operations apps**

  Clarified that Power Apps Premium, Dynamics 365 customer engagement, and finance and operations licenses all contribute to a single tenant-level Power Platform Requests (PPR) pool used across Dataverse and finance and operations apps. Introduced a PowerShell-based method to retrieve tenant PPR capacity via the Power Platform API and translate it into AOS capacity, including prerequisites and calculation logic (650,000 PPRs per AOS; min 2, max 80). This helps admins plan scaling, monitor capacity, and align AOS provisioning with available PPRs.

  https://learn.microsoft.com/en-us/power-platform/admin/unified-experience/elastic-compute

- **Programmability and extensibility - what's new or changed**

  Added a July 2026 roundup of new and enhanced API endpoints spanning Copilot Studio, Dynamics 365 Finance and Operations, environment management, licensing and entitlement insights, and Power Pages (including WAF policy updates). Noted bug fixes for the “Provision New Environment” API. Highlighted ongoing monthly releases of the Power Platform Management SDKs (Python and C#) and the Power Platform for Admins V2 connector to keep automation scenarios current.

  https://learn.microsoft.com/en-us/power-platform/admin/programmability-whats-new-changed

## Moderate Changes

- **Requests limits and allocations**

  Clarified how service principal–owned flows consume action limits: when covered by a Process or per-flow license, assigned to a flow group with a Process license, or linked to a designated licensed user, the flow uses those licensed limits rather than the non-licensed user pool. This helps admins align flow ownership and licensing to avoid unintended throttling.

  https://learn.microsoft.com/en-us/power-platform/admin/api-request-limits-allocations

- **Dataverse capacity-based storage details**

  Added detailed guidance on how storage overages are calculated, including cross capacity-type borrowing rules and examples. Clarified that alerts consider effective capacity after borrowing, but environment lifecycle operations are validated per storage type and can be blocked even when effective capacity appears sufficient. Minor wording improvements enhance capacity views and advisor UI clarity.

  https://learn.microsoft.com/en-us/power-platform/admin/capacity-storage

- **Power Automate licensing FAQ**

  Expanded licensing guidance, including the option to designate a licensed user for service principal–owned flows, clearer coverage for Process licenses, and whose action limits apply in various ownership scenarios. Improved explanations of action limits, throttling, overage handling, and best practices, with updated examples for reducing usage and scaling flows.

  https://learn.microsoft.com/en-us/power-platform/admin/power-automate-licensing/faqs

- **Dataverse capacity-based storage overview**

  Updated overage and operations guidance to note that notification banners evaluate thresholds after cross-type borrowing, while environment lifecycle operations are checked against per-type capacity. Clarified restricted actions and removed prior language suggesting exceeding entitlements doesn’t affect service availability.

  https://learn.microsoft.com/en-us/power-platform/admin/whats-new-storage