# Microsoft Defender for Endpoint
**Date created:** 2026-08-04 UTC  
**Tags:** Administration, Automation, Security  

## Moderate Changes

- **Manage endpoint security policies in Microsoft Defender for Endpoint**

  Clarified support limitations for endpoint security policy management on devices using the Microsoft Monitoring Agent (MMA) sensor, with guidance to upgrade using the Defender deployment tool. Also specified that only the Microsoft Defender Antivirus policy is supported on Windows 7 SP1 and Windows Server 2008 R2 SP1, helping admins avoid unsupported configurations.

  https://learn.microsoft.com/en-us/defender-endpoint/endpoint-security-policies-configure

- **Take response actions on a device**

  Added guidance for excluding specific devices from automatic device isolation using policy applications and device tags, including configuration steps. Documented that the Isolate device action shows a Skipped status in Action center for excluded devices and advised temporarily excluding isolation during breach and attack simulations to prevent unintended disruptions.

  https://learn.microsoft.com/en-us/defender-endpoint/respond-machine-alerts