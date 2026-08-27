# Microsoft Defender for Office 365
**Date created:** 2026-08-27 UTC  
**Tags:** Configuration, Guidance  

## Moderate Changes

- **User reported settings in Microsoft Teams**

  Clarified that user reporting in Teams works only for users with an online Teams mailbox and that the configured reporting mailbox must be an Exchange Online mailbox. On-premises mailboxes aren't supported for either user reporting or the reporting mailbox. This helps admins avoid unsupported configurations that can break reporting workflows.

  https://learn.microsoft.com/en-us/defender-office-365/submissions-teams

- **User reported settings**

  Updated the “My reporting mailbox only” option to specify that you cannot use distribution groups or route to external or on-premises mailboxes; only a single Exchange Online mailbox is allowed. This reduces misconfiguration risk and ensures reported messages are delivered to a supported destination.

  https://learn.microsoft.com/en-us/defender-office-365/submissions-user-reported-messages-custom-mailbox