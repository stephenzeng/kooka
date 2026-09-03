# Microsoft Entra
**Date created:** 2026-09-03 UTC  
**Tags:** Governance, Guidance, Identity, Troubleshooting  

## New Articles

- **Troubleshoot STATUS_ACCOUNT_DISABLED in Microsoft Entra**

  Introduced a troubleshooting guide for hybrid Azure AD joined Windows devices that intermittently show STATUS_ACCOUNT_DISABLED during sign-in or unlock. Explains common symptoms and correlates event logs and codes (including AADSTS50034) to the underlying cause. Clarifies that stale local cache from PRT expiration or VSM key rollover combined with failed communication to on-premises AD—often after sleep, hibernation, or delayed VPN—triggers the issue. Notes the problem doesn’t affect Entra-native deployments and recommends moving to Entra-native where possible, with links to related guidance.

  https://learn.microsoft.com/en-us/entra/identity/devices/troubleshoot-intermittent-status-account-disabled

## Moderate Changes

- **Managed identities for Azure resources frequently asked questions**

  Added guidance on directory object quota behavior: when tenant usage reaches 98%, creating new managed identity service principals is blocked. Details which operations are affected (such as creating user-assigned identities or enabling system-assigned identities that require a new SP), clarifies that assigning existing user-assigned identities still works, notes soft-deleted objects count toward quota, and provides resolution steps to reduce usage or request an increase before retrying.

  https://learn.microsoft.com/en-us/entra/identity/managed-identities-azure-resources/managed-identities-faq

- **Prerequisites to validate and publish your app**

  Updated prerequisites for Microsoft Entra App Gallery onboarding to require a Partner One ID (formerly MPN ID). Explains what the ID is, which organization’s ID to use, and directs readers to contact their program administrator and consult Partner Center documentation.

  https://learn.microsoft.com/en-us/entra/identity/enterprise-apps/v2-howto-app-gallery-listing