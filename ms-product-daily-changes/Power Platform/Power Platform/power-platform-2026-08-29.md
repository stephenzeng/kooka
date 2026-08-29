# Power Platform
**Date created:** 2026-08-29 UTC  
**Tags:** Compliance, Configuration, Guidance, Governance, Identity, Security, Troubleshooting  

## New Articles

- **Deploy packages to a unified developer environment in administration mode**

  Introduced a how-to that enables deploying code-only packages to OnlineDev/Unified Developer environments while the environment is in administration mode. This flow skips database sync to help recover environments blocked by package or schema issues. The article clarifies scope (OnlineDev/UDE only) and provides step-by-step actions to deploy the fix and then exit administration mode. It also links to related admin mode guidance and X++ development workflows.

  https://learn.microsoft.com/en-us/power-platform/developer/unified-experience/finance-operations-deploy-admin-mode

## Moderate Changes

- **Administration mode**

  Clarified that package deployment is permitted in OnlineDev unified developer environments for finance and operations apps while the environment is in administration mode, with a link to step-by-step instructions. This helps administrators apply code-only fixes without leaving admin mode.

  https://learn.microsoft.com/en-us/power-platform/admin/admin-mode

- **Control user access to environments with security groups and licenses**

  Updated guidance to map least-privileged admin roles to key tasks and clarified options for managing nested security groups, with an example scenario. Clarified licensing behavior so only eligible licensed users in the environment’s security group are created, and reiterated that security groups cannot be set on default or developer environments; also refined procedures and added related Microsoft Entra group management content.

  https://learn.microsoft.com/en-us/power-platform/admin/control-user-access

- **Power Platform environments overview**

  Clarified that Preferred environment location applies to macro regions only when Advanced Data Residency for Microsoft 365 is enabled. Elevated this as an IMPORTANT callout and linked to macro region geography documentation to guide deployment planning.

  https://learn.microsoft.com/en-us/power-platform/admin/environments-overview

- **Workflow to write, deploy, debug, and troubleshoot X++ code across multiple environments**

  Added guidance on deploying code-only packages while in administration mode to bypass DB sync and expedite fixes. Included a cross-reference to the dedicated admin-mode deployment article and expanded related resources to streamline recovery workflows.

  https://learn.microsoft.com/en-us/power-platform/developer/unified-experience/finance-operations-innerloop