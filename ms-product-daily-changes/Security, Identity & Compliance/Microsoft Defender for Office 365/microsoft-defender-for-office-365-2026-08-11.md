# Microsoft Defender for Office 365
**Date created:** 2026-08-11 UTC  
**Tags:** Analytics, Best Practices, Configuration, Guidance, Security, Troubleshooting  

## Moderate Changes

- **Safe Attachments in Microsoft Defender for Office 365**

  Added an option to block messages with password-protected attachments when the unknown malware response is set to Block, sending them to quarantine. Clarified how these items are handled, including admin and user release workflows with just-in-time detonation on password submission, supported/unsupported scenarios, attachment-type exclusions, and default quarantine policy behavior. Included best practices and an advanced hunting query to identify messages containing password-protected attachments.

  https://learn.microsoft.com/en-us/defender-office-365/safe-attachments-about

- **Set up Safe Attachments policies in Microsoft Defender for Office 365**

  Introduced configuration to block unscannable, encrypted attachments when the action is Block, with UI controls for enabling the feature, selecting excluded file types, and choosing a quarantine policy. Updated PowerShell guidance with new parameters to manage the feature: -EnableBlockingEncryptedAttachments, -ExcludedTypesFromBlockingEncryptedAttachments, and -QuarantineTagForBlockingEncryptedAttachments.

  https://learn.microsoft.com/en-us/defender-office-365/safe-attachments-policies-configure

- **Configure quarantine policies in cloud organizations**

  Updated Safe Attachments policy mapping to distinguish quarantine policy selection for standard scanning outcomes versus blocked encrypted attachments. Enhanced PowerShell guidance with -EnableBlockingEncryptedAttachments and -QuarantineTagForBlockingEncryptedAttachments and documented default behavior when no specific quarantine tag is set.

  https://learn.microsoft.com/en-us/defender-office-365/quarantine-policies

- **Quarantined email messages in cloud organizations**

  Documented how messages quarantined by Safe Attachments that contain encrypted attachments are retained for 30 days. Clarified release options: admins can release without a password, while users may submit the attachment password for rescanning and potential release, subject to quarantine policy.

  https://learn.microsoft.com/en-us/defender-office-365/quarantine-about

- **Manage quarantined messages and files as an admin**

  Added a new quarantine reason, “Password protected item,” for messages with encrypted attachments that cannot be scanned. Clarified release behavior: admins can release without providing the password, while end users must supply it if they initiate release themselves.

  https://learn.microsoft.com/en-us/defender-office-365/quarantine-admin-manage-messages-files

- **Manage quarantined messages and files as a user**

  Introduced guidance for handling “Password protected item” messages, including entering the attachment password for rescanning, one attempt per prompt, and outcomes after rescanning. Noted that releases can’t be performed from notification emails and must be done in the Defender portal, with security reminders to enter only the attachment password and verify the sender.

  https://learn.microsoft.com/en-us/defender-office-365/quarantine-end-user

- **Configure outbound spam policies for cloud mailboxes**

  Clarified that “Automatic - System-controlled” for automatic forwarding may behave as On or Off depending on the organization, reflecting historical and policy changes. Recommended explicitly selecting On or Off to avoid ambiguity.

  https://learn.microsoft.com/en-us/defender-office-365/outbound-spam-policies-configure

- **Configuring and controlling external email forwarding in Microsoft 365**

  Updated guidance to explain that “Automatic - System-controlled” can act as On or Off based on organizational state. Recommended explicitly setting On or Off for external forwarding to ensure predictable behavior.

  https://learn.microsoft.com/en-us/defender-office-365/outbound-spam-policies-external-email-forwarding

- **Recommended email and collaboration threat policy settings for cloud organizations**

  Expanded recommendations for Safe Attachments to include settings that block encrypted attachments, with defaults across Built-in protection, Standard, and Strict. Updated outbound spam policy guidance by changing the recommended “Automatic forwarding rules” from “Automatic - System-controlled” to “Off,” noting org-dependent behavior and advising explicit configuration.

  https://learn.microsoft.com/en-us/defender-office-365/recommended-settings-for-eop-and-office365