# Microsoft Defender for Identity
**Date created:** 2026-07-15 UTC  
**Tags:** Security  

## Major Changes

- **Configure Windows event auditing**

  Expanded automatic Windows event auditing to cover more identity role servers and clarified configuration behavior. The update adds object-level SACL configuration for AD FS and enables the local Audit Application Generated policy, while noting other AD FS settings remain manual. It introduces automatic coverage for AD CS (updates CA audit filter via registry and requires restarting the Certificate Services) and Microsoft Entra Connect (enables Audit Logon). Guidance now specifies support for domain controllers and AD FS/AD CS/Entra Connect servers running Defender for Identity sensor v3.x, and removes prior references to health alerts about configuration state.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/configure-windows-event-collection

## Moderate Changes

- **What's new in Microsoft Defender for Identity**

  Added a July 2026 entry highlighting expanded automatic Windows event auditing for identity role servers, including AD FS, AD CS, and Microsoft Entra Connect. The note clarifies applicability to domain controllers running Defender for Identity sensor v3.x and links to configuration guidance.

  https://learn.microsoft.com/en-us/defender-for-identity/whats-new