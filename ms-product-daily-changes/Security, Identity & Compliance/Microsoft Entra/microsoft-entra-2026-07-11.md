# Microsoft Entra
**Date created:** 2026-07-11 UTC  
**Tags:** Administration, Governance, Security  

## Major Changes

- **Add an on-premises application for remote access through application proxy in Microsoft Entra ID**

  Introduced a new requirement to explicitly grant admin consent for the User.Read delegated permission on newly created Application Proxy enterprise apps. Added an IMPORTANT notice that starting June 30, 2026, automatic admin consent won’t be granted for new apps, helping admins prepare for compliance and avoid provisioning failures. Expanded guidance includes step-by-step consent in the Microsoft Entra admin center, a Microsoft Graph PowerShell script, and verification steps to confirm the permission is applied.

  https://learn.microsoft.com/en-us/entra/identity/app-proxy/application-proxy-add-on-premises-application

- **Bring Your Own Device**

  Updated macOS guidance to require Mobile Device Management (MDM) enrollment and clarified that BYOD scenarios without enrollment aren’t supported. The platform behavior table now reflects the MDM requirement, removing prior references to Microsoft Entra registration without enrollment and Company Portal-based registration. These changes help organizations enforce consistent device compliance and access policies for macOS.

  https://learn.microsoft.com/en-us/entra/global-secure-access/concept-bring-your-own-device

## Moderate Changes

- **Configure assignment restriction for user-assigned managed identities (preview)**

  Marked the capability as preview and added guidance on supported resource providers and resource types in the Azure portal, noting that not all supported resources appear in the portal list. Expanded Azure CLI examples cover creating identities with restrictions, updating or removing restrictions, and listing associated resources, enabling more reliable and automated governance.

  https://learn.microsoft.com/en-us/entra/identity/managed-identities-azure-resources/configure-managed-identities-assignment-restriction

- **Assignment restriction for managed identities (preview)**

  Labeled assignment restrictions as a preview feature and added a section detailing supported resource providers and types in the Azure portal. Clarified that selecting “None” leaves an identity unrestricted, that the portal list may be incomplete, and directed users to Azure CLI when needed for full configuration coverage.

  https://learn.microsoft.com/en-us/entra/identity/managed-identities-azure-resources/managed-identities-assignment-restriction

- **Microsoft Entra ID Governance licensing for guest users**

  Added a billable action for Access Reviews – Catalog Access Reviews, specifying that charges occur when a guest user is included in a review. Included the corresponding Microsoft Graph API endpoint to help teams identify and manage usage: v1.0/identityGovernance/accessReviews/unified/definitions.

  https://learn.microsoft.com/en-us/entra/id-governance/microsoft-entra-id-governance-licensing-for-guest-users