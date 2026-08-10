# Microsoft Entra
**Date created:** 2026-08-10 UTC  
**Tags:** Configuration, Guidance, Security  

## Moderate Changes

- **Configure Microsoft Entra Connect for an existing tenant**
  
  Updated PowerShell guidance for managing the allowOnPremUpdateOfOnPremisesObjectIdentifierEnabled feature flag. The article now uses a consistent $OnPremSync variable, adds explicit steps to enable a temporary bypass and verify the current value, and includes a clear rollback example to set the flag to $false. Command examples were refined with parameter ordering and line continuations to improve readability and reduce errors.
  
  https://learn.microsoft.com/en-us/entra/identity/hybrid/connect/how-to-connect-install-existing-tenant