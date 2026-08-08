# Dynamics 365 Customer Insights
**Change date:** 2026-08-07 UTC  
**Tags:** Administration, Automation, Security  

## New Articles

- **Permission changes in the March 2026 release (version 1.1.62960.43)**

  Introduced a dedicated article detailing out-of-the-box role permission changes for the March 2026 release. It outlines per-role add/remove/update changes for core event and marketing roles, including BU-level variants. The update adds new event and marketing tables with defined privilege scopes, introduces Workflow/WorkflowSession AppendTo privileges, and adjusts privilege levels across many entities. It also removes legacy SDK-related tables from Lead Score Modeler (BU) and provides granular read/write/create/append/append-to scope details to help admins keep custom roles aligned.

  https://learn.microsoft.com/en-us/dynamics365/customer-insights/journeys/role-permissions-2026-03

- **Permission changes in the April 2026 release (version 1.1.64196.86)**

  Added a new article documenting April 2026 permission updates focused on the msdynmkt_agentsetting table. Four marketing roles received full privileges with scopes tailored to Global, Deep, or Local, while other roles remain unchanged. The article includes role identifiers, metrics, and a tabular changelist to make it easier to validate and update custom security configurations.

  https://learn.microsoft.com/en-us/dynamics365/customer-insights/journeys/role-permissions-2026-04

- **Permission changes in the May 2026 release (version 1.1.65002.146)**

  Published a confirmation that no changes were made to out-of-the-box role permissions in the May 2026 release. The article directs readers to the overall permission change list to validate current baselines and ensure custom roles remain compliant.

  https://learn.microsoft.com/en-us/dynamics365/customer-insights/journeys/role-permissions-2026-05

- **Permission changes in the June 2026 release (version 1.2.437.94)**

  Introduced a comprehensive article covering significant June 2026 role permission updates across nine roles, with breaking changes in seven. It details large-scale additions, removals, and privilege level shifts, including new lead scoring and compliance entities and the removal of legacy/portal items. The article highlights broadened or reduced scopes where applicable and provides per-role changelists to guide remediation. Admins should review and reconcile custom roles to prevent access gaps or unintended privileges.

  https://learn.microsoft.com/en-us/dynamics365/customer-insights/journeys/role-permissions-2026-06

## Major Changes

- **Permission changes overview**

  Reorganized the page into a clear overview that explains how to use baseline and per-release pages to keep custom roles synchronized. Clarified terminology (for example, BU as business unit) and the scope implications for BU-level roles. Moved release-by-release logs for March–June 2026 into separate pages and streamlined guidance throughout to improve discoverability and maintenance workflows.

  https://learn.microsoft.com/en-us/dynamics365/customer-insights/journeys/role-permissions

## Moderate Changes

- **New and upcoming features**

  Updated descriptions to emphasize that dynamic content blocks can automatically refresh emails when source content changes. Expanded personalization guidance by describing how PowerFx expressions can format text, dates, and numbers and perform simple calculations. No new sections or structural changes were introduced.

  https://learn.microsoft.com/en-us/dynamics365/customer-insights/journeys/whats-new-marketing