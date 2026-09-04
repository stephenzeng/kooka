# Microsoft Defender for Identity
**Date created:** 2026-09-04 UTC  
**Tags:** Configuration, Guidance, Troubleshooting  

## Major Changes

- **Activate the Microsoft Defender for Identity sensor v3.x**

  Expanded activation guidance beyond domain controllers to include eligible AD FS, AD CS, and Microsoft Entra Connect servers, currently in preview. Clarified the Activation page to show v3.x eligibility and available actions, and updated state table terminology and actions. Added instructions for enabling automatic activation for eligible domain controllers via Advanced features, noting requirements (Defender for Endpoint onboarding) and exclusions (not for non-DC servers or v2.x-to-v3.x migration). Refined steps and messaging around activation timing and confirmed no server restart is required.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/activate-sensor

- **Deploy the Defender for Identity sensor v3.x**

  Extended deployment to non-domain controller identity-role servers (AD FS, AD CS, and Microsoft Entra Connect) as a preview capability. Documented constraints: manual activation and automatic Windows event auditing are supported, while automatic activation and migration are not yet available; at least one v3.x sensor must run on a domain controller if deploying only to these servers. Updated performance and capacity guidance, including v3.x resource caps (CPU 30%, memory 1.5 GB) and generalized recommendations from domain controllers to servers. Clarified DSA/gMSA handling in mixed v2.x/v3.x environments and recommended removing those accounts after full v3.x migration, and reinforced time synchronization across all servers.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/deploy-sensor-v3

## Moderate Changes

- **Configure sensors for AD FS, AD CS, and Microsoft Entra Connect | Microsoft Defender for Identity**

  Updated guidance to reflect that deploying sensor v3.x on AD FS, AD CS, and Microsoft Entra Connect servers that aren't domain controllers is in preview. Clarified version selection: use v3.x on eligible Windows Server 2019+ servers, and follow v2.x procedures for supported Windows Server 2016 or earlier.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/active-directory-federation-services

- **Migrate from sensor v2.x to sensor v3.x**

  Clarified that migration to v3.x is not yet supported for AD FS, AD CS, or Microsoft Entra Connect servers that aren't domain controllers, with support planned for a future update. Updated prerequisites to explicitly allow domain controllers that also host these roles.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/migrate-to-sensor-v3

- **Manage and Update Sensors**

  Revised migration eligibility to include domain controllers that also run AD FS, AD CS, or Microsoft Entra Connect, removing the prior restriction on in-place migration for these scenarios.

  https://learn.microsoft.com/en-us/defender-for-identity/sensor-settings

- **Troubleshooting known issues**

  Expanded the “Auditing health alerts persist on sensor v3.x” guidance to list specific alerts, explain typical causes when auditing is configured manually, and confirm no impact on sensor health or detections. Added a clear resolution path in the Defender portal (Settings > Identities > Advanced features) to enable Automatic Windows auditing configuration and noted a fix is planned in a future sensor update.

  https://learn.microsoft.com/en-us/defender-for-identity/troubleshooting-known-issues