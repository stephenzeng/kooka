# Microsoft Defender for Identity
**Date created:** 2026-08-25 UTC  
**Tags:** Configuration, Guidance, Monitoring, Security  

## Major Changes

- **Configure Windows event auditing**

  Expanded automatic Windows event auditing for Defender for Identity sensor v3.x to include AD FS, AD CS, and Microsoft Entra Connect servers, not just domain controllers. Updated guidance recommends enabling automatic auditing for all v3.x sensors, with changes applied via local system policy and re-applied every 24 hours. Key automation includes AD FS object-level SACL auditing and advanced audit policies, AD CS auditing via CA audit filter updates (requires certsvc restart), and Audit Logon policy on Entra Connect servers; some AD FS settings still require manual configuration. Clarified that automatic auditing is supported only on v3.x, while v2.x or opted-out scenarios should use the manual procedure.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/configure-windows-event-collection

## Moderate Changes

- **Deploy the Defender for Identity sensor v3.x**

  Updated auditing guidance so the “enable automatic auditing” step now applies to all v3.x sensors, not only domain controllers. This broadens coverage and reduces manual steps for non-domain controller servers.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/deploy-sensor-v3

- **What's new in Microsoft Defender for Identity**

  Added an August 2026 entry announcing expanded automatic Windows event auditing for v3.x sensors to include AD FS, AD CS, and Microsoft Entra Connect servers. The note clarifies that eligible non-domain controller servers are configured automatically and links to the configuration guidance.

  https://learn.microsoft.com/en-us/defender-for-identity/whats-new