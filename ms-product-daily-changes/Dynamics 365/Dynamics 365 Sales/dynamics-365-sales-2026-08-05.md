# Dynamics 365 Sales
**Date created:** 2026-08-05 UTC  
**Tags:** Administration, AI, Agent  

## New Articles

- **Business functions overview**

  Introduced Business Function Builder (preview) for Sales Research Agent and explained how business functions are generated from your environment’s schema and descriptions. Outlined the end-to-end workflow to review, validate, and share reusable functions. Provided best practices for scoping, defining metrics and acronyms, adding data instructions for custom data, and validating after changes. Included related links to creation, sharing, troubleshooting, usage, data connection, and context enhancement.

  https://learn.microsoft.com/en-us/dynamics365/sales/sales-research-agent-business-function-builder

- **Create business functions with Business Function Builder (preview)**

  Added a step-by-step guide to create business functions using natural language intent and reference content, then refine them with discovered anchor tables and clarifying questions. Described generating and editing the draft (role, business context, data instructions, glossary, and table/column hints), saving, and validating with built-in evaluations. Included guidance for handling custom tables, understanding schema, and applying best practices to improve function quality.

  https://learn.microsoft.com/en-us/dynamics365/sales/sales-research-agent-business-function-builder-create

- **Share business functions (preview)**

  Documented how to share business functions with teams, security roles, or business units from the Business functions list. Provided instructions to manage shared content, including updating, revalidating after changes, and revoking access as needed. Helps admins govern distribution so the right users can reliably use approved functions.

  https://learn.microsoft.com/en-us/dynamics365/sales/sales-research-agent-business-function-builder-share

- **Troubleshoot business functions (preview)**

  Added troubleshooting guidance for common issues in Business Function Builder, including routing when functions are missing across environments and prerequisites for draft generation. Covered recovery steps for long-running evaluation or discovery failures (refresh, re-authenticate, retry). Clarified engagement analysis and how to use data instructions for activity data so results are interpreted correctly.

  https://learn.microsoft.com/en-us/dynamics365/sales/sales-research-agent-business-function-builder-troubleshoot

## Major Changes

- **Provide context to enhance the Sales Research Agent**

  Replaced detailed procedural steps for building context with a streamlined, schema-aware approach centered on Business Function Builder to create, validate, and share reusable business functions. This change removes redundant examples and tightly couples guidance to your environment’s data model. The updated guidance is easier to follow, promotes consistency, and accelerates setup by focusing on reusable configurations.

  https://learn.microsoft.com/en-us/dynamics365/sales/sales-research-agent-provide-context

## Moderate Changes

- **Copilot Studio agents and app registrations for sales agents**

  Clarified when skill-based agents are provisioned for Dynamics 365 Sales and noted that some are shared across multiple sales agents, affecting provisioning counts. Updated the example and math to reflect tenant-level behavior, helping admins accurately estimate app registrations.

  https://learn.microsoft.com/en-us/dynamics365/sales/ai-agents-apps

- **Import an agent into a target environment**

  Replaced an embedded table of required agents with a link to centralized, up-to-date guidance for which agents to add by type. This reduces duplication and helps users rely on a single source of truth.

  https://learn.microsoft.com/en-us/dynamics365/sales/import-export-agent-solutions