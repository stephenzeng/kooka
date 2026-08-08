# Microsoft Defender for Identity
**Change date:** 2026-08-07 UTC  
**Tags:** Administration, Security  

## Moderate Changes

- **Deploy Microsoft Defender for Identity sensors**

  Clarified deployment guidance: environments that require VPN integration or syslog notifications must use the v2.x sensor on applicable domain controllers because these features aren’t supported in v3.x. This helps teams plan sensor selection and avoid feature gaps during deployment or migration.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/deploy-defender-identity

- **Migrate from Advanced Threat Analytics (ATA) to Microsoft Defender for Identity**

  Strengthened lifecycle guidance for ATA, emphasizing end-of-life status, support timelines (Mainstream Support ended January 12, 2021; Extended Support ended January 2026), and the need to migrate to Defender for Identity. Also updated related references to Microsoft Defender XDR.

  https://learn.microsoft.com/en-us/defender-for-identity/migrate-from-ata-overview

- **Migrate from Defender for Identity sensor v2 to sensor v3.x**

  Reworked migration troubleshooting to consolidate reasons, verification steps, and resolutions, focusing on confirming Defender for Endpoint onboarding, service health, device ID presence, and connectivity. Guidance now directs admins to update to the latest versions rather than rely on specific minimums, reiterates Windows Server 2019+ support (with current CUs), and clarifies that migration applies only to domain controllers. This streamlines readiness checks and reduces setup friction.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/migrate-to-sensor-v3

- **Investigate identity password protection**

  Removed the “preview” label for Okta and SaaS app integrations on Password Hygiene and Password Policies, indicating these capabilities are now generally available. This signals production readiness and broader adoption.

  https://learn.microsoft.com/en-us/defender-for-identity/password-protection

- **Microsoft Defender for Identity role groups**

  Clarified which Microsoft Entra roles are eligible to perform Defender for Identity response actions, updating the permissions table to remove ambiguity. This helps administrators assign the correct roles and enforce least-privilege access.

  https://learn.microsoft.com/en-us/defender-for-identity/role-groups

- **Manage and update Microsoft Defender for Identity sensors**

  Added an IMPORTANT note that v3.x sensor updates are delivered via Windows Update as part of normal server OS updates; the per-sensor “Delayed update” option applies only to v2.x. This helps admins align maintenance processes for each sensor version.

  https://learn.microsoft.com/en-us/defender-for-identity/sensor-settings

- **VPN integration | Microsoft Defender for Identity**

  Introduced a new prerequisite requiring at least one connected and healthy v2.x sensor to receive RADIUS accounting events. This ensures VPN integrations function as expected during and after sensor transitions.

  https://learn.microsoft.com/en-us/defender-for-identity/vpn-integration

- **What's new in Microsoft Defender for Identity**

  Refreshed the page by removing prior subsections about Windows Server 2025 migration details and the Sensors page “Not ready for migration” tooltip explanations, while keeping core updates like GA migration notices and SaaS app expansions. This keeps the feed concise and focused on current highlights.

  https://learn.microsoft.com/en-us/defender-for-identity/whats-new