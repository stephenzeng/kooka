# Microsoft Defender for Office 365
**Date created:** 2026-07-19 UTC  
**Tags:** Security  

## Moderate Changes

- **Anti-phishing policies in cloud organizations**

  Updated impersonation protection scope to cover only users and domains, removing references to brands. This clarifies feature coverage and helps admins set accurate expectations for detection and policy configuration.

  https://learn.microsoft.com/en-us/defender-office-365/anti-phishing-policies-about

- **Microsoft Defender for Office 365 ICES Vendor Ecosystem integration guide**

  Added VIPRE Integrated Email Security (IES) to the list of supported non-Microsoft security vendors and refreshed the FAQ to reflect availability for Darktrace, KnowBe4, and VIPRE Security Group. This expands integration options and clarifies current partner support.

  https://learn.microsoft.com/en-us/defender-office-365/mdo-ices-vendor-ecosystem

- **Allow or block email using the Tenant Allow/Block List**

  Corrected UI guidance to use the “Allow domains & addresses” flyout when creating allow entries and fixed the PowerShell example to use Set-TenantAllowBlockListSpoofItems for spoofed sender changes. These updates reduce configuration errors in the portal and prevent scripting mistakes.

  https://learn.microsoft.com/en-us/defender-office-365/tenant-allow-block-list-email-spoof-configure