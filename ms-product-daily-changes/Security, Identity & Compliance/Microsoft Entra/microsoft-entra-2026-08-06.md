# Microsoft Entra
**Date created:** 2026-08-06 UTC  
**Tags:** Administration, Governance, Security  

## Major Changes

- **Configure dynamic membership groups with the memberOf operator in the Entra Admin Center (preview)**

  Announced the end of the public preview for the memberOf operator and warned that after November 3, 2026, configurations using it will stop updating, risking stale access and policy enforcement gaps. Added a comprehensive migration guide to find and replace memberOf usage across dynamic groups, dynamic administrative units, and entitlement management auto-assignment policies. Recommended moving to supported operators or converting to assigned membership, then validating memberships and cleaning up unused resources. The change also explains the rationale, citing observed performance impact during the preview.

  https://learn.microsoft.com/en-us/entra/identity/users/groups-dynamic-rule-member-of

## Moderate Changes

- **Choose a telephony provider for SMS and voice authentication**

  Rebranded the capability as “Choose Your Own Telephony Provider” and clarified the operating model: Microsoft Entra ID enforces policies while your selected provider sends SMS/voice. Updated availability timelines and streamlined planning guidance to help compare providers and focus on production-ready deployment steps.

  https://learn.microsoft.com/en-us/entra/identity/authentication/concept-phone-providers

- **Configure an automatic assignment policy for an access package in entitlement management**

  Updated the enforcement date for the end of the memberOf rule operator preview to November 3, 2026. This timeline change helps admins plan migrations away from memberOf in automatic assignment policies before updates stop.

  https://learn.microsoft.com/en-us/entra/id-governance/entitlement-management-access-package-auto-assignment-policy

- **Configure Snowflake for Single sign-on with Microsoft Entra ID**

  Clarified prerequisites and administrator roles, confirmed support for both SP- and IdP-initiated SAML SSO, and noted additional options like OIDC, Workload Identity Federation, and OAuth (beyond this article’s scope). Added a troubleshooting reference for SAML error codes to speed issue resolution during testing.

  https://learn.microsoft.com/en-us/entra/identity/saas-apps/snowflake-tutorial