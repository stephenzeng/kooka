# Microsoft Defender for Identity
**Date created:** 2026-08-13 UTC  
**Tags:** Configuration, Deprecation, Guidance, Monitoring, Security, Troubleshooting  

## Major Changes

- **Configure Windows event auditing**

  Re-scoped automatic Windows auditing to apply only to domain controllers running sensor v3.x. Non-domain controller AD FS, AD CS, and Microsoft Entra Connect servers, as well as any v2.x deployments, now require manual auditing configuration. Removed automatic auditing steps for AD CS and Entra Connect and simplified AD FS guidance to SACL changes; noted that health alerts reflect configuration state and that changes affect only the DC’s local policy. Updated manual configuration steps for non-DC role servers and removed the “Find GPO conflicts” troubleshooting section and its PowerShell script.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/configure-windows-event-collection

## Moderate Changes

- **Activate the Defender for Identity sensor v3.x on a domain controller**

  Clarified that v3.x sensor activation is supported only on domain controllers running Windows Server 2019 or later, including DCs that also host AD FS, AD CS, or Microsoft Entra Connect roles. Directed non-domain controller role servers and domain controllers on older OS versions to use the v2.x sensor.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/activate-sensor

- **Configure sensors for AD FS, AD CS, and Microsoft Entra Connect | Microsoft Defender for Identity**

  Updated guidance to recommend sensor v3.x only when the role runs on a domain controller with Windows Server 2019 or later. Clarified that this article applies to servers that are not domain controllers.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/active-directory-federation-services

- **Microsoft Defender for Identity deployment overview**

  Refined deployment guidance to install sensors on all domain controllers, and to use the v2.x sensor on non-domain controller AD FS, AD CS, and Microsoft Entra Connect servers. Updated the support matrix to remove v3.x for non-DC servers and clarified mixed environments: use v3.x on Windows Server 2019+ DCs and v2.x on older DCs and non-DC role servers.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/deploy-defender-identity

- **Deploy the Defender for Identity sensor v3.x**

  Clarified that v3.x supports domain controllers, including those hosting AD FS, AD CS, or Microsoft Entra Connect roles. Removed the prior requirement to add another v3.x sensor on a DC when deploying only on role servers and advised using v2.x for non-domain controller role servers.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/deploy-sensor-v3

- **Microsoft Defender for Identity health issues**

  Removed the v3.x health issue entry about auditing configuration being reverted on a domain controller, including prior recommendations and references to the diagnostic script.

  https://learn.microsoft.com/en-us/defender-for-identity/health-alerts

- **Microsoft Defender for Identity sensor v2.x prerequisites**

  Narrowed the recommendation so that v3.x is advised specifically for domain controllers running Windows Server 2019 or later, rather than all servers on those versions.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/prerequisites-sensor-version-2

- **What's new | Microsoft Defender for Identity**

  Removed the August 2026 section, including the entry about a new health alert for reverted auditing configuration and the read-only Find-MdiAuditingGpoConflicts.ps1 script. Also removed prior sections describing v3.x support for AD FS/AD CS/Microsoft Entra Connect servers and expanded automatic auditing for these roles. These changes align guidance to use v3.x only on domain controllers and eliminate references to automatic auditing on non-DC role servers.

  https://learn.microsoft.com/en-us/defender-for-identity/whats-new