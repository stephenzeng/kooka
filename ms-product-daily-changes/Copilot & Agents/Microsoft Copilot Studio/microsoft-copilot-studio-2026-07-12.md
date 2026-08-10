# Microsoft Copilot Studio
**Date created:** 2026-07-12 UTC  
**Tags:** Administration, Governance, Security  

## Major Changes

- **Remove sensitive data**
  
  Expanded guidance to cover redaction of context variables from both Live Chat and voice channels, not just voice-captured inputs. Added clear steps to mark context variables as sensitive by defining global variables on the Conversation Start topic with external write access and sensitivity enabled, plus configuration details for Live Chat (workstream matching and display controls) and voice via SIP X-headers. Clarified variable naming rules, what is and isn’t redacted for context variables, and that marking data as sensitive does not prevent Dataverse storage. Updated tables, cross-references, and UI procedures, and refined guidance on Application Insights logging to improve data protection and governance practices.
  
  https://learn.microsoft.com/en-us/microsoft-copilot-studio/voice-sensitive-data