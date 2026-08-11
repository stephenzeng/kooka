# Microsoft Entra
**Date created:** 2026-07-25 UTC  
**Tags:** Security  

## Major Changes

- **Tutorial: Develop and plan provisioning for a SCIM endpoint in Microsoft Entra ID**

  Introduced Workload Identity Federation (WIF) as a supported authentication method for SCIM provisioning, enabling JWT-based, secretless trust using OAuth 2.0 JWT bearer (RFC 7523). Added guidance on required Entra-provided values (issuer, JWKS URL, subject, audience) and ISV-provided values (client identifier, token endpoint, SCIM URL), with a per-customer workload identity requirement to avoid shared credentials. Included a step-by-step setup flow in the Entra admin center and links to the WIF implementation guide to streamline deployment and improve security posture.

  https://learn.microsoft.com/en-us/entra/identity/app-provisioning/use-scim-to-provision-users-and-groups

- **Submit a request to publish your application in Microsoft Entra application gallery**

  Retired references to the SCIM Validator tool and updated validation guidance to rely on the non-gallery application template. Added a recommended approach for Workload Identity Federation (WIF), highlighting JWT-based authentication, elimination of long‑lived secrets, and JWKS-based key validation, with a link to implementation guidance. These changes simplify the publishing checklist and align integrations with more secure, modern authentication patterns.

  https://learn.microsoft.com/en-us/entra/identity/enterprise-apps/v2-howto-app-gallery-listing

## Moderate Changes

- **Access token claims reference**

  Updated the AMR claim description to reflect that it can appear beyond v1.0 tokens. This clarifies claim behavior across token versions and helps apps avoid brittle version checks when evaluating authentication methods.

  https://learn.microsoft.com/en-us/entra/identity-platform/access-token-claims-reference

- **Host custom Proxy Automatic Configuration (PAC) files for Explicit Forward Proxy (Preview)**

  Added a security note that custom PAC hosting validates only basic JavaScript and recommends thorough code reviews. Also corrected the efpURL placeholder in the sample to use ${GSAEFP}, ensuring accurate configuration.

  https://learn.microsoft.com/en-us/entra/global-secure-access/how-to-custom-proxy-file-hosting

- **Configure Salesforce Sandbox for Single sign-on with Microsoft Entra ID**

  Clarified that v2.0 tokens include AMR and ACR claims and that AMR signals from external MFA providers are forwarded to Salesforce and other third‑party apps. Consolidated guidance to use Conditional Access for phishing‑resistant MFA and aligned with Salesforce device activation changes, while streamlining legacy AD FS specifics and noting ongoing standardization of AMR/ACR across federation providers.

  https://learn.microsoft.com/en-us/entra/identity/saas-apps/salesforce-sandbox-tutorial

- **Configure Salesforce for Single sign-on in Microsoft Entra ID**

  Updated notes to confirm inclusion of AMR and ACR in tokens for SAML/OIDC and forwarding of AMR signals from external MFA providers. Recommended Conditional Access to meet Salesforce phishing‑resistant MFA and device activation expectations, added explicit pointers for AD FS to include expected MFA assertions, and noted ongoing standardization work for AMR/ACR with other federation providers.

  https://learn.microsoft.com/en-us/entra/identity/saas-apps/salesforce-tutorial