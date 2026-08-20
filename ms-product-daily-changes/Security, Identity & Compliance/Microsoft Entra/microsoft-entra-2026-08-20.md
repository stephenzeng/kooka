# Microsoft Entra
**Date created:** 2026-08-20 UTC  
**Tags:** Automation, Configuration, Governance, Guidance  

## Major Changes

- **Delegate approvals and access reviews in My Access (Preview)**
  
  Expanded delegation from approvals-only to include multi-resource (catalog) access reviews, while clarifying that single-resource reviews aren’t eligible. Added admin controls to restrict who users can delegate to (for example, manager or specific groups) and to set duration limits, with updated setup and management steps in the Entra admin center. Clarified post-delegation routing, delegate capabilities, and limitations so admins can enforce governance while maintaining continuity. Included detailed instructions for creating, editing, and removing delegates, reflecting updated UI across Approvals and Access reviews pages.
  
  https://learn.microsoft.com/en-us/entra/id-governance/delegate-approvals-my-access

## Moderate Changes

- **Web filtering in Global Secure Access (V2)**
  
  Clarified that V2 web filtering rules don’t support user or group targeting and that scoping should be applied at the security profile level via Conditional Access. Updated migration and evaluation guidance: V2 uses a different model, has higher priority than V1, and evaluates only the first applicable profile, which can change enforcement when users match multiple profiles. Added best-practice guidance to consolidate intended outcomes into a single V2 policy with ordered rules and a default action, plus an FAQ on when to remain on V1 and how to revert by removing V2 policies.
  
  https://learn.microsoft.com/en-us/entra/global-secure-access/concept-web-filtering

- **Plan a Lifecycle Workflow deployment**
  
  Clarified that the “Remove all access package assignments for user” action is scheduled (not immediate) when daysUntilExpiration is set. Expanded applicability from Leaver to Leaver–Mover workflows to support more consistent deprovisioning plans.
  
  https://learn.microsoft.com/en-us/entra/id-governance/lifecycle-workflows-deployment

- **Lifecycle Workflow built-in tasks**
  
  Updated the “Remove all access package assignments for user” task to support mover scenarios with a default scheduled removal of 15 days and to mark daysUntilExpiration as required (with the mover default noted). Clarified that setting daysUntilExpiration schedules removal rather than performing it immediately, and aligned example JSON to reflect scheduled vs. immediate behavior.
  
  https://learn.microsoft.com/en-us/entra/id-governance/lifecycle-workflow-tasks

- **Lifecycle Workflows templates and categories**
  
  Refreshed template task lists to add or replace with “Remove all access package assignments for user,” using scheduled removal with a 15-day default across real-time employee change, employee group membership changes, and employee job profile change templates. This provides clearer default deprovisioning behavior and more predictable access removal during moves.
  
  https://learn.microsoft.com/en-us/entra/id-governance/lifecycle-workflow-templates

- **Automate employee mover tasks when they change jobs using the Microsoft Entra admin center**
  
  Added guidance to keep the default “Remove all access package assignments for user” task with a scheduled 15-day removal to preserve appropriate access during transitions. Clarified review steps to retain this task while configuring “Add user to groups” (for example, adding the user to the Sales group).
  
  https://learn.microsoft.com/en-us/entra/id-governance/tutorial-mover-custom-workflow-portal