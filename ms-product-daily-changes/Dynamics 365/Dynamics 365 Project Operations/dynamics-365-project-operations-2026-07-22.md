# Dynamics 365 Project Operations
**Date created:** 2026-07-22 UTC  
**Tags:** Administration, Agent, Governance  

## New Articles

- **Set up project-level policy documents for the Approvals Agent (preview)**

  Introduced guidance for attaching Time, Expense, and Material policy documents at the project level so the Approvals Agent applies project-specific rules before org-wide policies, with automatic fallback when a project policy isn’t present. Provides prerequisites, step-by-step setup, and instructions to re-evaluate previously classified entries using Reassign to Agent. Clarifies required Dataverse permissions (Read/Create on Approval Classification Policy, included in the Project Manager role) and links to related setup and administration resources.

  https://learn.microsoft.com/en-us/dynamics365/project-operations/approvals/approvals-agent-project-policy

## Major Changes

- **Set up policy documents for the Approvals Agent (preview)**

  Marked the feature as a production-ready preview with supplemental terms and significantly expanded the policy data model. Added new columns (Example output and Conditions for inclusion) and clarified that not all data signals are always present, with explicit inclusion criteria. Introduced numerous signals (for example, subcontract line name, capacity/allocation checks, receipt requirements, product type and write-in description, additional dates, category fields, and budget validations for cost and sales). Refined explanations of how the agent ingests and uses data and streamlined example guidance to make policy configuration clearer and more reliable.

  https://learn.microsoft.com/en-us/dynamics365/project-operations/approvals/approvals-agent-policy

## Moderate Changes

- **Approvals Agent overview (preview)**

  Expanded policy management guidance to include project-level policy documents for Time, Expense, and Material, clarifying that project policies take precedence over org-wide policies. Documented behavior when policies are missing at either level to help ensure predictable classification outcomes.

  https://learn.microsoft.com/en-us/dynamics365/project-operations/approvals/approvals-agent-intro