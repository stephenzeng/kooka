# Microsoft Purview
**Date created:** 2026-08-20 UTC  
**Tags:** Compliance, Guidance, Security  

## Major Changes

- **Data loss prevention policy tips reference**

  Updated the DLP policy tip support matrix to show that Outlook Mobile (iOS and Android) and Outlook for Mac now support policy tips, replacing previous “not supported” status. Separated these clients into distinct entries and clarified that support depends on app version and licensing, with only a subset of conditions and actions available. Added links to a dedicated guide for Outlook on Android, iOS, and macOS to help admins plan and validate client-specific behavior. These updates help administrators set accurate expectations and design consistent DLP experiences across Outlook clients.

  https://learn.microsoft.com/en-us/purview/dlp-policy-tips-reference

## Moderate Changes

- **Detect channel signals with Communication Compliance**

  Clarified Teams shared channels guidance: Communication Compliance policies don’t support modern attachments in shared channels, and shared channel coverage remains automatic without extra configuration. This helps admins understand monitoring limits for certain file types while confirming no additional setup is needed for shared channels.

  https://learn.microsoft.com/en-us/purview/communication-compliance-channels