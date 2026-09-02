# Microsoft Defender for Identity
**Date created:** 2026-09-02 UTC  
**Tags:** Best Practices, Configuration, Guidance, Security  

## Major Changes

- **Deploy Microsoft Defender for Identity sensors**

  Updated deployment guidance to require installing sensors on all domain controllers, including RODCs. Clarified sensor versioning: use v3.x only on domain controllers running Windows Server 2019 or later (with required cumulative updates), and use v2.x on older domain controllers and on non-domain controller identity servers (AD FS, AD CS, Microsoft Entra Connect). Revised selection guidance to remove prior recommendations for v3.x on non-domain controller identity servers and aligned deployment steps accordingly. Removed outdated notes about workspace creation time impacting v2.x availability to simplify planning and reduce misconfiguration risk.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/deploy-defender-identity

## Moderate Changes

- **Install the sensor v2.x | Microsoft Defender for Identity**

  Updated the title and installation guidance to recommend deploying sensor v3.x for domain controllers on Windows Server 2019 or later, activated directly from the Defender portal without a download. Clarifies when to choose v3.x versus v2.x to streamline deployments.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/install-sensor

- **Microsoft Defender for Identity sensor v2.x prerequisites**

  Replaced a workspace-based installation restriction with a tip recommending v3.x on domain controllers running Windows Server 2019 or later. Shifts guidance to clear OS-based version selection for more predictable deployments.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/prerequisites-sensor-version-2

- **What's new | Microsoft Defender for Identity**

  Removed the August 2026 note about “Sensor v2.x installation restriction for new workspaces,” indicating the limitation no longer applies. Keeps the changelog current and removes outdated constraints.

  https://learn.microsoft.com/en-us/defender-for-identity/whats-new