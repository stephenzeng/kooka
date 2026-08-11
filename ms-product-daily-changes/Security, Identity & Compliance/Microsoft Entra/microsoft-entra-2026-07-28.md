# Microsoft Entra
**Date created:** 2026-07-28 UTC  
**Tags:** Administration, Governance, Security  

## New Articles

- **Configure device sync with Microsoft Entra Cloud Sync (preview)**

  Introduced guidance for synchronizing Active Directory computer objects to Microsoft Entra ID using Cloud Sync. Covers prerequisites, configuring the Service Connection Point via PowerShell, enabling device sync in the admin center, and reviewing supported attribute mappings. Details how to provision devices on demand, manage sync via Microsoft Graph (including AD2AADDeviceSync jobs), and recover deleted devices to streamline hybrid device management.

  https://learn.microsoft.com/en-us/entra/identity/hybrid/cloud-sync/device-sync

- **Configure Lovable (OIDC) for Single sign-on with Microsoft Entra ID**

  Added an OIDC SSO setup guide for Lovable, including prerequisites, adding the gallery app, and configuring the Microsoft Entra application (redirect URI, delegated permissions, and client secret). Provides Lovable-side configuration using the tenant discovery URL, client credentials, and optional login URL suffix, with instructions for creating a test user. Includes testing steps, timing guidance before enforcing SSO, and post-setup options like enforcing SSO, just-in-time user provisioning, and SCIM provisioning.

  https://learn.microsoft.com/en-us/entra/identity/saas-apps/lovable-oidc-tutorial

- **Configure Orgvue for Single sign-on with Microsoft Entra ID**

  Published a SAML SSO integration guide for Orgvue with step-by-step configuration and required SAML settings (Identifier, Reply URL, and Sign-on URL). Explains how to download and send federation metadata to Orgvue, create and assign test users, and validate access using Test this application, a direct sign-on URL, or My Apps. Highlights options to enhance session control using Microsoft Defender for Cloud Apps.

  https://learn.microsoft.com/en-us/entra/identity/saas-apps/orgvue-tutorial

## Moderate Changes

- **Cross-cloud settings**

  Added guidance on cross-cloud B2B sign-in behavior where login_hint is derived from the guest user’s mail attribute, not the home tenant UPN. Recommends aligning the guest mail attribute with the user’s home UPN to prevent extra prompts and account resolution failures in SSO flows.

  https://learn.microsoft.com/en-us/entra/external-id/cross-cloud-settings

- **Configure Global Relay Identity Sync for automatic user provisioning with Microsoft Entra ID**

  Updated provisioning steps to use OAuth client credentials, adding Client identifier, Client secret, and OAuth token endpoint along with the Tenant URL. Clarified the Test connection procedure to validate connectivity with these credentials for a more reliable setup.

  https://learn.microsoft.com/en-us/entra/identity/saas-apps/global-relay-identity-sync-provisioning-tutorial

- **Update user attributes with Lifecycle Workflows**

  Marked general availability by removing Preview labels and aligning UI text with the finalized task name. Expanded support to include additional attribute types, directory extension attributes for synced users, and now supporting employeeLeaveDateTime; added guidance for datetime attributes to use a specific date or system.now. Clarified limitations indicating only directory extension attributes are supported for synced users.

  https://learn.microsoft.com/en-us/entra/id-governance/how-to-lifecycle-workflow-update-user-attributes

- **Configure Visa Spend Clarity for Enterprise for automatic user provisioning with Microsoft Entra ID**

  Migrated provisioning to OAuth client credentials, replacing secret token usage with Tenant URL, Client identifier, Client secret, and OAuth token endpoint. Updated the test connection flow and imagery to reflect the new authentication model, improving security and reliability.

  https://learn.microsoft.com/en-us/entra/identity/saas-apps/visa-provisioning-tutorial