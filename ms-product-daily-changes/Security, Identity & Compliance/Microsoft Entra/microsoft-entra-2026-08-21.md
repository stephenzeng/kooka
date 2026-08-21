# Microsoft Entra
**Date created:** 2026-08-21 UTC  
**Tags:** Automation, Best Practices, Configuration, Deprecation, Governance, Guidance, Identity, Security, Troubleshooting  

## New Articles

- **Clear attribute values (Preview)**

  Introduced a preview capability to clear target attribute values when source attributes are null or empty in Microsoft Entra provisioning. Explains scope and limits (API-driven inbound provisioning to Entra ID and on-premises AD; single-valued attributes only) and how to enable “Flow null values” in both source schema and target mappings. Provides payload examples, verification steps, and troubleshooting to prevent unintended clears.

  https://learn.microsoft.com/en-us/entra/identity/app-provisioning/clear-attribute-values

- **Strengthen federated sign-in security**

  New concept guidance on Federated Token Validation Policy to block cross-domain federated sign-ins by enforcing root domain alignment between the federated realm and the user UPN. Details risks of cross-realm impersonation, default enforcement behavior and error handling, and how to prepare, validate, and monitor impact. Covers Microsoft Graph beta administration and configuration modes to tailor domain validation to organizational needs.

  https://learn.microsoft.com/en-us/entra/identity/users/strengthen-federated-sign-in-security

## Major Changes

- **Token Protection Deployment Guide - Apple Platforms**

  Marked general availability by removing “Preview” and simplifying setup guidance. Updated the supported apps matrix to include Microsoft Scout on iPadOS. Streamlined deployment by removing the need for the use_most_secure_storage flag and directing admins to enable the Microsoft Enterprise SSO plug-in on Apple devices or use Platform SSO on macOS, reducing configuration complexity.

  https://learn.microsoft.com/en-us/entra/identity/conditional-access/deployment-guide-token-protection-apple

- **Error AADSTS50105 - The signed-in user isn't assigned to a role for the application**

  Overhauled troubleshooting guidance to cover SAML, OIDC, OAuth 2.0, WS-Fed, and Application Proxy scenarios. Clarifies how the “Assignment required?” setting and app role assignments drive the error, including nuances like Default Access, nested groups, and admin bypass behavior. Adds step-by-step resolutions, role and licensing prerequisites for group-based assignment, testing guidance, and updated references for related error codes.

  https://learn.microsoft.com/en-us/troubleshoot/entra/entra-id/app-integration/error-code-AADSTS50105-user-not-assigned-role

- **CSS reference guide for customizing company branding**

  Expanded the deprecation to include both layout and positioning properties and clarified tenant eligibility and cutoff dates for configuring custom CSS. Significantly broadened the list of deprecated properties and refined rationale aligned to the Secure Future Initiative and phishing resistance. Added detailed remediation steps, including admin center, Microsoft Graph, and tooling guidance to review and adapt branding for all locales.

  https://learn.microsoft.com/en-us/entra/fundamentals/reference-company-branding-css-template

## Moderate Changes

- **Microsoft Entra ID attestation for FIDO2 security key vendors**

  Updated the FIDO Alliance MDS reference to version 275 and added new eligible authenticators. Thetis Pro FIDO2 Key and TruU FIDO2 Authenticator are now included in the attestation table, helping organizations validate broader device options.

  https://learn.microsoft.com/en-us/entra/identity/authentication/concept-fido2-hardware-vendor

- **Token Protection in Microsoft Entra Conditional Access**

  Updated platform support: native apps on iOS/iPadOS and macOS moved from Preview to General Availability. Browser-based app support remains unchanged, clarifying rollout status for administrators planning deployments.

  https://learn.microsoft.com/en-us/entra/identity/conditional-access/concept-token-protection

- **Configure workload identity-based authentication for SAP SuccessFactors provisioning (Preview)**

  Generalized the basic authentication deprecation note by removing a specific date and removed a note about current workload identity enablement status. No procedural changes were made, focusing the article on durable guidance rather than time-bound messaging.

  https://learn.microsoft.com/en-us/entra/identity/app-provisioning/configure-workload-identity-sap-successfactors-provisioning

- **Tutorial - Customize user provisioning attribute-mappings for SaaS applications in Microsoft Entra ID**

  Clarified handling of null and cleared values in provisioning. By default, nulls are not sent, and clearing attribute values is a preview feature limited to API-driven inbound provisioning apps, with references to enablement steps.

  https://learn.microsoft.com/en-us/entra/identity/app-provisioning/customize-application-attributes

- **Add company branding to your organization's sign-in page**

  Updated deprecation guidance for custom CSS, adding tenant eligibility rules and configuration cutoff dates tied to the Secure Future Initiative. Emphasizes security and phishing resistance and retains references to the CSS template guide for impacted properties and remediation.

  https://learn.microsoft.com/en-us/entra/fundamentals/how-to-customize-branding

- **Customize the sign-in experience for your application with branding themes**

  Expanded the Important note to cover deprecation of layout and positioning properties, plus new eligibility rules and configuration cutoffs. Reinforces the phased retirement plan with security rationale and links to remediation resources.

  https://learn.microsoft.com/en-us/entra/fundamentals/how-to-customize-branding-themes-apps

- **API-driven inbound provisioning concepts**

  Added guidance for the “clear attribute values (Preview)” feature and cautions to include complete user records in each bulk request to avoid unintended clears. Updated scenarios and added an external learning resource for API-driven provisioning patterns.

  https://learn.microsoft.com/en-us/entra/identity/app-provisioning/inbound-provisioning-api-concepts

- **Frequently asked questions about API-driven inbound provisioning**

  Added FAQs confirming support for clearing existing user attributes via the preview capability and clarifying that /bulkUpload does not support user deletions. Recommends Lifecycle Workflows to automate post-termination deletions.

  https://learn.microsoft.com/en-us/entra/identity/app-provisioning/inbound-provisioning-api-faqs

- **Optional claims reference**

  Clarified AMR indicators for certificate-based authentication by distinguishing PRMFA (“hwk”) from single-factor or device-based X.509 (“x509”). Added guidance that “x509” alone is not sufficient for phishing-resistant MFA and requires an additional MFA factor.

  https://learn.microsoft.com/en-us/entra/identity-platform/optional-claims-reference

- **Single sign-on SAML protocol**

  Added device-based X.509 authentication details, updating tables with AuthnContextClassRef “X509” and amr “x509.” Clarified that x509 by itself does not meet phishing-resistant MFA requirements, guiding architects on correct assurance signaling.

  https://learn.microsoft.com/en-us/entra/identity-platform/single-sign-on-saml-protocol

- **Understanding errors during Microsoft Entra synchronization**

  Expanded error coverage by adding DataValidationFailed alongside IdentityDataValidationFailed. Included a new scenario for onPremisesObjectIdentifier changes due to hard match and updated fixes to direct admins to appropriate recovery paths.

  https://learn.microsoft.com/en-us/entra/identity/hybrid/connect/tshoot-connect-sync-errors