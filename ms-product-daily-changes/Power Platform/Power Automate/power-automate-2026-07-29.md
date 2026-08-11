# Power Automate
**Date created:** 2026-07-29 UTC  
**Tags:** Administration, Automation, Monitoring, Other, Security  

## Major Changes

- **Operator role for Power Automate**

  Expanded guidance explains the Operator role’s monitoring scope and constraints, including that operators can’t view action-level inputs/outputs, expression results, trigger payloads, or resubmit/cancel runs. Clarifies which run metadata is accessible via the Dataverse FlowRun table for solution-aware cloud flows and notes that non-solution flows aren’t covered, while desktop flow monitoring remains fully detailed. Adds workarounds such as sharing flows (co-owner/run-only) and using the Power Automate Management connector to export action-level details, plus related links for deeper guidance.

  https://learn.microsoft.com/en-us/power-automate/operator-role

- **Power Automate mobile app (deprecated)**

  Reframed the article to announce deprecation of the mobile app and provide alternatives for common tasks, such as using the Teams Approvals app, the Power Automate portal via mobile browser, and Power Apps mobile for running instant flows. Confirms existing automated, scheduled, and instant flows continue to run, and outlines limitations of alternatives (no direct home-screen widget, add Teams/email notifications with Run after on failure, designer not optimized for small screens). Removes prior installation and environment-switching instructions to avoid outdated guidance.

  https://learn.microsoft.com/en-us/power-automate/mobile/overview-mobile

## Moderate Changes

- **Create flows from your phone**

  Added a deprecation notice at the top to reflect changes to the mobile experience. No other substantive updates were made.

  https://learn.microsoft.com/en-us/power-automate/mobile/mobile-create-flow

- **Create widgets for flows**

  Inserted a deprecation notice to inform readers about changes in mobile support. No other meaningful content changes.

  https://learn.microsoft.com/en-us/power-automate/mobile/widgets

- **Manage approvals**

  Updated the page with a deprecation notice for the Power Automate mobile app to set expectations about mobile availability. No functional guidance was modified.

  https://learn.microsoft.com/en-us/power-automate/mobile/manage-approvals

- **Manage cloud flows**

  Added a deprecation notice for the mobile app immediately after the title to communicate support changes. Other content remains unchanged aside from metadata.

  https://learn.microsoft.com/en-us/power-automate/mobile/manage-cloud-flows

- **Overview of cloud flows**

  Removed the section about creating and using cloud flows from a phone, including app installation guidance and links. This streamlines the overview to align with the mobile app deprecation.

  https://learn.microsoft.com/en-us/power-automate/overview-cloud

- **Receive notifications**

  Added a deprecation notice for the mobile app and removed steps for viewing notifications from a different environment. Core notification guidance was otherwise retained.

  https://learn.microsoft.com/en-us/power-automate/mobile/notifications