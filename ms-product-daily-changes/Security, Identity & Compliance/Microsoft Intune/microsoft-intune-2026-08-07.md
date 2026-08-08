# Microsoft Intune
**Change date:** 2026-08-07 UTC  
**Tags:** Administration, Security  

## New Articles

- **Reports don't run when RBAC is enabled**

  Introduced a troubleshooting guide for Configuration Manager reports failing under RBAC due to Kerberos or Active Directory permission issues. Explains symptoms and root causes, including missing tokenGroupsGlobalAndUniversal access and encryption type mismatches (KDC_ERR_ETYPE_NOSUPP) related to RC4 deprecation in 2026. Provides step-by-step diagnostics using SCCMReporting.log and prescriptive fixes such as adding the service account to Windows Authorization Access Group, enabling AES for the SSRS service account, rotating passwords to generate AES keys, and monitoring domain controller events.

  https://learn.microsoft.com/en-us/troubleshoot/mem/configmgr/alerts-reports-queries/reports-rbac-cannot-get-usersid

## Moderate Changes

- **Assign Apps to Groups in Microsoft Intune**

  Clarified that most app types support Available assignments only for user groups, with two exceptions where device groups are supported: Win32 apps and Android Enterprise fully managed (COBO) and COPE apps. This reduces ambiguity and helps admins target deployments correctly.

  https://learn.microsoft.com/en-us/intune/app-management/deployment/assign-groups

- **Manually register Microsoft Entra apps**

  Removed the requirement to set oauth2AllowIdTokenImplicitFlow to true in the app manifest for both web (server) and native (client) apps used for CMG registration. This streamlines setup, aligns with current guidance, and reduces unnecessary configuration steps.

  https://learn.microsoft.com/en-us/intune/configmgr/core/clients/manage/cmg/manually-register-azure-ad-apps

- **Use a PKCS certificate profile to provision devices with certificates in Microsoft Intune**

  Added a supportability note that device configuration profiles, including PKCS certificate profiles, aren’t supported on Microsoft Teams devices running AOSP. This helps avoid unsupported deployments and related troubleshooting.

  https://learn.microsoft.com/en-us/intune/device-configuration/certificates/pkcs-profiles

- **Set up automated device enrollment for macOS**

  Added an important warning not to target Platform SSO profiles that enable registration during Setup Assistant to userless ADE devices, as this can cause unexpected enrollment behavior and loss of user affinity. The update points to guidance for configuring Platform SSO correctly during enrollment.

  https://learn.microsoft.com/en-us/intune/device-enrollment/apple/setup-automated-macos

- **What's new in version 2603**

  Expanded guidance on SQL Server Management Objects changes: SQLSysClrTypes.msi and SharedManagementObjects.msi are no longer included in redistributables. After updating to version 2603, admins can safely uninstall these legacy MSI packages because required files are now bundled with Configuration Manager.

  https://learn.microsoft.com/en-us/intune/configmgr/core/plan-design/changes/whats-new-in-version-2603