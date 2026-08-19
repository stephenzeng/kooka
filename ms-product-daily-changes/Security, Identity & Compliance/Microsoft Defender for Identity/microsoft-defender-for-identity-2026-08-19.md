# Microsoft Defender for Identity
**Date created:** 2026-08-19 UTC  
**Tags:** Best Practices, Governance, Guidance, Security  

## Major Changes

- **Accounts security posture assessments**
  
  Added three new security posture assessments covering: removal or time-bounding of privileged access for external and guest accounts; elimination of non-admin WriteDACL permissions on sensitive groups; and correction of service accounts holding Domain Admin or Global Admin roles. These additions help reduce lateral movement paths and privilege escalation risks by enforcing least privilege and tighter permission boundaries. The guidance includes clear user impact notes and step-by-step remediation actions to accelerate mitigation and strengthen identity governance.
  
  https://learn.microsoft.com/en-us/defender-for-identity/security-posture-assessments/accounts

## Moderate Changes

- **Microsoft Defender for Identity classic security alerts**
  
  Updated guidance clarifies that some vulnerability-related alerts may still trigger after systems are patched, with severity lowered to Low when all affected assets are updated (where patch status is shown in evidence). Multiple CVE-specific alerts were revised to reflect conditional severity based on patch status, improving triage and helping teams prioritize true exposures over residual patterns.
  
  https://learn.microsoft.com/en-us/defender-for-identity/alerts-mdi-classic

- **Remediate hybrid security posture assessments in Defender for Identity**
  
  Added an assessment to detect and remediate privileged SaaS application accounts that exist outside identity provider control. The guidance directs teams to migrate privileged access to IdP-managed identities and enforce SSO, MFA, Conditional Access, and lifecycle governance to close control gaps and reduce bypass risks.
  
  https://learn.microsoft.com/en-us/defender-for-identity/security-posture-assessments/hybrid-security