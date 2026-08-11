# Microsoft Entra
**Date created:** 2026-07-30 UTC  
**Tags:** Administration, Analytics, Governance, Security  

## New Articles

- **Investigate related tenant signals by using Microsoft Graph (preview)**

  Introduces a step-by-step workflow to analyze Tenant Governance discovery signals with Microsoft Graph, helping admins validate and act on cross-tenant activity. Explains how to list related tenants, expand investigation hints for specific metrics, and execute ordered actions using templated URLs. Provides sample requests and responses to accelerate automation and reduce investigation time.

  https://learn.microsoft.com/en-us/entra/id-governance/tenant-governance/how-to-investigate-related-tenants-api

- **Mutable subjects in federated identity credentials**

  Explains the risks of mutable OIDC subject claims—such as subject recycling and dangling credentials—for federated identity in Microsoft Entra. Recommends anchoring trust to immutable subjects, periodically removing unused credentials, and applying least privilege. Shows how to implement immutable subject matching with standard or flexible federated credentials, including a detailed GitLab example and CLI/Graph steps.

  https://learn.microsoft.com/en-us/entra/workload-id/workload-identities-federated-credential-mutable-subjects

- **Migrate GitHub Actions federated credentials to immutable subjects**

  Provides a guided migration from name-based to immutable subjects for GitHub Actions federated credentials in Microsoft Entra to mitigate subject recycling risk. Details how to retrieve repository/owner IDs, create parallel credentials for a safe cutover, enable immutable subjects in GitHub, validate workflows, and retire the old credential. Helps strengthen supply chain security without interrupting CI/CD.

  https://learn.microsoft.com/en-us/entra/workload-id/workload-identities-github-immutable-subjects

## Major Changes

- **Cross-tenant delegated administration**

  Substantially repositions the article as the core reference for GDAP-based permissions across Microsoft services, detailing the two-layer model of relationship-level GDAP plus workload RBAC. Adds clear mappings for remote tenant groups and governance templates, and a new matrix of expected behaviors across Entra roles, Azure RBAC, Defender RBAC, and security groups. Provides recommended practices for customers and partners to right-size permissions, monitor activity, and use logging and policy controls for stronger governance.

  https://learn.microsoft.com/en-us/entra/id-governance/tenant-governance/cross-tenant-delegated-administration

- **Interpret tenant discovery data**

  Adds drill-down guidance that connects high-level discovery signals to underlying users and apps, helping admins validate findings and prioritize remediation. Clarifies data nuances such as metric magnitudes, live vs. aggregated data, log retention, and privacy considerations, and introduces Graph-based investigation. Enhances initial assessment with Microsoft-managed tenant identification to improve classification accuracy.

  https://learn.microsoft.com/en-us/entra/id-governance/tenant-governance/how-to-interpret-discovery-data

- **Prerequisites for Microsoft Entra Cloud Sync in Microsoft Entra ID**

  Updates prerequisites to officially support Windows Server 2025 for the Cloud Sync agent, removing prior warnings and KB dependencies. Refreshes OS support tables for gMSA and host requirements while clarifying support nuances for older OS versions. This simplifies planning and enables deployment on current server platforms.

  https://learn.microsoft.com/en-us/entra/identity/hybrid/cloud-sync/how-to-prerequisites

## Moderate Changes

- **Passkeys by default and retirement of Microsoft-provided SMS and voice authentication**

  Adds explicit opt-out instructions for the Sept 1, 2026–Feb 1, 2027 window using Microsoft Graph by setting optOutSettings.passkeyDynamicMigration to true. Clarifies that opting out delays automatic passkey enablement and Registration Campaign only during this period and that enforcement resumes Feb 1, 2027. Helps organizations manage rollout timing while preparing users for passkeys.

  https://learn.microsoft.com/en-us/entra/identity/authentication/concept-sms-voice-retirement

- **Customize emails sent from workflow tasks**

  Updates email customization to use dynamic attributes by Graph property names (for example, {{user.givenName}}) with a comprehensive table of supported attributes. Notes that the new syntax applies to newly created custom email tasks, while existing tasks continue to function with the previous format. This improves consistency and discoverability of available attributes.

  https://learn.microsoft.com/en-us/entra/id-governance/customize-workflow-email

- **Add OIDC for customer sign-in**

  Revises known limitations and documents that changing the Issuer URI for an existing OIDC IdP may not automatically update user flows. Provides a simple remediation: disable the IdP in the user flow, save, re-enable, and save again so the sign-in option appears. Reduces troubleshooting time for sign-in configuration changes.

  https://learn.microsoft.com/en-us/entra/external-id/customers/how-to-custom-oidc-federation-customers

- **Use cross-tenant delegated administration**

  Expands sign-in guidance for governed tenants, including navigation via the Entra admin center and direct admin portal URLs. Adds a new step-by-step flow with eligibility and role details, PIM activation for group-based roles, and clarifies behavior when multiple relationships exist. Streamlines prerequisites and steps to reduce sign-in friction.

  https://learn.microsoft.com/en-us/entra/id-governance/tenant-governance/how-to-delegated-administration

- **Global Secure Access and Universal Tenant Restrictions**

  Refocuses guidance on Universal Tenant Restrictions with TRv2 enforced via GSA clients or Remote Networks, removing proxy steering complexity. Simplifies the overview and configuration steps, clarifies prerequisites (including tunneling Entra ID services), and streamlines related content. Helps administrators deploy consistent tenant restrictions across protected apps.

  https://learn.microsoft.com/en-us/entra/global-secure-access/how-to-universal-tenant-restrictions

- **Lifecycle Workflow built-in tasks**

  Expands and restructures dynamic email attribute guidance with detailed tables for user, manager, and extension/custom attributes and the new {{user.graphPropertyName}} syntax. Highlights that the new format applies to new custom email tasks while preserving compatibility for existing ones. Improves accuracy and flexibility when personalizing lifecycle notifications.

  https://learn.microsoft.com/en-us/entra/id-governance/lifecycle-workflow-tasks

- **Microsoft-managed Conditional Access policies**

  Adds a new policy, “Require remediation for high-risk users,” that guides risk-based remediation for users flagged by Entra ID Protection (P2). Explains licensing, precedence, exclusions, and report-only usage, and notes that external users aren’t in scope. Helps tenants standardize enforcement for high-risk scenarios with minimal configuration.

  https://learn.microsoft.com/en-us/entra/identity/conditional-access/managed-policies

- **Related tenants in Tenant Governance**

  Introduces “Microsoft-managed tenants” labeling to identify Microsoft-owned infrastructure tenants discovered by signals. Clarifies that these typically need no action and helps admins focus on tenants that require governance. Indicator availability is noted for licensed admins with read permissions.

  https://learn.microsoft.com/en-us/entra/id-governance/tenant-governance/related-tenants