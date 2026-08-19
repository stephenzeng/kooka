# Dynamics 365 Customer Insights
**Date created:** 2026-08-19 UTC  
**Tags:** Configuration, Governance, Guidance, Identity, Security, Troubleshooting  

## New Articles

- **Troubleshoot Personalization in Customer Insights - Journeys**

  Introduced a troubleshooting guide that explains why dynamic content can render empty or behave unexpectedly by contrasting preview (signed-in user) versus live execution (service account) contexts. It details common root causes such as business unit scoping, field-level security, data timing issues, and Dataverse customizations/plugins affecting queries. The article provides step-by-step diagnostics and practical mitigations, including adding defaults, inserting waits, and ensuring data readiness. It also links to related guidance on ownership, FLS, business units, service users, personalization, and auditing to help teams resolve production issues faster.

  https://learn.microsoft.com/en-us/troubleshoot/dynamics-365/customer-insights/journeys/personalization/troubleshoot-personalization

## Moderate Changes

- **Connect to a Power Query data source**

  Updated prerequisites to require Admin-level permissions (and dataflow ownership) for creating or editing Power Query data sources, reflecting configuration of the environment’s Dataverse managed data lake. Added troubleshooting for save validation errors, including table/column naming rules, handling downstream dependencies after deletions, selecting a single primary key for incremental refresh, and removing unsupported complex column types. These changes clarify permissions and help prevent common setup and save failures.

  https://learn.microsoft.com/en-us/dynamics365/customer-insights/data/connect-power-query

- **User roles**

  Clarified role capabilities for Power Query data sources: only Admins can create or edit due to managed data lake configuration, while Contributors can view data sources and refresh those they own but cannot create or edit. The role matrix and notes were updated to reflect these governance and security requirements.

  https://learn.microsoft.com/en-us/dynamics365/customer-insights/data/user-roles