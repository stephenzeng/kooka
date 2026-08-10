# Dynamics 365 Contact Center
**Date created:** 2026-07-18 UTC  
**Tags:** Administration, Analytics  

## Major Changes

- **Use evaluation criteria**

  Introduced a weighted scoring model with support for enabling question-level scoring via a new “Allow scoring for question” toggle. The guidance clarifies how to distribute weights across criteria, sections, and questions, including rules and validation for question weightage. It details scoring logic for different question types (yes/no, single-select, multi-select, and descriptive) and explains overall score calculation. It also covers scoring for extended parent/child criteria with clear weight distribution rules and final score formulas.

  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/evaluation-criteria

## Moderate Changes

- **Configure conversation orchestration in Dynamics 365 Contact Center (preview)**

  Added guidance for migrating conversation orchestration playbooks between environments using solutions. The new content covers prerequisites and dependencies, preparing the destination environment, export/import steps, handling missing dependencies, and post-import verification to reduce deployment errors.

  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/configure-conversation-orchestration

- **Deprecations in Dynamics 365 Contact Center**

  Added a deprecation notice for Apple Messages for Business: onboarding is deprecated as of July 17, 2026, and Apple configuration options will be removed from the Copilot Service admin center on September 30, 2026. Organizations should plan alternative channels and update configurations ahead of the removal date to avoid disruptions.

  https://learn.microsoft.com/en-us/dynamics365/contact-center/implement/deprecations-contact-center