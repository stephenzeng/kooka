# Power Platform
**Date created:** 2026-09-05 UTC  
**Tags:** Automation, Best Practices, Configuration, Deprecation, Guidance, Troubleshooting  

## New Articles

- **COSMO CONSULT improves sales operations and data quality using Copilot Studio agents**

  Introduced a new case study detailing how four Copilot Studio agents integrate with Dynamics 365, Dataverse, Teams, and Power Apps to improve sales operations and data quality. The article outlines business challenges, architecture, and workflows for Data Health Assistant, Text2Lead, Lead Recorder, Fund Eligibility Checker, and Expense Mapping agents. It highlights implementation approaches using topics, agent flows, Dataverse, Azure Speech, AI Builder, and Power Automate, along with measurable impact and key takeaways.

  https://learn.microsoft.com/en-us/power-platform/guidance/case-studies/cosmo-consult-improves-sales-operations

## Moderate Changes

- **Manage administration mode in a unified developer environment**

  Expanded guidance beyond package deployment to broader administration mode management for OnlineDev/UDE environments. Added instructions for reviewing failures in environment history and obtaining detailed logs via the Finance and Operation Package Manager App. Clarified that deployments in administration mode are code-only (no DB sync) for OnlineDev/UDE and provided recovery steps for environments stuck in administration mode.

  https://learn.microsoft.com/en-us/power-platform/developer/unified-experience/finance-operations-deploy-admin-mode

- **Important changes (deprecations) coming in Power Platform**

  Added a deprecation notice for the Power Virtual Agents help chatbot in the Power Automate maker portal, scheduled for removal on September 9, 2026, with no impact on flows or connectors and no admin action required beyond user communications. Clarified the Power Automate mobile app deprecation by updating impact details and removing outdated notes about the “Send me a mobile notification” action.

  https://learn.microsoft.com/en-us/power-platform/important-changes-coming

- **Real-world case studies**

  Updated the case studies index with a new entry on COSMO CONSULT’s use of Copilot Studio agents, including a link and description. This addition broadens available examples for practitioners evaluating similar solutions.

  https://learn.microsoft.com/en-us/power-platform/guidance/case-studies/

- **Power Platform and Dynamics 365 macro region geography**

  Clarified environment placement by adding product availability as a factor alongside capacity and performance. Updated capability bullets, the example workflow, and the FAQ to reflect an algorithm that considers capacity and product availability when selecting a datacenter region.

  https://learn.microsoft.com/en-us/power-platform/admin/macro-regions

- **Tenant-to-tenant migrations**

  Added a tip to validate your approach by copying production to a sandbox and migrating the sandbox first. Introduced a warning to assign the System Administrator role post-migration due to non-migrated security groups, clarifying that an empty environment view indicates a permissions issue. Expanded the FAQ to note migrations can take up to 24 hours and that slow progress does not imply failure.

  https://learn.microsoft.com/en-us/power-platform/admin/move-environment-tenant