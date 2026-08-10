# Dynamics 365 Contact Center
**Date created:** 2026-07-12 UTC  
**Tags:** AI, Administration, Analytics, Automation  

## New Articles

- **Manage schedules in Workforce Management**

  Introduced a comprehensive guide to the Schedule Workforce page, detailing the interactive schedule board and how to view, filter, and adjust schedules. Explains assignment views, adding representatives to shift plans, and publishing schedules in segments up to six weeks. Covers editing and deleting bookings, scheduling ad-hoc activities, and how changes affect publishing states to improve day-to-day scheduling efficiency.

  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/workforce-management-schedule-workforce

- **Create and manage shift rotation policies**

  Added end-to-end guidance for creating, assigning, and maintaining shift rotation policies, including prerequisites, cadence setup, time slots, and representative assignments. Clarifies operational behavior such as pause/resume effects, when changes take effect, and safeguards when policies are linked to shift plans. Highlights key constraints (one policy per shift plan, one policy per representative) to ensure predictable, fair rotation and simpler scheduling governance.

  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/workforce-management-shift-rotation-policies

## Major Changes

- **Create and schedule a shift plan**

  Streamlined the article by removing detailed scheduling steps and consolidating that guidance into a centralized Schedule Workforce article. The shift plan creation content remains, while procedures for adding/editing/deleting bookings and publishing schedules now redirect to the new, dedicated page. This reduces duplication and helps users find all scheduling operations in one place for a clearer workflow.

  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/workforce-management-shift-plan

## Moderate Changes

- **Manage quality evaluation**

  Added the ability for evaluators to regenerate evaluation summaries and action plans, with automatic regeneration on submission when answers change and skipped generation when no changes occur for efficiency. Included admin controls to enable or disable the option, which affects availability of manual and post-completion generation for AI-assisted and AI agent evaluations.

  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/manage-quality-evaluation-agent

- **Use evaluations**

  Updated end-user guidance to support regenerating evaluation summaries, including a Regenerate summary option, status visibility, and timestamps; summaries auto-generate on submission when responses change. Also reorganized evaluation states content and clarified steps in viewing and editing evaluations to streamline the workflow.

  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/use-evaluations

- **Configure shift activity types**

  Introduced new fields to classify activities (Work Type and optional Meal/Break Subtype) and added adherence tracking with presence-state monitoring and configurable tolerance. Clarified that only Meal/Break subtypes are eligible for break distribution in auto-schedule to ensure accurate scheduling rules.

  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/workforce-management-shift-activity-types

- **Schedule representatives with auto-schedule**

  Added configuration for break distribution with clear rules for spacing and timing, and documented validation requirements so only eligible activity types are scheduled. Described post-generation acceptance or rejection workflows and refined steps and labels to make auto-scheduling easier to configure and review.

  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/workforce-management-use-auto-schedule