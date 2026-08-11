# Microsoft Defender for Identity
**Date created:** 2026-08-04 UTC  
**Tags:** Administration, Security  

## Moderate Changes

- **Accounts security posture assessments**

  Removed “(Preview)” labels from multiple assessment headings, signaling general availability and maturity. Added anchor IDs to these sections to support reliable deep links. Content and remediation guidance remain unchanged.

  https://learn.microsoft.com/en-us/defender-for-identity/security-posture-assessments/accounts

- **Configure a gMSA directory service account for Defender for Identity**

  Updated gMSA setup guidance to include KDS root key replication timing and a single-DC test method, with a warning not to use it in production. Clarified that the script configures AES128 and AES256 Kerberos encryption and updated the sample to pass the KerberosEncryptionType parameter. These changes improve security clarity and reduce setup errors.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/create-directory-service-account-gmsa