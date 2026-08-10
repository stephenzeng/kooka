# Microsoft 365 Copilot
**Date created:** 2026-07-22 UTC  
**Tags:** Automation, Governance, Security  

## Major Changes

- **Use Copilot Cowork**

  Expanded task status guidance to include automated tasks, covering both scheduled prompts and new event-driven automations. Introduced detailed setup for event-driven tasks, including triggers from email and Teams messages (with @mentions), run context, and required permissions captured in setup fields. Documented how to manage these tasks on the Scheduled page, with states, last fired time, history, and controls to edit, pause, resume, or delete. Clarified default draft-and-approve behavior, permission scope, rate limits, and how results are delivered.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/use-cowork

## Moderate Changes

- **Manage Copilot Cowork for your organization**

  Added governance guidance for automated tasks, including scheduled and event-driven automations. Clarified that tasks run with the creator’s permissions, require user approval for shared actions (with an option to pre-authorize), and are subject to rate limits, loop protection, and auditing via Microsoft Purview policies.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/cowork-admin-governance

- **Copilot Cowork common questions**

  Expanded the FAQ with references to scheduling prompts and a new entry on event-driven tasks triggered by emails or Teams messages (including @mentions). Explained that actions default to draft-and-approve and run under the user’s permissions, with links to setup guidance.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/cowork-faq

- **Manage plugins for Copilot Cowork**

  Added an important limitation: Microsoft Purview Information Barriers aren’t supported for plugin or skill management and sharing. When IB is enabled, embedded knowledge file uploads are blocked tenant-wide, preventing affected plugins and skills from being uploaded or published.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/cowork-manage-plugins

- **Cowork network endpoints**

  Updated network guidance to bypass SSL/TLS decryption and traffic inspection for Microsoft 365 traffic. SSL/TLS inspection isn’t supported for Cowork traffic to *.gateway.prod.island.powerapps.com:443 and can break long-lived SSE connections, causing delivery failures or frozen tasks, with references to broader Microsoft 365 network guidance.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/cowork-network-endpoints

- **Build plugins for Copilot Cowork**

  Noted that Microsoft Purview Information Barriers aren’t supported for plugin or skill management and sharing. In IB-enabled tenants, embedded knowledge file uploads are blocked, which prevents affected plugins and skills from being uploaded or published.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/cowork-plugin-development

- **What's new in Copilot Cowork**

  Added a July 2026 entry announcing event-driven tasks that let users create trigger-based automations from matching emails or Teams messages (including @mentions). Highlighted that these automations appear alongside scheduled prompts on the Scheduled page, with a link to setup instructions.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/whats-new