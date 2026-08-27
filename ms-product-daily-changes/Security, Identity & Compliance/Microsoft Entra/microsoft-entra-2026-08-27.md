# Microsoft Entra
**Date created:** 2026-08-27 UTC  
**Tags:** Best Practices, Compliance, Configuration, Get Started, Governance, Guidance, Identity, Security  

## New Articles

- **SSO requirements for Microsoft Entra App Gallery**

  Introduced a comprehensive requirements guide for apps seeking listing in the Microsoft Entra App Gallery. It details SAML SSO and multitenant OIDC requirements, including protocol expectations, validation via a non-gallery app, and security best practices. The article also defines ISV obligations, documentation standards, and links to next steps for validation and publishing.

  https://learn.microsoft.com/en-us/entra/identity/enterprise-apps/app-gallery-sso-requirements

- **User provisioning requirements for Microsoft Entra App Gallery**

  Added end-to-end requirements for SCIM-based user provisioning integrations, including SCIM 2.0 endpoints, performance targets, supported operations, and correct API behaviors. It clarifies OAuth 2.0 client credentials, token and secret management, and workload identity federation options. Guidance includes ISV obligations, documentation expectations, references to known limitations, and links to implementation and publishing steps.

  https://learn.microsoft.com/en-us/entra/identity/enterprise-apps/app-gallery-user-provisioning-requirements

- **Publish your app to Microsoft Entra App Gallery**

  Introduced a step-by-step tutorial for self-service publishing of validated applications. It covers prerequisites, accessing the publishing experience, creating and completing a submission, associating validation results, and preparing customer-facing documentation and branding. The guide explains how to track status, address review feedback, and manage updates post-publication.

  https://learn.microsoft.com/en-us/entra/identity/enterprise-apps/publish-app-gallery

- **Update or remove your app from the Microsoft Entra App Gallery**

  Added instructions for submitting update or removal requests through the Microsoft Application Network portal. The article outlines supported change types (for SSO, MDM listings, and user provisioning), how to request access, and how to resolve common blockers. It also links to troubleshooting guidance for blocked sign-in errors.

  https://learn.microsoft.com/en-us/entra/identity/enterprise-apps/update-or-remove-app-gallery

- **Validate an OIDC multitenant app for Microsoft Entra App Gallery onboarding**

  Added a how-to guide for validating an OIDC multitenant app using the Microsoft Entra App Validator browser extension. It walks through prerequisites, running the auth flow, interpreting validation results, and declaring user identifier claims for account matching. Successful validation yields a time-bound Test ID required for publishing.

  https://learn.microsoft.com/en-us/entra/identity/enterprise-apps/validate-oidc-multitenant-app-gallery

- **Validate a SAML single sign-on app for Microsoft Entra App Gallery onboarding**

  Introduced a validation tutorial for SAML 2.0 integrations using the App Validator extension prior to gallery submission. It covers configuring a non-gallery app, running IdP- and SP-initiated scenarios (including an expired-certificate test), and reviewing results with identity-mapping requirements. The article includes troubleshooting guidance and scripts to streamline testing.

  https://learn.microsoft.com/en-us/entra/identity/enterprise-apps/validate-saml-single-sign-on-app-gallery

## Major Changes

- **Global Secure Access Client Release Notes**

  Added guidance on automatic client upgrades via Windows Update starting November 2026, with minimum supported versions and an installer parameter to opt out. Introduced release 2.32.294 with improvements like a “Prefer local network” option for overlapping subnets, faster tunnel creation, updated .NET runtime, telemetry updates, accessibility enhancements, and fixes. Clarified upgrade behavior and administrator responsibilities to ensure compliant and predictable client rollouts.

  https://learn.microsoft.com/en-us/entra/global-secure-access/reference-windows-client-release-history

- **Strengthen federated sign-in security**

  Significantly expanded guidance on Federated Token Validation Policy to position it as a defense-in-depth control that enforces domain consistency during sign-in. The update explains existing validation checks, cross-domain scenarios, and how the policy strengthens federation security, with expanded sign-in flow steps. Policy administration guidance is clarified with recommended use cases for validatingDomains settings and explicit cautions for permissive options. Operational guidance emphasizes preparation, monitoring, and exception handling with compensating controls.

  https://learn.microsoft.com/en-us/entra/identity/users/strengthen-federated-sign-in-security

- **Prerequisites to validate and publish your app**

  The article is restructured to highlight shared, capability-agnostic prerequisites and defer protocol-specific details to dedicated requirement pages. It helps ISVs select capabilities (SAML/OIDC SSO and SCIM), provides a consolidated prerequisite checklist, and strengthens guidance for OIDC multitenancy and SCIM (including OAuth 2.0 client credentials). Documentation expectations are consolidated, and next steps now point to separate requirement and planning resources, simplifying the publishing path.

  https://learn.microsoft.com/en-us/entra/identity/enterprise-apps/v2-howto-app-gallery-listing

## Moderate Changes

- **Create a governed workforce tenant**

  Clarified that a governance relationship forms only when the home tenant has a default governance policy template. Updated prerequisites to require the Tenant Creator role regardless of tenant-creation restrictions, and refined post-creation behavior based on template availability. These changes help admins plan role assignments and understand conditional provisioning outcomes.

  https://learn.microsoft.com/en-us/entra/id-governance/tenant-governance/how-to-create-tenant

- **Known limitations for Global Secure Access**

  Updated government cloud availability to specify support for GCC and not yet for GCC-H, DoD, or other sovereign clouds. Removed older GCC-specific notes about FIPS 140-2 status and potential data residency/TLS termination outside the US. This streamlines compliance and deployment expectations for government customers.

  https://learn.microsoft.com/en-us/entra/global-secure-access/reference-current-known-limitations