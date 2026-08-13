# Microsoft Entra
**Date created:** 2026-08-13 UTC  
**Tags:** Configuration, Guidance, Identity, Security  

## Major Changes

- **Configure Puzzel for automatic user provisioning with Microsoft Entra ID**

  Added support for OAuth2 Client Credentials Grant to improve secure, service-to-service authentication. Introduced step-by-step instructions to create an OIDC client in the Puzzel portal, including token lifetime settings, generating a client secret, and collecting the Client ID/Secret and Token Endpoint. Updated Microsoft Entra provisioning guidance to select Client Credentials and provide Tenant URL, Client ID, Client Secret, and Token Endpoint, with new screenshots. This streamlines setup and reduces reliance on less secure auth methods.

  https://learn.microsoft.com/en-us/entra/identity/saas-apps/puzzel-provisioning-tutorial

- **Configure Zscaler Provisioning for automatic user provisioning with Microsoft Entra ID**

  Added support for Client Credentials authentication and updated configuration to require Tenant URL, Client identifier, Client secret, and OAuth token endpoint, replacing the prior Secret Token flow. Expanded user attribute mappings with a comprehensive set of SCIM attributes, including core profile fields, multiple emails, addresses, phone numbers, and enterprise extensions (such as costCenter, division, department, and manager), and refreshed the test connection example. These changes enable stronger authentication and more complete, accurate user synchronization.

  https://learn.microsoft.com/en-us/entra/identity/saas-apps/zscaler-zidentity-provisioning-tutorial

## Moderate Changes

- **Grant agents access to Microsoft 365 resources**

  Added a new section detailing the permissions required for agent communication across Outlook, OneDrive/SharePoint, and Teams, including a matrix of Microsoft Graph scopes for inbound and outbound operations. Clarified that these permissions must be defined in the agent identity blueprint and consented by a tenant admin to enable cross-channel messaging. This helps admins provision the exact permissions needed for reliable agent operation.

  https://learn.microsoft.com/en-us/entra/agent-id/grant-agent-access-microsoft-365

- **Microsoft Entra Connect: Cloud authentication via Staged Rollout**

  Reworked guidance on authentication behavior to explicitly list scenarios that trigger an extra interactive sign-in, including when users are added to or removed from Staged Rollout and when certain Microsoft Entra ID Protection events reset rollout state. Renamed and refined the workaround section to highlight using Temporary Access Pass to avoid an extra federated sign-in during transitions. This improves predictability during rollout changes and reduces user friction.

  https://learn.microsoft.com/en-us/entra/identity/hybrid/connect/how-to-connect-staged-rollout