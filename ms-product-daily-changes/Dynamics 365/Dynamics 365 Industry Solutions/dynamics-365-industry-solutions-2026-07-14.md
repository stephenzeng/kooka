# Dynamics 365 Industry Solutions
**Date created:** 2026-07-14 UTC  
**Tags:** Administration, Analytics, Governance  

## New Articles

- **Export data from Microsoft Sustainability Manager (preview)**
  
  Introduced a preview Data exports capability that lets admins generate Excel exports based on a selected data definition and date range. The article explains how to enable the feature per environment, the required privileges, and how to surface it in the sitemap. It provides step-by-step guidance to create and monitor export jobs, interpret status and job fields, and download results when complete. It also outlines key limitations, including backend-owned processing, read-only scope after submission, attachment retention behavior, and a single concurrent job constraint.
  
  https://learn.microsoft.com/en-us/industry/sustainability/sustainability-manager-data-export

- **What's new in Microsoft Sustainability Manager - July 2026**
  
  Summarizes new and enhanced capabilities including a preview data export to Excel, ownership changes for Power Query imports, reporting metrics and calculation framework improvements, and a new calculation data trail report replacing the deprecated report. Highlights operational enhancements like partial locking for reporting periods, bulk Excel uploads for Data Collection, and Goals page state retention, along with numerous reliability fixes across approvals, calculation/reporting, and imports. Lists current preview areas such as allocations, alternate standards, data trail, circularity dashboards, connectors, data approval/collection management, export, and waste quality.
  
  https://learn.microsoft.com/en-us/industry/sustainability/whats-new-2026-07

## Major Changes

- **Generate a calculation data trail report (preview)**
  
  Reworked the article to focus on a calculation-level data trail report tied to calculation profiles, replacing the prior, broader emissions data trail flow. Added prerequisites to enable the feature via an environment variable and a new Data trail (preview) toggle on calculation profiles, plus end-to-end steps to run a calculation, generate the report, track status, and download a CSV. Expanded scope covers input sources, calculation models/profiles, emissions outputs, gases, factors, and mappings, with guidance to compare runs by job ID and manage report versions. Removed the older approach centered on scope/date selection and generic activity/emissions attributes to better align with calculation governance and auditability.
  
  https://learn.microsoft.com/en-us/industry/sustainability/sustainability-manager-report-data-trail

## Moderate Changes

- **Supported versions**
  
  Updated the support policy to N-2 compliance as of April 2026, replacing the prior “four most recent versions” approach. Refreshed the versions table to add July 2026 (current 2.35.0, earliest supported 2.33.0), update April 2026 earliest supported to 2.33.0, and remove outdated February and January 2026 rows. This clarifies upgrade expectations and helps organizations plan version currency and support windows.
  
  https://learn.microsoft.com/en-us/industry/sustainability/deploy-supported-versions

- **Change data import connection ownership**
  
  Expanded guidance for transferring ownership of data import connections, covering supported import types (Power Query and data provider connectors) and explicitly excluding manual and Excel template imports. Added prerequisites for required roles and clarified post-transfer behavior: access must be reconnected with the new owner’s credentials, incremental refresh must be recreated after the first successful import, and the system sets status to Action required and disables Ready to import while preserving queries. Updated procedures detail the steps for Power Query imports and a dedicated flow for data provider connectors to reduce handover friction and prevent failures.
  
  https://learn.microsoft.com/en-us/industry/sustainability/sustainability-manager-import-data-connection-ownership

- **Troubleshoot data import**
  
  Added troubleshooting for import failures caused by missing data lake permissions when staging via Power Query. Instructs users to run Refresh permissions from the Data imports command bar to restore access, verify the refresh, and retry if the service is temporarily unavailable. This helps resolve common permission-related failures quickly.
  
  https://learn.microsoft.com/en-us/industry/sustainability/sustainability-manager-import-data-troubleshoot

- **Deprecations in Microsoft for Sustainability**
  
  Announced deprecation of the Data trail report (preview) and removal of its documentation. Advises organizations to adopt the new Generate a calculation data trail report capability, which offers calculation-level tracking and CSV exports with different specifications. This directs users to the supported replacement for ongoing audit and governance needs.
  
  https://learn.microsoft.com/en-us/industry/sustainability/whats-new-deprecations