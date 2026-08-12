# Microsoft Defender for Identity
**Date created:** 2026-08-12 UTC  
**Tags:** Best Practices, Configuration, Guidance, Identity, Monitoring, Security, Troubleshooting  

## Major Changes

- **Configure Windows event auditing**

  Expanded automatic Windows auditing for sensor v3.x beyond domain controllers to include AD FS, AD CS, and Microsoft Entra Connect servers, with new portal-based enablement steps. Clarified exactly what automatic auditing configures per role, noted required manual AD FS settings, and refined guidance for directory services auditing. Documented PowerShell usage for Get-MDIConfiguration and Set-MDIConfiguration with parameters and examples. Introduced a troubleshooting workflow and a read-only script (Find-MdiAuditingGpoConflicts.ps1) to detect and remediate GPO conflicts that revert required auditing.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/configure-windows-event-collection

- **What's new | Microsoft Defender for Identity**

  Added an August 2026 update covering a new health alert for auditing being reverted by conflicting policies, a read-only script to find GPO conflicts, support for deploying sensor v3.x on AD FS/AD CS/Microsoft Entra Connect servers (including non-DCs), and expanded automatic Windows event auditing for these roles. Also updated the July 2026 notes with a sensor v2.x update entry adding an ETW provider and other improvements before the v2-to-v3 migration GA note.

  https://learn.microsoft.com/en-us/defender-for-identity/whats-new

## Moderate Changes

- **Activate the Defender for Identity sensor v3.x on a domain controller**

  Updated activation guidance to deploy sensor v3.x on all Windows Server 2019+ servers, including AD FS, AD CS, and Microsoft Entra Connect servers, whether or not they are domain controllers. Limited v2.x recommendations to domain controllers on older operating systems and removed prior direction to use v2.x for non-DC identity servers.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/activate-sensor

- **Configure sensors for AD FS, AD CS, and Microsoft Entra Connect | Microsoft Defender for Identity**

  Revised the TIP to recommend sensor v3.x on Windows Server 2019+ regardless of domain controller status. Clarified that the detailed procedures in this article apply to sensor v2.x.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/active-directory-federation-services

- **Security alerts**

  Clarified differences between classic and Defender-format alerts during the transition: alert format depends on detection source and is not tied to sensor version, and some detections may appear in both lists under different names. Explained that tuning is format-specific—use Excluded entities for Defender for Identity detections and alert tuning rules in Microsoft Defender for Defender-format alerts.

  https://learn.microsoft.com/en-us/defender-for-identity/alerts-overview

- **Connect to the Defender for Identity service | Microsoft Defender for Identity**

  Added CLI-based steps to configure or clear an authenticated proxy using Microsoft.Tri.Sensor.Deployment.Deployer.exe, including parameters for ProxyUrl, ProxyUserName, and ProxyUserPassword. Clarified that SSL inspection is unsupported due to mutual certificate authentication and advised testing connectivity after configuration.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/configure-proxy

- **Microsoft Defender for Identity deployment overview**

  Updated deployment requirements to install sensors on all domain controllers (including RODCs) and on AD FS, AD CS, and Microsoft Entra Connect servers, regardless of DC status. Clarified the sensor selection matrix: use v3.x on Windows Server 2019+ and v2.x on Windows Server 2016 or earlier, with steps adjusted accordingly.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/deploy-defender-identity

- **Deploy the Defender for Identity sensor v3.x**

  Stated that v3.x supports AD FS, AD CS, and Microsoft Entra Connect servers even when they are not domain controllers, and required at least one v3.x sensor on a domain controller if deploying only to these roles. Clarified DSA/gMSA credential validation in mixed v2/v3 environments and refined post-activation guidance.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/deploy-sensor-v3

- **Detection exclusions in Microsoft Defender XDR**

  Warned that as detections migrate to the Microsoft Defender XDR engine, existing Defender for Identity exclusions do not carry over and previously suppressed alerts may reappear. Guided admins to recreate equivalent tuning using alert tuning rules and noted that deleting an exclusion takes immediate effect.

  https://learn.microsoft.com/en-us/defender-for-identity/exclusions

- **Microsoft Defender for Identity health issues**

  Added a new health issue for v3.x sensors indicating auditing is being reverted on a domain controller, typically by GPO or local policy. Provided remediation steps to keep automatic auditing enabled, use the GPO conflict script, align or unlink conflicting GPOs, run gpupdate, and verify stability.

  https://learn.microsoft.com/en-us/defender-for-identity/health-alerts

- **Connect Okta to Microsoft Defender for Identity (Preview)**

  Instructed creating a custom Okta role named “Microsoft Defender for Identity” for ongoing API access and clarified role assignment flow, including when to remove Super Admin. Tightened prerequisites and added a clear directive to configure the Okta connector in the Microsoft Defender portal.

  https://learn.microsoft.com/en-us/defender-for-identity/okta-integration

- **Microsoft Defender for Identity sensor v2.x prerequisites**

  Broadened the TIP to recommend deploying sensor v3.x on all Windows Server 2019+ servers, not just domain controllers. Positions v2.x for older operating systems.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/prerequisites-sensor-version-2