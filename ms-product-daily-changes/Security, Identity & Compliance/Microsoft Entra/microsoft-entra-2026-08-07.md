# Microsoft Entra
**Change date:** 2026-08-07 UTC  
**Tags:** Administration, Security  

## New Articles

- **Token Protection deployment guide - Web apps (Preview)**

  Introduced a new deployment guide for enabling Token Protection in Conditional Access for browser-based apps targeting Azure Resource Manager. The article details prerequisites and platform/browser support, and provides step-by-step setup for Windows and macOS, including required SSO browser extensions. It walks through creating a report-only Conditional Access policy, reviewing sign-in logs (including the tokenProtectionStatusDetails field), and using sample Graph and Kusto queries to assess readiness. Guidance is included for moving to enforcement and applying complementary policies to block unknown platforms and require device compliance.

  https://learn.microsoft.com/en-us/entra/identity/conditional-access/deployment-guide-token-protection-web-apps

## Moderate Changes

- **Tutorial - Customize user provisioning attribute-mappings for SaaS applications in Microsoft Entra ID**

  Updated guidance on managing group provisioning: enabling or disabling group sync now occurs on the Scoping filters page for supported apps rather than via Attribute Mapping. Removed an outdated illustrative image to reflect the current experience and reduce confusion.

  https://learn.microsoft.com/en-us/entra/identity/app-provisioning/customize-application-attributes

- **Sign in to an Azure Arc-enabled server using Microsoft Entra ID and Azure Roles Based Access Control**

  Clarified that Microsoft Entra joined Arc-enabled machines are not intended to be joined to other domains. If domain join is required, the article now directs admins to disconnect and use the Entra hybrid join solution to avoid misconfiguration and access issues.

  https://learn.microsoft.com/en-us/entra/identity/devices/howto-arc-sign-in-windows

- **Configure Microsoft Entra Connect for an existing tenant**

  Improved remediation steps by adding the required Import-Module ADSyncTools -MinimumVersion 2.5 for clearing onPremisesObjectIdentifier and replacing raw Graph beta PATCH examples with supported Microsoft Graph PowerShell cmdlets. The article also clarifies that enabling the related feature flag temporarily disables hard match protection and explains how to re-enable it, providing safer and more reliable configuration guidance.

  https://learn.microsoft.com/en-us/entra/identity/hybrid/connect/how-to-connect-install-existing-tenant