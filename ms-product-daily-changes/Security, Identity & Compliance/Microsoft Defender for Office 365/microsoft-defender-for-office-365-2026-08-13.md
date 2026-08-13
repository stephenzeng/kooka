# Microsoft Defender for Office 365
**Date created:** 2026-08-13 UTC  
**Tags:** Configuration, Guidance, Security, Troubleshooting  

## Major Changes

- **Troubleshoot anti-spam policies in Microsoft Defender for Office 365**
  Shifted troubleshooting from SCL-focused steps to a spam verdict and filtering decision model, clarifying how components like mail flow rules, IP Allow List, allow/block lists, Safe Senders, Tenant Allow/Block List, Advanced delivery, and Enhanced Filtering influence outcomes. Added explicit notes that SCL -1 is only an instruction and that malware and high confidence phishing protections are never bypassed. Expanded SFV value mappings (e.g., SKN, SKS, SKI) and reworked the decision tree to use SFV, CAT, DIR, Authentication-Results, and IPV, with refreshed header examples and actionable admin checks and PowerShell. This improves accuracy when identifying what filtered or bypassed a message and how to remediate.
  https://learn.microsoft.com/en-us/defender-office-365/anti-spam-policies-troubleshooting

- **Spam confidence level (SCL) in Microsoft 365**
  Overhauled guidance to clarify that SCL no longer determines spam verdicts or actions in cloud environments and should not be used for interpreting filtering outcomes. Directs admins to rely on CAT/DIR and policy actions instead, and explains SCL’s current roles: mail flow rule inputs and on-premises Exchange thresholds. Updated troubleshooting pointers align with the verdict-focused model, reducing misdiagnosis and improving resolution accuracy.
  https://learn.microsoft.com/en-us/defender-office-365/anti-spam-spam-confidence-level-scl-about

## Moderate Changes

- **Tune anti-phishing protection**
  Updated guidance on interpreting the X-Forefront-Antispam-Report to use SFV:SKN when transport rules skip spam filtering, replacing older SCL-based examples. This makes it easier to identify when filtering was intentionally bypassed.
  https://learn.microsoft.com/en-us/defender-office-365/anti-phishing-protection-tuning

- **Advanced Spam Filter (ASF) settings in anti-spam policies**
  Clarified that “Increase spam score” settings directly mark matching messages as spam and apply the policy action unless overridden by higher-priority detections. Rewrote outcomes to use verdicts (Spam, High confidence spam) rather than SCL numbers and refined setting descriptions for accuracy. This helps admins understand actual enforcement and precedence.
  https://learn.microsoft.com/en-us/defender-office-365/anti-spam-policies-asf-settings-about

- **Anti-spam protection in cloud organizations**
  Revised verdict descriptions to remove specific SCL thresholds and use “identified as spam” or “identified as high confidence spam” language. Updated guidance on BCL-based bulk handling to describe outcomes by verdicts, aligning with current filtering behavior.
  https://learn.microsoft.com/en-us/defender-office-365/anti-spam-protection-about

- **Configure junk email settings on Exchange Online mailboxes**
  Clarified that Safe Senders informs spam filtering but does not guarantee delivery, and that malware and high confidence phishing detections take precedence. Simplified Outlook Junk Email Filter guidance to focus on SmartScreen behavior separate from Microsoft 365 verdicts. This helps set correct expectations and reduces reliance on legacy SCL concepts.
  https://learn.microsoft.com/en-us/defender-office-365/configure-junk-email-settings-on-exo-mailboxes

- **Configure connection filtering in cloud organizations**
  Added guidance that IP Allow List bypass is treated as an input that can be overridden by Secure by default, so some messages may still be filtered. Clarified that setting SCL to 0 is also just an input and might not return mail to filtering as expected, helping prevent misconfiguration.
  https://learn.microsoft.com/en-us/defender-office-365/connection-filter-policies-configure

- **Create sender blocklists for cloud mailboxes**
  Removed recommendations to use mail flow rules that set SCL=9 and updated Tenant Allow/Block List descriptions to reference the High confidence spam verdict without SCL numbers. This aligns guidance with current verdict-driven enforcement.
  https://learn.microsoft.com/en-us/defender-office-365/create-block-sender-lists-in-office-365

- **Configure trusted ARC sealers**
  Updated ARC troubleshooting to rely on spam verdict/category indicators (CAT:SPM, CAT:HSPM, SFV:SPM) instead of SCL thresholds and refreshed header examples accordingly. This improves diagnosis of ARC-related outcomes and reduces confusion from deprecated SCL cues.
  https://learn.microsoft.com/en-us/defender-office-365/email-authentication-arc-configure

- **Resolve false positives for legitimate blocked emails in Microsoft Defender for Office 365**
  Shifted analysis and remediation to use SFV and CAT indicators rather than SCL, with updated header interpretation and verification steps (e.g., SFV:NSPM, CAT:NONE). Separated bulk (CAT:BULK) from spam/high confidence spam (CAT:SPM/CAT:HSPM) scenarios with targeted actions and clarified that mail flow rules can request, but not guarantee, spam bypass. This streamlines root cause identification and corrective actions.
  https://learn.microsoft.com/en-us/defender-office-365/step-by-step-guides/how-to-handle-false-positives-in-microsoft-defender-for-office-365

- **Anti-spam message headers in cloud organizations**
  Refreshed header reference to clarify SCL’s limited role in cloud and emphasize CAT/DIR for interpreting filtering. Added or expanded SFV entries (SKI for IP Allow List, SKN for transport rules, SKS for hybrid inputs and Secure by default) and updated SRV:BULK to match current behavior. These changes make header analysis more reliable and aligned with today’s filtering pipeline.
  https://learn.microsoft.com/en-us/defender-office-365/message-headers-eop-mdo