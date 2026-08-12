# Microsoft Entra
**Date created:** 2026-08-12 UTC  
**Tags:** Best Practices, Configuration, Governance, Guidance, Identity, Security, Troubleshooting  

## New Articles

- **Web filtering in Global Secure Access (V2)**

  Introduced a new concept article outlining the V2 web filtering model for Microsoft Entra Internet Access, consolidating multiple V1 policies into a single V2 policy with rule-based actions and a policy-level default action. Clarifies destination matching by treating FQDNs as URLs, changing how matches are evaluated. Explains policy, rule, and security profile relationships, with guidance on authoring policies, adding rules, and configuring priorities, sources, HTTP methods, destinations, and actions. Details V2 and V1 coexistence and evaluation order, including terminal Block behavior and non-terminal Allow, along with logging behavior and the update/delete-only state of V1 once V2 policies exist.

  https://learn.microsoft.com/en-us/entra/global-secure-access/concept-web-filtering

## Major Changes

- **Discover identities in target applications with account discovery**

  Added end-to-end guidance for retrieving account discovery results using Microsoft Graph (beta), including supported list, get, and filter operations and links to identityCorrelation resources. Introduced investigation workflows with Microsoft MCP Server for Enterprise (preview), with prerequisites, example natural-language queries, sample Graph requests, and mappings for correlation statuses. Reorganized the article to foreground Graph retrieval steps and refined examples for assigning correlated users, while clarifying prerequisites, connector behavior, and application support to streamline investigations.

  https://learn.microsoft.com/en-us/entra/identity/app-provisioning/how-to-account-discovery

## Moderate Changes

- **Host custom Proxy Automatic Configuration (PAC) files for Explicit Forward Proxy (Preview)**

  Clarified JavaScript case sensitivity for PAC files and standardized variable naming from efpURL to efpUrl to prevent runtime errors. Updated examples to correctly reference the ${GSAEFP} endpoint and set var efpUrl = "HTTPS ${GSAEFP}"; to ensure consistent behavior.

  https://learn.microsoft.com/en-us/entra/global-secure-access/how-to-custom-proxy-file-hosting

- **Configure optional claims**

  Expanded guidance for the AMR claim, including steps to configure granular AMR values for SAML apps via the application manifest (include_granular_amr) and Microsoft Graph PATCH API with JSON examples. Clarified that include_granular_amr applies only to SAML tokens and added guidance for OIDC apps to request amr in ID and access tokens.

  https://learn.microsoft.com/en-us/entra/identity-platform/optional-claims