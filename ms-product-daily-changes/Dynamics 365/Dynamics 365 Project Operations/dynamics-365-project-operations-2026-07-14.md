# Dynamics 365 Project Operations
**Date created:** 2026-07-14 UTC  
**Tags:** Administration  

## New Articles

- **Time Entry Configurations**

  Introduced a how-to article detailing time entry governance in Project Operations. It explains how admins can cap daily time entry with Max Daily Duration (0–1,440 minutes) and how enforcement works on create and update, with 1,440 minutes as the default if unset. It also clarifies time zone behavior options for time entry grids, allowing a choice between time zone aware and time zone independent modes, with guided steps to configure these under Settings > Parameters > Organization Units > Time Entry Configuration.

  https://learn.microsoft.com/en-us/dynamics365/project-operations/time/time-entry-configurations

## Major Changes

- **Resource reconciliation overview**

  Added a preview Bulk Resource Reconciliation UI to reconcile booking shortages and excesses across multiple resources and time slices in one action. The update includes how to enable the preview in Settings > Parameters, workflows for reconciling selected slices or running Reconcile All at the project level, and behavior notes for notifications and skipped already-reconciled slices. It clarifies that the UI uses the same business logic as the Bulk Reconciliation API and adds a dedicated section to organize project-level reconciliation guidance.

  https://learn.microsoft.com/en-us/dynamics365/project-operations/resource-management/resource-reconciliation-overview

## Moderate Changes

- **Reconcile projects with Bulk Reconciliation**

  Updated guidance to remove references to limited reconciliation support and point users to the new Bulk Resource Reconciliation UI (preview) as an alternative to the custom action. This helps administrators choose a more scalable, UI-driven approach where appropriate.

  https://learn.microsoft.com/en-us/dynamics365/project-operations/resource-management/bulk-reconciliation-dev

- **Enhanced Team Member experience (Preview)**

  Revamped terminology and navigation from staffed projects to booked capacity, updating paths from Projects to Bookings under My Work and aligning configuration with My Bookings in the Bookable Resource Booking table. Added time-phased views for bookings and task assignments with daily/weekly/monthly horizons and streamlined instructions for tracking work.

  https://learn.microsoft.com/en-us/dynamics365/project-operations/time/enhanced-team-member-experience