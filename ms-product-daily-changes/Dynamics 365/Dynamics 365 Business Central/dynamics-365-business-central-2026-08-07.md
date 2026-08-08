# Dynamics 365 Business Central
**Change date:** 2026-08-07 UTC  
**Tags:** AI, Administration, Agent, Automation  

## New Articles

- **Manage known senders for Payables Agent**

  Introduced a new article on the known senders feature that maintains a sender list with per-sender policies (Ask, Approve, Reject) to control invoice email processing. It clarifies how policies are applied based on the Email review setting and whether a monitored subfolder is used, ensuring predictable handling of trusted and unwanted senders. The guidance includes steps to access the list, add senders, and update or remove policies, along with defaults for new senders under different review configurations and best-practice recommendations. This helps administrators tighten governance, reduce false positives, and streamline payables intake.

  https://learn.microsoft.com/en-us/dynamics365/business-central/payables-agent-known-senders

## Major Changes

- **Set up Payables Agent**

  Reorganized the setup guide into clear tabbed sections, including a dedicated “Monitor incoming information” tab to configure the mailbox and optional subfolder the agent watches. Expanded the Document processing guidance with granular Email review modes—Manage per sender (recommended), Never, and Always—and clarified behaviors for authenticated internal senders and subfolder handling. Added integrated management of known senders with a direct link to the new configuration page, and streamlined the “Get sample invoices” guidance for evaluation companies. These updates improve discoverability, strengthen governance over incoming emails, and make initial setup and evaluation faster and more reliable.

  https://learn.microsoft.com/en-us/dynamics365/business-central/payables-agent-setup