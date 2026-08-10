# Microsoft Entra
**Date created:** 2026-07-16 UTC  
**Tags:** Administration, Automation, Governance  

## New Articles

- **Admin Control for SSO prompts**

  Introduced a new enterprise admin control to automatically accept SSO permission prompts on managed Windows devices. Admins can enable a registry policy (HKLM\SOFTWARE\Policies\Microsoft\Windows\AAD\AutoAcceptSsoPermission=1) starting with the July 2026 security update (KB5101650) for Windows 11 versions 24H2 and 25H2. The control applies only to managed Entra ID devices and excludes personal accounts and unmanaged devices. The article details deployment via GPO, Intune/MDM, Configuration Manager, or other registry-capable tools, along with validation steps.

  https://learn.microsoft.com/en-us/entra/identity/devices/sso-admin-control

## Moderate Changes

- **Lifecycle Workflows templates and categories**

  Updated Lifecycle Workflows templates to use the lastSuccessfulSignInDateTime attribute instead of LastSignInDateTime in the “Pre-Offboard inactive users” and “Offboard inactive users” templates. This clarifies the correct event user attribute, improving accuracy for inactivity-based offboarding logic and reporting.

  https://learn.microsoft.com/en-us/entra/id-governance/lifecycle-workflow-templates