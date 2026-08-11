# Microsoft Entra
**Date created:** 2026-08-11 UTC  
**Tags:** Configuration, Guidance, Identity, Security  

## Major Changes

- **Token Protection in Microsoft Entra Conditional Access**

  Expanded Token Protection to include preview support for browser-based applications accessing Azure Resource Manager, alongside existing native app support. Updated platform availability to distinguish native vs. browser readiness across Windows, iOS/iPadOS, and macOS, and added a link to web app deployment guidance. Clarified that previously listed supported resources apply to native apps, while browser-based enforcement (preview) is limited to selected web apps configured for the Windows Azure Service Management API resource. Added device and browser prerequisites for Windows and macOS, including OS, browser, extension, and configuration requirements.

  https://learn.microsoft.com/en-us/entra/identity/conditional-access/concept-token-protection

## Moderate Changes

- **Agent OAuth flows: On behalf of flow**

  Clarified that child agent identities cannot perform interactive /authorize or receive interactive consent (AADSTS82014); instead, preauthorize delegated permissions via inheritable permissions on the parent agent blueprint with admin consent so children inherit required scopes. Refined OBO validation: Tc must target the agent blueprint client ID (tokens for other resources like Microsoft Graph are rejected with AADSTS50013); T1 is requested with scope api://AzureADTokenExchange/.default, and Entra verifies T1 is bound to the blueprint (azp) and the child agent identity (sub). These updates help avoid consent blockers and ensure correct token audience and binding for reliable OBO exchanges.

  https://learn.microsoft.com/en-us/entra/agent-id/agent-on-behalf-of-oauth-flow

- **Configure Orgvue for Single sign-on with Microsoft Entra ID**

  Updated SAML settings to new patterns: Identifier and Reply URL now use the orgvue-staging.us-east-1.concentra.io domain, and the Sign-on URL uses a login-gateway pattern with a domain parameter. Clarified that Reply URL and Sign-on URL are placeholders that must be replaced with tenant-specific values, with guidance to contact Orgvue support as needed.

  https://learn.microsoft.com/en-us/entra/identity/saas-apps/orgvue-tutorial