# Dev and Admin for Dynamics 365 Business Central
**Date created:** 2026-08-01 UTC  
**Tags:** Administration, Security  

## Moderate Changes

- **Register Business Central on-premises in Microsoft Entra ID for integrating with other services**

  Clarified setup and security requirements for registering Business Central on-premises in Microsoft Entra ID. Endpoints (web client, OData, and SOAP) must be secured with a production certificate and exposed over HTTPS; guidance and updated redirect URI examples (e.g., BC280) are provided. The required Azure portal permission is now explicit (at least Application Developer), authentication guidance points to Microsoft Entra OpenID Connect, and troubleshooting examples for reply URLs were refined to reduce sign-in and consent errors.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/administration/register-app-azure