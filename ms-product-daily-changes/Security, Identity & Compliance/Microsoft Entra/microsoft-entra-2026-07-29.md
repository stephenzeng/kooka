# Microsoft Entra
**Date created:** 2026-07-29 UTC  
**Tags:** Administration, Automation, Governance, Monitoring, Security  

## New Articles

- **Manage unsponsored guests using Lifecycle Workflows (Preview)**

  Introduced a new how-to guide for removing unsponsored guest users with Microsoft Entra ID Governance Lifecycle Workflows. Explains how to use the built-in Unsponsored guest cleanup (Preview) template, including the non-configurable trigger based on sponsor count and steps to create, configure tasks, and enable the workflow. Highlights the default Delete User Account task and an optional notification task to email stakeholders about removals. Helps admins operationalize guest lifecycle governance with clear, step-by-step guidance.

  https://learn.microsoft.com/en-us/entra/id-governance/how-to-lifecycle-workflow-unsponsored-guest-removal

## Major Changes

- **Lifecycle Workflow built-in tasks**

  Removed the Preview label from the Update user attributes task and clarified that for users synced from on-premises AD, only directory extension attributes are supported. Updated Microsoft Graph parameter examples to reflect the new display name. Added a new task, Send email about unsponsored guest removal (Preview), including prerequisites, availability for leaver workflows, supported parameters, recipient options, and a full example payload. These updates expand automation options for guest lifecycle management and clarify attribute update constraints for hybrid environments.

  https://learn.microsoft.com/en-us/entra/id-governance/lifecycle-workflow-tasks

## Moderate Changes

- **Automatic formation of governance relationships**

  Removed preview labels and notes to reflect general availability. Content remains the same, signaling that the capability is supported for production use.

  https://learn.microsoft.com/en-us/entra/id-governance/tenant-governance/automatic-governance-relationships

- **Cross-tenant delegated administration**

  Updated the article to remove the preview designation and note. Guidance is now positioned for production use without content changes.

  https://learn.microsoft.com/en-us/entra/id-governance/tenant-governance/cross-tenant-delegated-administration

- **Governance relationships in Tenant Governance**

  Removed preview indicators and notes, reflecting GA status. The guidance is unchanged but now represents supported, production-ready functionality.

  https://learn.microsoft.com/en-us/entra/id-governance/tenant-governance/governance-relationships

- **Install the Microsoft Entra Connect Health agents**

  Clarified that installing with the Hybrid Identity Administrator role is supported only in the Azure public cloud, not sovereign clouds. This helps admins plan deployments appropriately for Azure Government and similar environments.

  https://learn.microsoft.com/en-us/entra/identity/hybrid/connect/how-to-connect-health-agent-install

- **Create a governed workforce tenant**

  Removed preview labels and notes to mark the feature as generally available. The procedures are unchanged, indicating readiness for production rollout.

  https://learn.microsoft.com/en-us/entra/id-governance/tenant-governance/how-to-create-tenant

- **Use cross-tenant delegated administration**

  Eliminated preview status from the title and page notes. Guidance remains the same and is now aligned with GA support.

  https://learn.microsoft.com/en-us/entra/id-governance/tenant-governance/how-to-delegated-administration

- **Enable tenant discovery**

  Removed preview indicators and the preview note to reflect GA. No procedural changes; the feature can be adopted for standard operations.

  https://learn.microsoft.com/en-us/entra/id-governance/tenant-governance/how-to-enable-tenant-discovery

- **Interpret tenant discovery data**

  Updated the article to remove preview status and the associated note. The content is unchanged but now suitable for production environments.

  https://learn.microsoft.com/en-us/entra/id-governance/tenant-governance/how-to-interpret-discovery-data

- **Monitor governing tenant admin activity in a governed tenant**

  Removed preview labels and notes, indicating GA availability. Monitoring guidance is unchanged but now officially supported.

  https://learn.microsoft.com/en-us/entra/id-governance/tenant-governance/how-to-monitor-governing-activity

- **See monitor results and configuration drifts**

  Removed preview markers and the preview note to signal GA. Content remains the same to support production monitoring scenarios.

  https://learn.microsoft.com/en-us/entra/id-governance/tenant-governance/how-to-see-monitor-results

- **Set up a governance relationship**

  Transitioned the article from preview to GA by removing labels and the preview note. Core setup guidance is unchanged and ready for production use.

  https://learn.microsoft.com/en-us/entra/id-governance/tenant-governance/how-to-set-up-governance-relationship

- **Update a governance relationship**

  Removed preview status from the title and page notes, reflecting GA. Procedures are unchanged, enabling production adoption.

  https://learn.microsoft.com/en-us/entra/id-governance/tenant-governance/how-to-update-governance-relationship

- **What is Microsoft Entra Tenant Governance?**

  Removed preview indicators and outdated text that suggested most experiences were in preview, aligning the page with GA status. This clarifies service readiness while retaining information about service levels.

  https://learn.microsoft.com/en-us/entra/id-governance/tenant-governance/overview

- **Related tenants in Tenant Governance**

  Removed preview status and the preview note to mark GA. Content remains consistent, indicating production support.

  https://learn.microsoft.com/en-us/entra/id-governance/tenant-governance/related-tenants

- **Signals and metrics for tenant discovery**

  Removed preview labels and the preview note, reflecting GA. No content changes; metrics guidance is stable for production use.

  https://learn.microsoft.com/en-us/entra/id-governance/tenant-governance/signals-metrics