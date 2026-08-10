# Microsoft Defender for Identity
**Date created:** 2026-07-16 UTC  
**Tags:** Administration, Security  

## Major Changes

- **Configure Windows event auditing**

  Narrowed automatic Windows event auditing to domain controllers for sensor v3.x, removing automatic auditing coverage for AD CS and Microsoft Entra Connect. Consolidated AD FS guidance to SACL configuration only. Introduced health alerts from the sensor that report the configuration state. Clarified that automatic auditing doesn't apply to v2.x domain controllers or to AD FS, AD CS, and Microsoft Entra Connect servers that aren't domain controllers, directing those scenarios to manual or PowerShell-based setup.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/configure-windows-event-collection

- **Deploy the Defender for Identity sensor v3.x**

  Updated deployment requirements to mandate the Windows Server July 2026 or later cumulative update, replacing a specific KB reference. Simplified RPC auditing by removing manual tagging steps and confirming that, starting with sensor version 3.0.8 (July 2026), RPC auditing is automatically enabled on domain controllers after upgrade. Existing Unified Sensor RPC Audit or Sensor Extended RPC Audit tags can remain without action.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/deploy-sensor-v3

## Moderate Changes

- **Deploy Microsoft Defender for Identity sensors**

  Revised prerequisites for Windows Server 2019+ domain controllers (including those with AD FS, AD CS, or Microsoft Entra Connect roles) to require the July 2026 or later cumulative update. This raises the minimum patch level while keeping the sensor v3.x deployment recommendations unchanged.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/deploy-defender-identity

- **Microsoft Defender for Identity health issues**

  Updated the “Sensor v3.x RPC Audit Misconfigured” issue to reflect that starting with sensor version 3.0.8, RPC auditing is enabled automatically upon upgrade. This removes the need to configure the Unified Sensor RPC Audit tag in supported environments.

  https://learn.microsoft.com/en-us/defender-for-identity/health-alerts

- **Migrate from sensor v2.x to sensor v3.x**

  Raised the prerequisite to the Windows Server July 2026 or later cumulative update, removing the earlier specific KB reference. The requirement is reflected in both the migration checklist and the readiness validation table to ensure environments meet the newer baseline.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/migrate-to-sensor-v3

- **Manage and update sensors**

  Clarified that from sensor version 3.0.8, RPC auditing is enabled automatically during upgrade, and tag-based configuration applies only to earlier v3.x sensors. Also updated prerequisites to require the July 2026 or later cumulative update.

  https://learn.microsoft.com/en-us/defender-for-identity/sensor-settings

- **What's new | Microsoft Defender for Identity**

  Announced general availability of migration from sensor v2.x to v3.x, with a link to the migration guide. Updated RPC auditing guidance to confirm automatic enablement starting with sensor version 3.0.8, eliminating the need to manually apply the Sensor Extended RPC Audit tag.

  https://learn.microsoft.com/en-us/defender-for-identity/whats-new