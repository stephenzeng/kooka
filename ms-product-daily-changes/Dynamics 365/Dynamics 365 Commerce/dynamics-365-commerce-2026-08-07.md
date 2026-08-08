# Dynamics 365 Commerce
**Change date:** 2026-08-07 UTC  
**Tags:** Administration, Security  

## Major Changes

- **Create and configure a Microsoft Entra application for account manager sign-in**

  Expanded guidance to support both Azure AD B2C and Microsoft Entra External ID (EEID) with clear, tabbed instructions. Added end-to-end EEID setup steps, including app registration, redirect URIs, client secrets, configuring Azure B2B as a custom OIDC provider, user flow integration, and claims mapping. Introduced configuration for a dedicated app registration that exposes a user_impersonation scope, granting delegated permissions (admin consent) to the site sign-in app, and wiring the scope into Commerce site builder authentication profiles. Clarified naming requirements and updated ID/scope examples to reduce misconfiguration and streamline deployment.

  https://learn.microsoft.com/en-us/dynamics365/commerce/dev-itpro/obo-create-aad-application

## Moderate Changes

- **Create and modify B2B pages for on behalf of (OBO) functionality**

  Clarified that the detailed steps apply only to Azure AD B2C and that EEID does not support custom sign-in/sign-up pages. For EEID, guidance explains that the B2B account manager sign-in option appears automatically after configuring the OIDC provider and adding it to the user flow, helping teams avoid unnecessary site builder customization.

  https://learn.microsoft.com/en-us/dynamics365/commerce/dev-itpro/obo-add-pages-site-builder

- **Set up and configure on behalf of (OBO) functionality in Commerce headquarters**

  Added EEID-specific instructions to register the Application (Client) ID of the app exposing the user_impersonation scope as a relying party under the EEID tenant issuer URL, with Type set to Confidential and User Type set to Worker. This ensures correct impersonation and authentication flow in EEID environments.

  https://learn.microsoft.com/en-us/dynamics365/commerce/dev-itpro/obo-configure-hq