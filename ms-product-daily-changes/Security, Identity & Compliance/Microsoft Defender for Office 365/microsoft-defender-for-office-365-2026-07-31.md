# Microsoft Defender for Office 365
**Date created:** 2026-07-31 UTC  
**Tags:** Administration, Security  

## Major Changes

- **Configure trusted ARC sealers**

  Simplified ARC sealer configuration by removing vendor-specific tables and step-by-step instructions, replacing them with a vendor-agnostic approach. Guidance now focuses on identifying the ARC sealer domain from message headers (the d= value) instead of relying on predefined vendor lists. This reduces complexity, avoids stale instructions, and helps administrators configure ARC using consistent, environment-derived details.

  https://learn.microsoft.com/en-us/defender-office-365/email-authentication-arc-configure

## Moderate Changes

- **Configure the advanced delivery policy for non-Microsoft phishing simulations and email delivery to SecOps mailboxes**

  Clarified configuration requirements for Advanced Delivery: it only applies to messages that traverse the Exchange transport pipeline. Direct Injection emails that bypass transport are excluded, helping prevent misconfiguration of third‑party phishing simulations and ensuring accurate policy expectations.

  https://learn.microsoft.com/en-us/defender-office-365/advanced-delivery-policy-configure

- **Attack simulation training deployment considerations and FAQ**

  Updated guidance on region-aware delivery introduces a “not before” model so each recipient receives the simulation at the scheduled local time in their mailbox time zone; if that time has already passed on launch day, delivery occurs at the same local time the following day. Delivery is throttled and occurs in batches, so large simulations complete progressively over a longer window.

  https://learn.microsoft.com/en-us/defender-office-365/attack-simulation-training-faq