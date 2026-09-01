# Microsoft Defender for Identity
**Date created:** 2026-09-01 UTC  
**Tags:** Configuration, Guidance, Security  

## Major Changes

- **Deploy Microsoft Defender for Identity sensors**

  Introduced a restriction for new workspaces: sensor v2.x may be installed only on servers running Windows Server 2016 or earlier. Expanded guidance to install sensor v3.x on Windows Server 2019 or later (with the July 2026 CU) across domain controllers and identity servers such as AD FS, AD CS, and Microsoft Entra Connect that aren’t domain controllers. Updated selection tables and alt-text to clearly map OS versions and server roles to supported sensor versions and clarified mixed-version environments (v3.x on 2019+; v2.x on 2016 or earlier). Aligned deployment steps so admins deploy v3.x where supported and reserve v2.x for legacy OS hosts.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/deploy-defender-identity

- **Install the Microsoft Defender for Identity sensor v2.x**

  Elevated guidance to an IMPORTANT note stating that in new workspaces, sensor v2.x can only be installed on Windows Server 2016 or earlier for all server roles. Clarifies that existing workspaces are not affected and removes the prior tip positioning v3.x recommendations narrowly for 2019+ domain controllers. This helps prevent unsupported installations and directs admins to choose the sensor version based on OS and role.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/install-sensor

- **Microsoft Defender for Identity sensor v2.x prerequisites | Microsoft Defender for Identity**

  Updated prerequisites to replace a tip with an IMPORTANT note that new workspaces may install sensor v2.x only on Windows Server 2016 or earlier across all roles. Confirms existing workspaces are unaffected and codifies this as a supportability constraint for new deployments. Guides admins to verify OS and server role before selecting v2.x to ensure compliant, stable deployments.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/prerequisites-sensor-version-2

## Moderate Changes

- **What's new | Microsoft Defender for Identity**

  Added an August 2026 update noting that for new workspaces, sensor v2.x is limited to Windows Server 2016 or earlier and that existing workspaces remain unaffected. Included a reference to deployment guidance to help admins choose the correct sensor version by OS and role.

  https://learn.microsoft.com/en-us/defender-for-identity/whats-new