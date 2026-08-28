# Microsoft Defender for Identity
**Date created:** 2026-08-28 UTC  
**Tags:** Monitoring, Security  

## Moderate Changes

- **Microsoft Defender for Identity classic alerts**

  Added a new “Group Policy Tampering” alert that detects suspicious Group Policy changes that disable Microsoft Defender Antivirus. The entry provides investigation guidance (validate legitimacy, revert changes if needed, and review GPO linkage and scope) and maps to MITRE Defense Evasion (TA0005) and Subvert Trust Controls (T1553). This improves coverage of defense evasion techniques with a medium-severity alert (ID 2440).

  https://learn.microsoft.com/en-us/defender-for-identity/alerts-mdi-classic

- **Microsoft Defender for Identity alerts in Microsoft Defender format**

  Streamlined and updated alert definitions: removed four deprecated alerts and revised the “Possible use of a stolen session cookie” alert with a new MITRE mapping and detector ID (xdr_StolenSessionArtifactReplay). Added missing detector IDs to improve clarity and correlation for “Suspicious bulk user deletion via scripted activity” (xdr_SuspiciousBulkUserDeletion) and “Reciprocal Temporary Access Pass creation between users” (xdr_ReciprocalTAPCreationViaGraphAPI).

  https://learn.microsoft.com/en-us/defender-for-identity/alerts-xdr