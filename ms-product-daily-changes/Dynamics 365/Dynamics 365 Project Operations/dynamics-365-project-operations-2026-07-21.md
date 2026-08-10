# Dynamics 365 Project Operations
**Date created:** 2026-07-21 UTC  
**Tags:** Administration, Other  

## New Articles

- **Project Operations and Field Service integration overview**

  Introduced an overview of how Dynamics 365 Project Operations integrates with Field Service, detailing data flows for work orders, projects, tasks, labor, materials, time entries, and financial transactions. Highlights key benefits such as reducing manual reconciliation and improving end-to-end visibility across delivery and finance. Provides context for when and how data can flow into Dynamics 365 Finance and links to broader integration guidance.

  https://learn.microsoft.com/en-us/dynamics365/project-operations/field-service-integration/project-operations-integration-overview

- **Create a work order in Project Operations**

  Added a how-to guide for creating Field Service work orders directly from a project and associating existing work orders to that project. Includes prerequisites and required permissions for integrating Project Operations with Field Service, plus step-by-step instructions using the Related tab and quick create. Explains how project context (account, project, price list) is auto-populated and when the work order becomes available for scheduling in Field Service. Provides links to related tasks and next steps.

  https://learn.microsoft.com/en-us/dynamics365/project-operations/field-service-integration/project-operations-integration-po-work-order

- **Create a work order from a project task in Project Operations**

  Introduced guidance for creating a Field Service work order from a specific project task, with prerequisites and how planned task dates drive Time Promised dates on the work order. Covers associating existing work orders to tasks, and how to remove or reassign them, including constraints when draft time entries exist and warnings when actuals are present. Describes how scheduling and bookings work, how progress rolls up to the WBS, and how to view related work orders. Includes related links for scheduling and task-to-work order workflows.

  https://learn.microsoft.com/en-us/dynamics365/project-operations/field-service-integration/project-operations-integration-po-work-order-task

- **Project task and work order integration**

  Detailed how project tasks relate to Field Service work orders, including prerequisites such as using leaf-level WBS tasks. Clarified one-way synchronization of task dates to Time Promised Start/End on work orders, and how updates affect unscheduled versus scheduled work without changing existing bookings. Explained the difference between planning (assignments) and scheduling (bookings), how resource requirements are generated, and how time entries inherit project/task context and affect task effort and project actuals only after approval. Noted that work order financial summaries exclude those time entries, while actuals/estimates retain Field Service context for traceability, and described task-based billing via mapping tasks to contract lines.

  https://learn.microsoft.com/en-us/dynamics365/project-operations/field-service-integration/project-operations-integration-project-task