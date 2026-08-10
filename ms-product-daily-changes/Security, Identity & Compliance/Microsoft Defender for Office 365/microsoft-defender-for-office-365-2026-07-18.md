# Microsoft Defender for Office 365
**Date created:** 2026-07-18 UTC  
**Tags:** Administration, Monitoring, Security  

## Moderate Changes

- **Report false positives or false negatives in automated investigation and response (AIR)**

  Added a prerequisites section to verify permissions and licensing before undoing remediation actions, and reordered the steps accordingly. This streamlines the workflow and reduces errors by making requirements explicit up front.

  https://learn.microsoft.com/en-us/defender-office-365/air-report-false-positives-negatives

- **Configure anti-phishing policies for all cloud mailboxes**

  Emphasized that deleting custom anti-phishing policies or rules is permanent, and clarified that policies and rules must be removed separately to avoid orphaned items. This reduces accidental loss and ensures cleaner policy management.

  https://learn.microsoft.com/en-us/defender-office-365/anti-phishing-policies-eop-configure

- **Login pages in Attack simulation training**

  Corrected the description of the “Use from default” control to reflect that it copies from a built-in login page and updated UI terminology to “Preview login page.” Clarified instructions for creating versus modifying a login page to reduce configuration mistakes.

  https://learn.microsoft.com/en-us/defender-office-365/attack-simulation-training-login-pages

- **Payloads in Attack simulation training**

  Clarified that payload creation occurs on the Tenant payloads tab and added guidance to rename payloads copied from Global payloads to prevent duplicates. These updates make payload management more consistent and error-resistant.

  https://learn.microsoft.com/en-us/defender-office-365/attack-simulation-training-payloads

- **Respond to a compromised connector**

  Added clear steps to confirm connector compromise via suspicious traffic review and audit activity, with alternatives for customers without Explorer. Clarified that guidance targets inbound connectors and specified the relevant PowerShell audit events to track, improving detection and recovery.

  https://learn.microsoft.com/en-us/defender-office-365/connectors-detect-respond-to-compromise

- **Detect and remediate illicit consent grants in Microsoft 365**

  Introduced prerequisites and refined how to search and validate suspicious consent events using Microsoft Purview audit logs. Enhanced PowerShell steps to run the permissions script and export results, and clarified how to determine breach scope, improving the end-to-end remediation flow.

  https://learn.microsoft.com/en-us/defender-office-365/detect-and-remediate-illicit-consent-grants

- **How to use DKIM for email in your custom domain**

  Clarified how to map DKIM selector CNAMEs across multiple domains and explained the impact and options for disabling DKIM. Added DNS provider-specific guidance (for example, Cloudflare proxy settings and Route 53 trailing dots) to prevent DKIM verification failures.

  https://learn.microsoft.com/en-us/defender-office-365/email-authentication-dkim-configure

- **Considerations for integrating non-Microsoft security services with Microsoft 365**

  Clarified integration goals and expanded guidance on Enhanced Filtering for Connectors and ARC, including avoiding double link wrapping and disabling third-party link rewriting. Highlighted security implications of Microsoft Graph API approaches that require broad mailbox access and explained Enhanced Filtering limitations, helping admins weigh trade-offs.

  https://learn.microsoft.com/en-us/defender-office-365/mdo-integrate-security-service

- **Configure and review priority account protection in Microsoft Defender for Office 365**

  Added a prerequisite to connect to Exchange Online PowerShell and identified the exact report views where the Priority account protection filter is available. This improves setup readiness and helps admins find the right insights faster.

  https://learn.microsoft.com/en-us/defender-office-365/priority-accounts-turn-on-priority-account-protection

- **Set up Safe Attachments policies in Microsoft Defender for Office 365**

  Introduced a prerequisite verification step and replaced generic references with direct links to key configuration tasks. Corrected preset policy processing to note that the Strict Preset Security Policy is applied first when assigned, aligning guidance with actual behavior.

  https://learn.microsoft.com/en-us/defender-office-365/safe-attachments-policies-configure

- **Safe Documents in Microsoft 365 A5/E5/G5 or Microsoft Defender Suite**

  Clarified licensing by specifying that users must have a plan including the Office 365 SafeDocs (SAFEDOCS) service plan. This helps admins validate eligibility before enabling the feature.

  https://learn.microsoft.com/en-us/defender-office-365/safe-documents-in-e5-plus-security-about

- **User tags in Microsoft Defender for Office 365**

  Added a warning that deleting a custom user tag is permanent and removes it across assigned users, groups, and related experiences. Clarified that the procedure creates a custom user tag in the Microsoft Defender portal to set expectations.

  https://learn.microsoft.com/en-us/defender-office-365/user-tags-about