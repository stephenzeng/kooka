# Microsoft Defender for Cloud Apps
**Date created:** 2026-08-12 UTC  
**Tags:** Compliance, Configuration, Governance, Guidance, Security  

## Moderate Changes

- **View and regulate OAuth app access to sensitive content with app governance | Microsoft Defender for Cloud Apps**

  Clarified how to review OAuth app access details and sensitivity label exposure across SharePoint, OneDrive, and Exchange Online, including how 30-day label access counts are calculated. Updated policy guidance to explain the built-in Access to sensitive data alert and how to customize it, including disabling apps and scoping inclusions/exclusions. Added instructions for creating custom policies using the Sensitivity labels accessed condition combined with other criteria.

  https://learn.microsoft.com/en-us/defender-cloud-apps/app-governance-visibility-insights-sensitive-content

- **Create policies to control OAuth apps**

  Added clearer guidance on using app permission policies to investigate requested permissions and approve or ban usage, noting that banning disables the associated enterprise application. Clarified that alerts fire only for apps authorized by users in the tenant and refined use of the Community use filter to evaluate requests.

  https://learn.microsoft.com/en-us/defender-cloud-apps/app-permission-policy

- **Commonly used information protection policies | Microsoft Defender for Cloud Apps**

  Expanded scenarios and procedures for both file and session policies, with step-by-step instructions to select sensitivity labels and configure governance actions. Emphasized using the Data Classification Service as the inspection method and clarified detection approaches for external sharing, confidential data, and GDPR-related data.

  https://learn.microsoft.com/en-us/defender-cloud-apps/policies-information-protection

- **Common threat protection policies | Microsoft Defender for Cloud Apps**

  Clarified detection descriptions for unfamiliar locations and impossible travel to better explain what each identifies. Expanded the unpaid leave policy to detail automated governance responses, clarified ransomware detection scope, and enhanced malware guidance with Microsoft Threat Intelligence indicators.

  https://learn.microsoft.com/en-us/defender-cloud-apps/policies-threat-protection

- **Protect your Salesforce environment | Microsoft Defender for Cloud Apps**

  Streamlined setup guidance by removing outdated prerequisites for a Salesforce Connected App and clarifying that SSPM does not require Salesforce Shield. Added clearer lead-ins for configuration and event manager steps and refined prerequisites and structure without changing the sequence.

  https://learn.microsoft.com/en-us/defender-cloud-apps/protect-salesforce

- **Deploy conditional access app control for any web app using AD FS**

  Refined prerequisites to explicitly require an AD FS environment, the appropriate license, and SAML 2.0. Corrected configuration to use the AD FS SingleSignOnService Location from federation metadata for the Single sign-on service URL and clarified which values to capture during external configuration.

  https://learn.microsoft.com/en-us/defender-cloud-apps/proxy-idp-adfs