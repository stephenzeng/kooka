# Dynamics 365 Field Service
**Date created:** 2026-07-21 UTC  
**Tags:** Administration, Other  

## New Articles

- **Projects, project contracts, and project tasks**

  Introduced foundational guidance that explains how project contracts, contract lines, projects, and project tasks relate in the Field Service and Project Operations integration. Clarifies eligibility rules for linking work orders and agreements to projects, including order type, billing method, customer and legal entity alignment, supported transaction classes, and valid project dates. Details the contract line fields that impact Field Service transactions and how they drive pricing and posting behavior. Outlines Field Service’s minimal project management capabilities and directs advanced planning and scheduling to Project Operations.

  https://learn.microsoft.com/en-us/dynamics365/field-service/project-operations-integration-projects

- **Set up projects with work orders in the Field Service and Project Operations integration**

  Added scenario-based setup guidance covering six common patterns, from single-project, multi–work order models to agreement-driven schedules and task-based billing. Provides recommended contract line configurations, including Include Time/Material/Expense/Fee settings, billing methods, and how transactions resolve to the correct project, task, and contract line. Helps readers choose the right setup for separate billing streams (labor vs. materials) and for fixed-price projects where Field Service costs post as cost-only actuals.

  https://learn.microsoft.com/en-us/dynamics365/field-service/project-operations-integration-scenarios

- **Time entry flow between Field Service and Project Operations**

  Describes how time captured in Field Service is priced and approved in Project Operations, with approval status syncing back. Explains prerequisites for approvals, and that only approved time drives financial actuals and updates project task progress. Clarifies that role-based pricing and exchange rates are handled in Project Operations, and that Field Service does not perform pricing. Provides guidance on using the Modern Time Entry Grid and how labor estimates are created, surfaced, and transferred.

  https://learn.microsoft.com/en-us/dynamics365/field-service/project-operations-integration-time

- **Schedule work orders linked to projects and project tasks**

  Provides step-by-step instructions to schedule work orders tied to projects and tasks, including prerequisites, adding Project and Project Task columns, and using the Project tab on the schedule board. Explains auto-updating Time Promised windows from task planned dates and shows warnings when scheduling conflicts with date ranges, dependencies, or predecessor completion. Covers how to review task dependencies before scheduling and notes key mobile behaviors.

  https://learn.microsoft.com/en-us/dynamics365/field-service/project-operations-integration-work-order-schedule

## Major Changes

- **What's new in the Field Service integration with Project Operations**

  Added a July 31, 2026 release section highlighting task-level work order association for creation, linking, reassignment, and contextual visibility from project tasks. Introduced project-driven scheduling where planned task dates inform advisory Time Promised windows and warn when bookings fall outside expected ranges. Surfaced project task dependencies on work orders to visualize sequencing. Expanded time entry integration to flow approvals and pricing into Project Operations, generate cost and unbilled sales actuals, and update task effort completed when tied to a task.

  https://learn.microsoft.com/en-us/dynamics365/field-service/project-operations-whats-new

## Moderate Changes

- **Field Service integration with Project Operations overview**

  Expanded the overview to emphasize out-of-the-box connectivity and end-to-end data flows across work orders, tasks, labor, materials, and financials. Added clear guidance on technician time entry flowing to Project Operations with pricing and approvals, and strengthened explanations of material usage processing and the financial pipeline.

  https://learn.microsoft.com/en-us/dynamics365/field-service/project-operations-integration

- **Known issues and limitations**

  Documented additional unsupported scenarios and operational constraints, such as fees not flowing, agreement-to-task linking not supported, task management in Project Operations, and limits around discount handling and mobile offline behavior. Retained prior limitations with clarifications and made minor wording updates to Known issues without changing functionality.

  https://learn.microsoft.com/en-us/dynamics365/field-service/project-operations-integration-issues

- **Manage projects in Field Service**

  Streamlined the article by removing embedded requirements and linking to centralized guidance for project contracts, tasks, and field impacts on transactions. Updated creation steps for projects and contract lines to point readers to those requirements for correct linkage and processing.

  https://learn.microsoft.com/en-us/dynamics365/field-service/project-operations-integration-manage-projects

- **Set up Field Service integration with Project Operations**

  Clarified that the integration package includes a recurring Power Automate flow that runs under the installing user, and advised verifying the appropriate license. Added references to license types and the Power Automate licensing FAQ to ensure compliant deployment.

  https://learn.microsoft.com/en-us/dynamics365/field-service/project-operations-integration-setup

- **Link projects to work orders and agreements**

  Clarified when a linked project can be changed or removed, limiting changes to unposted work orders without associated project tasks. Enabled selecting a project task when the user is assigned to it and locked fields when both project and task are set to preserve financial consistency and task alignment.

  https://learn.microsoft.com/en-us/dynamics365/field-service/project-operations-integration-work-order