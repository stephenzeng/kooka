# Microsoft Defender for Identity
**Date created:** 2026-07-28 UTC  
**Tags:** Administration, Security  

## Major Changes

- **Remediation actions for compromised users in Microsoft Defender for Identity**

  Expanded remediation coverage beyond Microsoft-managed identities to include on-premises Active Directory, Microsoft Entra ID, third-party IdPs (Okta, CyberArk Identity, SailPoint), and connected SaaS apps via Defender for Cloud Apps. Clarified that actions are executed through connectors and are accessible across identity-wide experiences and the action center. Updated the supported actions matrix, adding providers for Disable/Enable, clarifying Revoke session, adding Microsoft Entra support for Force password change, and removing certain Okta-specific actions. Refined the roles and permissions model, adding the SOC Identity Responder role and consolidating guidance for non-Microsoft connectors and supported SaaS apps.

  https://learn.microsoft.com/en-us/defender-for-identity/remediation-actions

## Moderate Changes

- **Account correlation rules in Microsoft Defender for Identity (Preview)**

  Expanded guidance from creating to fully managing account correlation rules with clear procedures to add, edit, and remove rules. Clarified prerequisites, licensing, and role requirements, improved explanations of identifiers and rule purpose, and standardized terminology; also added a settings page screenshot to aid navigation.

  https://learn.microsoft.com/en-us/defender-for-identity/custom-account-correlation-rules

- **Manage related identities and accounts in Microsoft Defender for Identity**

  Added guidance for two correlation methods—manual and rule-based—along with portal navigation steps to configure Account Correlation Rules and a reference to the dedicated rules article. Consolidated naming-convention advice and clarified how to link and unlink accounts to reduce duplication and errors.

  https://learn.microsoft.com/en-us/defender-for-identity/manage-related-identities-accounts

- **Microsoft Defender for Identity role groups**

  Updated the permissions table to include the Microsoft Entra SOC Identity Responder role as eligible for Defender for Identity response actions alongside Security Operator. This clarifies who can execute response actions and helps align operational responsibilities.

  https://learn.microsoft.com/en-us/defender-for-identity/role-groups