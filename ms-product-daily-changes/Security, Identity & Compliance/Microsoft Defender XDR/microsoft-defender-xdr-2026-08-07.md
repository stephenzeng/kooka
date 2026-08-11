# Microsoft Defender XDR
**Date created:** 2026-08-07 UTC  
**Tags:** Security  

## Moderate Changes

- **Use Microsoft Sentinel functions, saved queries, and custom rules **

  Clarified that the adx() operator isn’t supported when using granular delegated admin privileges (GDAP). Updated guidance recommends using Microsoft Entra B2B authentication as a workaround to ensure queries and automations relying on adx() function as expected.

  https://learn.microsoft.com/en-us/defender-xdr/advanced-hunting-defender-use-custom-rules