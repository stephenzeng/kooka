# Microsoft Entra
**Date created:** 2026-07-31 UTC  
**Tags:** Administration, Governance, Security  

## Major Changes

- **Licensing for Microsoft Entra Tenant Governance**

  Expanded licensing guidance with scenario-based calculations for Tenant Governance. Clarifies Basic vs. Premium capacities, including daily configuration drift monitoring under Basic limits and expanded capacity using Premium licenses (10 resources/day per license) plus large monthly snapshots (35 resources/month per license). Defines governance relationship licensing rules—licenses are required only in the governing tenant and counted by configuring admins, not the number of relationships—with examples to estimate needs. Details licensing for Related tenants discovery (license required for each admin who uses the feature) and notes secure tenant creation availability via Microsoft Entra Free for paid customers, with prerequisites.

  https://learn.microsoft.com/en-us/entra/id-governance/tenant-governance/licensing

## Moderate Changes

- **Passkeys by default and retirement of Microsoft-provided SMS and voice authentication**

  Added an FAQ clarifying scope and impact. Azure AD B2C tenants are out of scope and unaffected by this announcement, while Microsoft Entra External ID will be addressed next year in a separate communication. No immediate changes are required for these tenants.

  https://learn.microsoft.com/en-us/entra/identity/authentication/concept-sms-voice-retirement

- **Prerequisites for Microsoft Entra Connect**

  Removed a prior IMPORTANT note about a Windows Server 2025 issue that could affect sync for groups over 10,000 members, along with the associated KB update and restart guidance. This streamlines the prerequisites and avoids directing admins to an outdated workaround.

  https://learn.microsoft.com/en-us/entra/identity/hybrid/connect/how-to-connect-install-prerequisites

- **Mutable subjects in federated identity credentials**

  Added a GitLab-specific section for flexible federated identity credentials that require matching the sub claim plus additional immutable claims (project_id, namespace_id, and optionally user_id) to enforce a precise trust boundary. Includes JSON examples showing how to validate project/namespace and further restrict trust to a specific user, using IDs present in GitLab ID tokens.

  https://learn.microsoft.com/en-us/entra/workload-id/workload-identities-federated-credential-mutable-subjects

- **Migrate GitHub Actions federated credentials to immutable subjects**

  Introduced guidance for GitHub OIDC requiring credentials to match the sub claim as well as repository_id and optionally repository_owner_id to tighten trust boundaries. Provides JSON examples using claimsMatchingExpression to verify repository and repository owner with IDs from the GitHub OIDC token.

  https://learn.microsoft.com/en-us/entra/workload-id/workload-identities-github-immutable-subjects