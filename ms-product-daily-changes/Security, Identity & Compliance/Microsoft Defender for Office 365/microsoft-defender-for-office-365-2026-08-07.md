# Microsoft Defender for Office 365
**Change date:** 2026-08-07 UTC  
**Tags:** Administration, AI, Security  

## Major Changes

- **Configure trusted ARC sealers**
  Removed vendor-specific configuration details and tables for ARC sealers (for example, Proofpoint, Mimecast, Barracuda, Sophos, IIJ) and replaced them with vendor-agnostic guidance. Updated examples now use placeholders, and instructions focus on how to identify a vendor’s ARC sealer domain without relying on a vendor table. The IIJ entry was also removed from the enablement table. This shift simplifies guidance, reduces maintenance overhead, and helps organizations apply consistent configuration regardless of vendor.
  https://learn.microsoft.com/en-us/defender-office-365/email-authentication-arc-configure

- **Manage allows and blocks in the Tenant Allow/Block List**
  Updated the scope of Tenant Allow/Block List entries so they apply to messages from both internal and external senders, with notes on handling internal spoofing scenarios. The prior limitation to external senders and the related hybrid exception were removed. This change helps admins reliably apply allow/block decisions across internal and external mail flows.
  https://learn.microsoft.com/en-us/defender-office-365/tenant-allow-block-list-about

- **Zero-hour auto purge (ZAP) in Microsoft Defender for Office 365**
  Rewrote the ZAP behavior description to state that ZAP searches only the last 48 hours of delivered mail. Prior references to campaign-based remediation affecting messages older than 48 hours were removed, and it was clarified that users aren’t notified when ZAP moves a message. This update sets clearer expectations for remediation timelines and user experience.
  https://learn.microsoft.com/en-us/defender-office-365/zero-hour-auto-purge

## Moderate Changes

- **What's new in Microsoft Defender for Office 365**
  The July 2026 note about localized default “Mark as” and notify email templates was added and later removed. Readers should refer to the feature documentation for the current behavior rather than the transient What's New entry.
  https://learn.microsoft.com/en-us/defender-office-365/defender-for-office-365-whats-new

- **Prompt injection protection in Microsoft Defender for Office 365**
  Clarified that prompt injection content in inbound email is detected as part of standard mail flow inspection with no additional configuration required, and refined the wording about plan availability. This helps admins understand licensing applicability and operational behavior.
  https://learn.microsoft.com/en-us/defender-office-365/step-by-step-guides/prompt-injection-protection-defender-for-office-365

- **View and release quarantined messages from shared mailboxes**
  Clarified that automapping is no longer required and reorganized guidance into two access methods: reviewing from quarantine notifications (with prerequisites) and using the End-user Quarantine page with filtering by Recipient. Prerequisites for the notification method were tightened to require Full Access via direct assignment or a cloud-only security group, and it was clarified that the Review link grants access only to the shared mailbox’s quarantined messages.
  https://learn.microsoft.com/en-us/defender-office-365/quarantine-shared-mailbox-messages

- **Admin review for user reported messages**
  Refined guidance on automatic notification localization and its relationship to customized templates, emphasizing customization steps. Clarified that localization does not affect verdicts, classification, or automated investigations, aligning expectations for admins configuring notifications.
  https://learn.microsoft.com/en-us/defender-office-365/submissions-admin-review-user-reported-messages

- **User reported settings**
  Clarified that default admin review outcome and investigation result emails are automatically localized to the recipient’s preferred language for both manual “Mark as and notify” actions and automatic investigations. Customizing the email body or footer overrides the localized default, and the feature comparison table notes this behavior.
  https://learn.microsoft.com/en-us/defender-office-365/submissions-user-reported-messages-custom-mailbox

- **Allow or block email using the Tenant Allow/Block List**
  Clarified domain and subdomain blocking: a block for contoso.com affects only that domain, while *.contoso.com affects only subdomains; use both entries to block both. Reaffirmed support for wildcard syntax across top-level, internal, and email address domains.
  https://learn.microsoft.com/en-us/defender-office-365/tenant-allow-block-list-email-spoof-configure