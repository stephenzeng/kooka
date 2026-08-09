# Microsoft Defender for Identity
**Date created:** 2026-08-09 UTC  
**Tags:** Security  

## Moderate Changes

- **Connect CyberArk Identity to Microsoft Defender for Identity (Preview)**

  Clarified OAuth client setup by specifying that users must be added to the Privileged Cloud Auditors role to enable tagging identities as privileged accounts in the Microsoft Defender portal. This ensures administrators have the correct permissions to complete setup and manage privileged tagging reliably.

  https://learn.microsoft.com/en-us/defender-for-identity/connect-cyber-ark

- **Connect SailPoint Identity Security Cloud to Microsoft Defender for Identity (Preview)**

  Updated guidance to clarify integration through the Microsoft Defender portal and highlight investigation benefits. Enhanced prerequisites by specifying the SailPoint IdentityNow Admin role and required Microsoft Entra or Defender XDR permissions, and revised the Personal Access Token workflow to use a dedicated SailPoint user for sign-in. These changes streamline setup and improve clarity on required roles and steps.

  https://learn.microsoft.com/en-us/defender-for-identity/connect-sail-point

- **Microsoft Defender for Identity's security posture assessments**

  Added a dedicated prerequisites section detailing licensing and sensor requirements, with a link to sensor configuration guidance. Clarified the Certificates category by explicitly referencing Active Directory Certificate Services (AD CS) and improved section labeling for easier navigation. These updates help readers verify eligibility and configure sensors before using assessments.

  https://learn.microsoft.com/en-us/defender-for-identity/security-assessment

- **Manage and update Microsoft Defender for Identity sensors**

  Expanded guidance on monitoring sensor status and health, understanding sensor properties, updating v2.x and v3.x sensors, and configuring proxies, including required roles. Clarified migration states with explicit values and in-place upgrade eligibility to reduce confusion during transitions. This improves upgrade planning and day-to-day sensor operations.

  https://learn.microsoft.com/en-us/defender-for-identity/sensor-settings