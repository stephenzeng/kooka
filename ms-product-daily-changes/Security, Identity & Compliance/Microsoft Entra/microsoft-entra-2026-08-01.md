# Microsoft Entra
**Date created:** 2026-08-01 UTC  
**Tags:** Administration, Governance, Monitoring, Security  

## New Articles

- **Create configuration snapshots**

  Introduces end-to-end guidance for capturing configuration snapshots in Microsoft Entra Tenant Governance. Explains prerequisites, how to create a snapshot, and how to monitor asynchronous status until completion. Details how to view snapshot contents, download the baseline JSON, and use a completed snapshot to create a configuration monitor, including baseline cleanup. Includes links to configuration management concepts, Graph resources, permissions setup, and monitor creation.

  https://learn.microsoft.com/en-us/entra/id-governance/tenant-governance/how-to-create-snapshots

- **Global Secure Access and Microsoft Defender for Cloud Apps coexistence**

  Provides comprehensive guidance to run Microsoft Entra Internet Access (Global Secure Access) alongside Microsoft Defender for Cloud Apps without double-proxying. Compares overlapping capabilities across discovery, DLP, blocking, threat protection, and session controls, with clear division-of-responsibility recommendations. Includes step-by-step configuration (for example, bypass rules for *.mcas.ms), platform-specific discovery requirements, and integrations with Purview and Netskope to avoid conflicts. Offers practical design choices for session control using Conditional Access App Control versus forward proxy policies.

  https://learn.microsoft.com/en-us/entra/global-secure-access/reference-microsoft-defender-cloud-apps-coexistence

- **Microsoft Entra tenants for business partner access guidance**

  Introduces a tenant architecture pattern that isolates business partner access to reduce risk and decouple change control. Covers user lifecycle options (cross-tenant sync, entitlement management, self-service sign-up), credential and Conditional Access considerations, and structured collaboration with Teams and SharePoint. Addresses risk reduction (blast radius, governed external collaboration), regulatory scoping, and licensing tradeoffs, with references to related guidance in the tenant estate series.

  https://learn.microsoft.com/en-us/entra/architecture/tenant-estate-business-partner

- **Microsoft Entra collaborating production tenants guidance**

  Adds guidance for multitenant organizations operating multiple production tenants as one enterprise. Describes cross-tenant synchronization topologies, administration and governance across tenant boundaries, and alignment of credentials and Conditional Access (including MFA and device trust). Explains collaboration experiences across Microsoft 365, role-based access with entitlement management, and risk controls like access reviews and regulatory/data residency considerations. Includes an acquisition scenario, on-premises access patterns for MTO users, and links to related tenant estate articles.

  https://learn.microsoft.com/en-us/entra/architecture/tenant-estate-collaborating

- **Microsoft Entra tenants for critical business systems guidance**

  Outlines a separate tenant pattern for mission‑critical workloads to minimize blast radius and meet strict compliance requirements. Details administration, change control, account lifecycle governance, and strong credential policies including phishing‑resistant authentication. Recommends collaboration restrictions, role-based assignment via entitlement management and administrative units, and risk management measures. Summarizes operational overhead and licensing tradeoffs with links to related patterns.

  https://learn.microsoft.com/en-us/entra/architecture/tenant-estate-critical-production

- **Microsoft Entra tenant estate guidance introduction**

  Introduces a framework for composing a tenant estate with minimal tenant count while meeting security, compliance, and operational needs. Defines core patterns (primary production, collaborating production, isolated critical systems, business partner access, nonproduction) and seven evaluation areas such as administration, change control, lifecycle, credentials, collaboration, role-based assignment, and risk. Provides decision guidance for integrating apps and workloads, tenant lifecycle governance using Tenant Governance, and multitenant administration options. Clarifies workforce versus external user capabilities and B2B limitations across Microsoft services, with links to deep-dive articles.

  https://learn.microsoft.com/en-us/entra/architecture/tenant-estate-guide

- **Microsoft Entra hybrid identity and isolation multitenant guide**

  Explains how hybrid identity increases attack surface in multitenant scenarios and how to mitigate it. Recommends segmenting AD forests and synchronization boundaries per tenant, preventing overlapping identities, aligning device management, and enforcing least privilege on-prem. Aligns cloud isolation with on-prem infrastructure separation and links to the broader tenant estate series for end-to-end architecture guidance.

  https://learn.microsoft.com/en-us/entra/architecture/tenant-estate-hybrid-identity

- **Microsoft Entra nonproduction environments multitenant guidance**

  Details how to use separate tenants for nonproduction scenarios such as change validation, BCDR testing, and development. Provides an example architecture and guidance across administration, change control using configuration management, account lifecycle options (local, B2B, cross-tenant sync), and credential/device trust alignment. Covers collaboration constraints, role-based access, and risk management, including blast radius and regulatory considerations, with links to the tenant estate series.

  https://learn.microsoft.com/en-us/entra/architecture/tenant-estate-nonproduction

