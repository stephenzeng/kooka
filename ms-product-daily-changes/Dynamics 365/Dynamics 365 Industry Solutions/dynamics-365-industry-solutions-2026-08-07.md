# Dynamics 365 Industry Solutions
**Date created:** 2026-08-07 UTC  
**Tags:** Administration, Analytics  

## Major Changes

- **Configure reporting years**

  Overhauled reporting period management by introducing a new “Lock a reporting period” flow and adding a third status, “Restricted,” alongside Open and Closed. The Restricted status enables entity-level locking with configurable exclusions, with step-by-step setup guidance and visual examples. Guidance now clarifies the behavior of each status and streamlines steps for reopening periods, while removing older edit workflows and outdated notes.

  https://learn.microsoft.com/en-us/industry/sustainability/setup-reporting-years

## Moderate Changes

- **Calculate reporting metrics**

  Added a preview “Derived metrics” capability to build reporting metrics from Aggregation node outputs, including support for multiple aggregations, group-by, and organization-wide totals. Clarified Aggregate Input constraints (single-row outputs, supported node types only, unit consistency, no currency conversion or hierarchy rollups) and provided an end-to-end renewable energy percentage example with updated visuals. Content was reorganized to consolidate supported calculations and elevate guidance for averages, percentages, and ratios.

  https://learn.microsoft.com/en-us/industry/sustainability/microsoft-sustainability-manager/calculate-reporting-metrics

- **Export data from Microsoft Sustainability Manager (preview)**

  Added a caution that exports with 200,000+ rows can create large files that quickly increase Dataverse storage usage and costs. Recommends establishing data retention or deletion policies before enabling organization-wide exports, with links to relevant guidance.

  https://learn.microsoft.com/en-us/industry/sustainability/sustainability-manager-data-export