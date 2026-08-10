# Microsoft Entra
**Date created:** 2026-07-17 UTC  
**Tags:** Administration, Security  

## Moderate Changes

- **Microsoft Entra Connect Sync service features**

  Updated examples to include the AdditionalProperties.allowOnPremUpdateOfOnPremisesObjectIdentifierEnabled setting. Clarified hard match enforcement: matching is blocked when the cloud onPremisesObjectIdentifier differs from the incoming on-prem value, with remediation steps to clear the attribute and retry. Added guidance to use the tenant-level bypass flag only temporarily during migration, recovery, or consolidation and to disable it after remediation.

  https://learn.microsoft.com/en-us/entra/identity/hybrid/connect/how-to-connect-syncservice-features