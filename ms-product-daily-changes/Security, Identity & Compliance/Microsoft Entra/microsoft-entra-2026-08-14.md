# Microsoft Entra
**Date created:** 2026-08-14 UTC  
**Tags:** Automation, Configuration, Get Started, Governance, Guidance, Identity, Security  

## New Articles

- **Federate a Google Cloud workload identity**

  Introduced a step-by-step tutorial to enable secretless access to Azure resources by federating a Google Cloud service account with a Microsoft Entra application. The guide covers identifying the service account and configuring a federated identity credential (issuer=https://accounts.google.com, subject=<service-account-unique-id>, audience=api://AzureADTokenExchange). It shows how to obtain a Google ID token and exchange it for a Microsoft Entra access token using the Azure Identity SDK, with JavaScript samples and an option for user-assigned managed identities. Cleanup guidance and links to related federation topics are included to streamline adoption.

  https://learn.microsoft.com/en-us/entra/workload-id/workload-identity-federation-google-cloud

- **Federate a SPIFFE/SPIRE workload identity**

  Added a tutorial for federating SPIFFE/SPIRE workloads with Microsoft Entra ID to remove the need for stored secrets when accessing Azure resources. It walks through deploying SPIRE with JWT-SVID and OIDC discovery, ensuring RS256 signing with keys marked for signature use, and assigning SPIFFE IDs to workloads. The article details configuring a federated identity credential and exchanging a SPIFFE JWT-SVID for a Microsoft Entra access token via the Azure Identity SDK, plus operational notes on permissions, endpoints, and validation. Cleanup steps help maintain a secure and tidy environment post-testing.

  https://learn.microsoft.com/en-us/entra/workload-id/workload-identity-federation-spiffe-spire

## Major Changes

- **Include custom data provided resource in the catalog for catalog user Access Reviews**

  Marked the feature as generally available and overhauled the procedures for adding a custom data provided resource with a new multi-tab flow and Logic App deployment steps. Introduced Logic App integration to automate data upload at review start and automatic application of decisions at completion, with a template provided. Expanded the CSV schema with required fields (including ScopeId, ScopeDisplayName, owner columns, and CustomData) and clarified how owner columns drive resource owner reviews. Added guidance for manually applying results in the portal and removed the previous manager-only, single-stage limitation, enabling broader review scenarios.

  https://learn.microsoft.com/en-us/entra/id-governance/custom-data-resource-access-reviews

## Moderate Changes

- **Catalog Access Reviews**

  Updated the article to reflect general availability by removing Preview labels and replacing “managers” with “reviewers” to reflect broader reviewer support. Clarified reviewer selection guidance and added an operational note that changes within 12 hours of review start may not be captured. Updated references and links related to custom data provided resources.

  https://learn.microsoft.com/en-us/entra/id-governance/catalog-access-reviews

- **View, add, and remove assignments for an access package in entitlement management**

  Removed guidance that suggested creating a separate policy to bypass approval requirements for direct assignments. This aligns the documentation with current approval enforcement and removes the previously recommended workaround.

  https://learn.microsoft.com/en-us/entra/id-governance/entitlement-management-access-package-assignments

- **Delegation and roles in entitlement management**

  Eliminated a note stating that Access package assignment managers cannot bypass approval settings and the related recommendation to use an approval-free policy for specific identities. The update reduces confusion and aligns guidance with current entitlement management behavior.

  https://learn.microsoft.com/en-us/entra/id-governance/entitlement-management-delegate

- **Manage rules for dynamic membership groups in Microsoft Entra ID**

  Added guidance on evaluating agents’ user accounts with user-based dynamic membership rules, including how to explicitly include or exclude them (for example, by targeting specific agent identity blueprints). Clarified that agent identities as service principals aren’t supported as dynamic group members.

  https://learn.microsoft.com/en-us/entra/identity/users/groups-dynamic-membership