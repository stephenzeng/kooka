# Microsoft Defender for Identity
**Date created:** 2026-07-31 UTC  
**Tags:** Security  

## Major Changes

- **Microsoft Defender for Identity alerts in Microsoft Defender format**

  Added a broad set of new XDR alert entries spanning credential access/identity theft, impact/disruption, persistence, and AD CS abuse scenarios. Coverage includes attempts such as AADInternals private key extraction, malicious MFA device registration or method changes on high‑risk accounts, DPAPI master key requests, and organization branding changes by newly created users. It also adds alerts for persistence via strong MFA device registration and a potential Certighost (CVE-2026-54121) AD CS abuse path. Each alert includes severity, MITRE ATT&CK mappings, and detector IDs to improve triage, threat hunting, and response prioritization.

  https://learn.microsoft.com/en-us/defender-for-identity/alerts-xdr

- **Cloud identity assessments in Microsoft Defender for Identity**

  Expanded coverage beyond Okta to include CyberArk Identity and SailPoint Identity Security Cloud, with prerequisites and connection guidance for each. Introduced new assessments aligned to Microsoft Secure Score that target privileged access hygiene, including enforcing MFA for privileged accounts, reducing excessive role assignments, rotating aging passwords, and removing dormant or stale privileged identities. Consolidated guidance focuses on identifying exposed entities and enforcing least privilege across platforms to strengthen identity posture and reduce attack paths.

  https://learn.microsoft.com/en-us/defender-for-identity/security-posture-assessments/cloud-identities