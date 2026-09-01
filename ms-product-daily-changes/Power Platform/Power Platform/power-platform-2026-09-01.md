# Power Platform
**Date created:** 2026-09-01 UTC  
**Tags:** Compliance, Configuration, Deprecation, Governance, Guidance, Security, Troubleshooting  

## New Articles

- **Web API Requests Fail After Wildcard Column Deprecation**

  Introduced a new troubleshooting and migration guide for the deprecation of the wildcard (*) in Power Pages Web API field configuration, directing customers to explicit column allow lists. Explains symptoms, causes, and two migration paths: a manual approach and tooling-based options using the Security Agent and Power Pages plugin (available from Sep 2, 2026). Provides the deprecation timeline (new sites blocked in Aug 2026; all sites blocked Sep 14, 2026), testing and validation steps, FAQs, and references. Emphasizes least-privilege configuration and improved auditing to reduce risk and simplify governance.

  https://learn.microsoft.com/en-us/troubleshoot/power-platform/power-pages/migrate-web-api-wildcard

## Moderate Changes

- **Power Platform and Dynamics 365 macro region geography**

  Expanded guidance on macro region placement, including allow-listing behavior without ADR, affinity examples across regions, and planning for potential datacenter shifts. Added ADR eligibility details and clarified that data-at-rest commitments for Dynamics 365/Power Platform derive from product terms when ADR is enabled for all Microsoft 365 seats. These updates help admins plan environment placement for test/dev/prod and align governance with regional and ADR considerations.

  https://learn.microsoft.com/en-us/power-platform/admin/macro-regions