- **Microsoft Entra primary production tenant guidance**

  Establishes baseline architecture guidance for a primary production tenant. Covers delegated administration (built-in/custom roles, Azure RBAC, service roles, administrative units), use of PIM, and configuration baselines across services. Highlights high‑stakes change control with examples and recommends validation in nonproduction. Addresses workforce and guest lifecycle, passwordless and MFA enforcement, collaboration benefits, role-based access with entitlement management, and risk/regulatory considerations including data residency and IAM standards.

  https://learn.microsoft.com/en-us/entra/architecture/tenant-estate-primary

## Major Changes

- **Create a governed workforce tenant**

  Expanded and clarified prerequisites and audience scope for governed workforce tenant creation. Restricts eligibility to paid customers, clarifies that both EA and Pay-As-You-Go subscriptions and both MOSA and MCA billing accounts are supported, and outlines required roles (Tenant Creator when creation is restricted and Subscription Owner/Creator or Tenant Contributor for ARM). Provides clearer guidance to ensure admins have the right permissions and templates in place before provisioning, reducing setup failures and policy drift.

  https://learn.microsoft.com/en-us/entra/id-governance/tenant-governance/how-to-create-tenant

- **View monitor results and manage monitors**

  Significantly expands guidance for viewing and managing configuration monitors. Adds clear navigation, prerequisites, and detailed instructions for reviewing definitions, run history, drifts, baselines, permissions readiness, settings, and audit logs. Clarifies that remediation happens in the owning admin experiences and that later runs validate resolution, helping teams operationalize continuous configuration governance.

  https://learn.microsoft.com/en-us/entra/id-governance/tenant-governance/how-to-see-monitor-results

- **Configure configuration management service permissions**

  Overhauls instructions to center on the Configuration management permissions page, with workload-specific workflows for Graph (Entra ID/Intune), Teams, Exchange, Defender, and Purview. Clarifies least-privilege app-only permissions, where RBAC must be configured via PowerShell, and that wizard steps are read-only indicators of readiness. Simplifies permission removal steps and updates references, making it easier to provision the exact rights required for snapshots and monitors.

  https://learn.microsoft.com/en-us/entra/id-governance/tenant-governance/how-to-set-up-permissions-tenant-monitoring

- **Road to the cloud: Introduction**

  Rewrites the introduction to focus on modernizing identity, access, and device management with Microsoft Entra ID while minimizing reliance on on-premises Active Directory. Introduces “The AD minimization journey” with five clear stages and focus areas across users, applications, and devices. Helps organizations plan pragmatic steps from hybrid to cloud-only models while maintaining security and operational continuity.

  https://learn.microsoft.com/en-us/entra/architecture/road-to-the-cloud-introduction

## Moderate Changes

- **Quickstart - Access and create new tenant**

  Updated prerequisites to support EA and Pay-As-You-Go subscriptions and both MOSA and MCA billing accounts. Clarifies required Azure Resource Manager permissions (Tenant Contributor or Subscription Owner/Creator) and links to identify billing account type. These changes broaden eligibility and reduce setup friction for tenant creation.

  https://learn.microsoft.com/en-us/entra/fundamentals/create-new-tenant

- **Tutorial - Customize user provisioning attribute-mappings for SaaS applications in Microsoft Entra ID**

  Added a new mapping type where attribute values are generated by an Azure Logic App invoked via Lifecycle Workflows. Clarifies that attributes using this LCW extensibility workflow cannot serve as matching attributes. This expands extensibility while preventing configuration conflicts in matching logic.

  https://learn.microsoft.com/en-us/entra/identity/app-provisioning/customize-application-attributes

- **Deploy Microsoft Entra Tenant Governance end to end**

  Updated setup guidance to include EA and Pay-As-You-Go subscriptions and both MOSA and MCA billing accounts. Clarifies required permissions (Subscription Owner/Creator or Tenant Contributor) and aligns steps to those requirements, enabling smoother provisioning and compliance with least-privilege practices.

  https://learn.microsoft.com/en-us/entra/id-governance/tenant-governance/deployment-guide

- **Create a configuration monitor**

  Refocuses content on creating monitors with a clearer prerequisites section and a streamlined creation flow. Consolidates steps for naming, composing baselines (including upload/import with inline edits), and reviewing service permissions, and explains scheduling and where to view results. Removes outdated update guidance and links to Graph resources and related articles for ongoing operations.

  https://learn.microsoft.com/en-us/entra/id-governance/tenant-governance/how-to-create-monitor

- **Manage unsponsored guests using Lifecycle Workflows (Preview)**

  Adds an important note that managing unsponsored guests via Lifecycle Workflows is governed by the guest billing model. This helps admins plan licensing and cost implications before automating guest cleanup.

  https://learn.microsoft.com/en-us/entra/id-governance/how-to-lifecycle-workflow-unsponsored-guest-removal