# Microsoft Entra
**Date created:** 2026-07-20 UTC  
**Tags:** Security  

## Moderate Changes

- **Add OpenID Connect as an external identity provider**

  Updated guidance by removing a previous note and limitation related to using email one-time passcode (OTP) for MFA when user email collection is optional. This clarifies expected MFA behavior for OIDC external identity setups and reduces confusion for tenant configurations where email isn’t captured by default. Administrators should review MFA configurations and user communications to align with the clarified guidance.

  https://learn.microsoft.com/en-us/entra/external-id/customers/how-to-custom-oidc-federation-customers