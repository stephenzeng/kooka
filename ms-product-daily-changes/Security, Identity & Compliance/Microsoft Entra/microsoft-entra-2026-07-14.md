# Microsoft Entra
**Date created:** 2026-07-14 UTC  
**Tags:** Security  

## New Articles

- **Passkeys by default and retirement of Microsoft-provided SMS and voice authentication**

  Announced passkeys as the default authentication in Microsoft Entra ID and the retirement of Microsoft-provided SMS and voice MFA on a phased timeline. Provides guidance to inventory SMS/voice users, migrate them to synced or device-bound passkeys, and run a passkey registration campaign. Outlines options to transition to customer-managed telecom providers via the Microsoft Security Store, with key availability dates, and details post-retirement behavior and an opt-out window. Includes a communication plan and FAQs to help organizations plan, budget, and execute the change with minimal disruption.

  https://learn.microsoft.com/en-us/entra/identity/authentication/concept-sms-voice-retirement

- **Host custom Proxy Automatic Configuration files for Explicit Forward Proxy in Microsoft Entra Internet Access**

  Introduced support for hosting custom PAC files for Global Secure Access Explicit Forward Proxy (preview), enabling advanced routing logic, exclusions, and coexistence scenarios. Provides step-by-step instructions to create, upload, enable/disable, and edit PAC files in the admin center, including required template edits and use of the ${GSAEFP} placeholder. Highlights operational considerations such as device caching behavior, size limits (up to 950 KB; recommended under 250 KB), and tenant limits (up to 20 PAC files) to ensure reliable deployment.

  https://learn.microsoft.com/en-us/entra/global-secure-access/how-to-custom-proxy-file-hosting

## Moderate Changes

- **Explicit Forward Proxy overview**

  Updated the article to reflect general availability by removing preview labels and disclaimers; no functional content changed. This signals production readiness and helps admins align deployment plans with a GA service.

  https://learn.microsoft.com/en-us/entra/global-secure-access/concept-explicit-forward-proxy

- **Explicit Forward Proxy session management**

  Removed preview indicators from the title and notes to reflect general availability; core session management guidance remains the same. This clarifies support status and reduces ambiguity for policy configuration in production environments.

  https://learn.microsoft.com/en-us/entra/global-secure-access/concept-explicit-forward-proxy-session-management

- **Configure Microsoft Edge with Explicit Forward Proxy by using an Intune application management policy**

  Updated to reflect GA by removing preview wording while leaving procedures unchanged. This helps organizations confidently apply the documented configuration in production.

  https://learn.microsoft.com/en-us/entra/global-secure-access/how-to-configure-explicit-forward-proxy-intune-policy

- **Tutorial: Develop and plan provisioning for a SCIM endpoint in Microsoft Entra ID**

  Revised authentication guidance by retiring the OAuth authorization code grant for provisioning and clarifying that new connectors use OAuth 2.0 client credentials. This change improves security alignment and ensures future compatibility for SCIM integrations.

  https://learn.microsoft.com/en-us/entra/identity/app-provisioning/use-scim-to-provision-users-and-groups