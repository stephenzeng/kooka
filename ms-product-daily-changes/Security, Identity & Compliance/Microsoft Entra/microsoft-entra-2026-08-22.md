# Microsoft Entra
**Date created:** 2026-08-22 UTC  
**Tags:** Configuration, Governance, Guidance, Identity, Licensing, Security  

## New Articles

- **Microsoft Entra External ID credential management API reference**

  Introduced a new API reference for customer self-service passkey management using delegated tokens (no app-only), including prerequisites and steps to provision the service principal and permissions. Documents endpoints to list credentials, begin passkey registration (WebAuthn creation options with continuation tokens), activate a passkey, and delete a passkey. Clarifies supported credential types (passkeys/FIDO only), request/response schemas, and headers. Provides a comprehensive error model with codes, causes, and recommended caller actions, enabling secure low-privilege integrations for passkey lifecycle operations.

  https://learn.microsoft.com/en-us/entra/identity-platform/reference-credential-management-api

## Major Changes

- **Global Secure Access Client for macOS Release Notes**

  Removed the previously published release notes for version 1.1.26060207, including all listed features and fixes. This retraction signals the content is no longer applicable and should not be used for planning or deployment decisions. Customers should disregard earlier guidance tied to that version and monitor the release notes page for future updates or republished details.

  https://learn.microsoft.com/en-us/entra/global-secure-access/reference-macos-client-release-history

## Moderate Changes

- **Create a lifecycle workflow - Microsoft Entra ID**

  Updated guidance to highlight creating workflows from built-in templates or by cloning an existing workflow. Added step-by-step instructions (with visuals) for cloning from the workflow list or during creation. Clarified that building a workflow from scratch requires using Microsoft Graph.

  https://learn.microsoft.com/en-us/entra/id-governance/create-lifecycle-workflow

- **Quickstart: Create a new tenant in Microsoft Entra ID**

  Marked Secure add-on tenant creation as generally available by removing the preview label and prerelease disclaimer. This signals production readiness and reduces ambiguity for rollout planning.

  https://learn.microsoft.com/en-us/entra/fundamentals/create-new-tenant

- **Create a governed workforce tenant**

  Refined prerequisites to require at least one paid, license-based Microsoft product in the home tenant and a paid EA or Pay-As-You-Go Azure subscription. Made the default governance policy template optional for establishing governance during creation and clarified scope by referencing External ID for customer-facing scenarios.

  https://learn.microsoft.com/en-us/entra/id-governance/tenant-governance/how-to-create-tenant

- **Install the Global Secure Access Client for macOS**

  Simplified Intune detection rule guidance by removing the prior IMPORTANT note and the optional step to exclude com.microsoft.autoupdate2 from detection rules. The streamlined instructions reduce configuration complexity and potential conflicts in deployment workflows.

  https://learn.microsoft.com/en-us/entra/global-secure-access/how-to-install-macos-client

- **Sign in with passkeys in Microsoft Entra External ID**

  Updated guidance to recommend the preview credential management API with delegated permissions for customer self-service passkey registration and management, replacing prior references to FIDO2 provisioning APIs. Clarified that the Microsoft Graph passkey sample demonstrates administrator-controlled provisioning for testing only, and updated FAQs to direct builders to the credential management API for customer experiences.

  https://learn.microsoft.com/en-us/entra/external-id/customers/how-to-sign-in-with-passkey