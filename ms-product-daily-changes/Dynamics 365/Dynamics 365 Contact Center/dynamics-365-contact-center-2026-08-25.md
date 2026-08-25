# Dynamics 365 Contact Center
**Date created:** 2026-08-25 UTC  
**Tags:** Configuration, Guidance  

## New Articles

- **Configure customer-first direct callback in Dynamics 365 Contact Center**

  Introduced guidance for customer-first direct callback, where the system calls the customer before connecting to a representative to reduce hold time and improve capacity utilization. Clarifies prerequisites and one-way enablement with automatic provisioning of a Callback Agent and an initial profile requirement. Details how to build callback profiles, including offer options, operating-hours awareness, duplicate prevention, dialing choices, and use of a Copilot AI agent with defined fallbacks. Explains retry behavior, callback throttling based on target average wait time, and how to apply a profile to a queue’s overflow action.

  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/configure-customer-first-callback

## Moderate Changes

- **Configure conversation orchestration by using natural language playbooks (preview)**

  Updated availability to indicate support for voice and messaging channels and removed preview wording. Expanded overflow handling with new conditions (wait time in queue and queue position) and added a scenario to retain the same expert for returning asynchronous chats with presence and conversation limit checks. Increased the number of default popular prompts from three to six to streamline setup.

  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/configure-conversation-orchestration