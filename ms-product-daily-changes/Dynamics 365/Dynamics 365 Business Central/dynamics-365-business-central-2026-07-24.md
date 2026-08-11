# Dynamics 365 Business Central
**Date created:** 2026-07-24 UTC  
**Tags:** AI, Administration, Agent, Automation  

## Major Changes

- **Use item charges to account for extra trade costs**

  Expanded guidance explains how landed costs flow into inventory value and profitability, including a worked example to help teams allocate charges accurately. Clarified the Item Charge Assignment process and when to use each distribution option (Equally, By Amount, By Weight, By Volume), emphasizing Net Weight and Unit Volume for precise allocation. Documented support for assigning charges across more posted document types and distinguished inventoriable versus non‑inventoriable costs, including where non‑inventoriable amounts are tracked. Added steps to review posted charges via value entries, item ledger entries, and reports, and advised running Adjust Cost when charges are posted after sale to ensure correct COGS; also covered Standard cost treatment as purchase variances.

  https://learn.microsoft.com/en-us/dynamics365/business-central/payables-how-assign-item-charges

- **Set up Sales Order Agent**

  Updated setup guidance clarifies that the agent always creates a sales quote first as a safe step and provides a matrix showing how “Send quotes for confirmation” and “Make orders from quotes” interact. Added a tip to verify customer contact email addresses before activation to improve matching accuracy, and refined option descriptions to show when quotes are sent and when conversions occur. Introduced practical configuration scenarios, including limiting processing to approved senders via mailbox folders and rules, running multiple agent instances for different customer groups, and stopping at quote creation when teams prefer manual pricing or discount adjustments.

  https://learn.microsoft.com/en-us/dynamics365/business-central/sales-order-agent-setup

## Moderate Changes

- **FAQ for Sales Order Agent**

  Added a customer and contact identification section detailing strict email-based matching, behavior with forwarded emails, and limitations when contacts lack email addresses. Removed the constraint that only one Sales Order Agent can be configured per company and clarified extensibility expectations, noting that the agent’s prompt instructions are available in source for review.

  https://learn.microsoft.com/en-us/dynamics365/business-central/faqs-sales-order-taker-agent

- **Sales Order Agent overview**

  Expanded functional guidance on relevance, including examples of non-sales attachments that are ignored, and highlighted that the agent’s prompt rules are available in the extension source. Clarified that the agent creates a quote first by design and how to configure direct order creation, and refined email-based customer identification with security-focused matching, forwarded email behavior, and improved process flow wording.

  https://learn.microsoft.com/en-us/dynamics365/business-central/sales-order-agent

- **Item availability in Sales Order Agent (preview)**

  Clarified that the “Unit Price Including Discount” comes from a temporary sales document that uses Business Central’s pricing engine for the specific customer, date, and quantity, rather than the item’s list price. This helps ensure quotes reflect real pricing rules and discounts.

  https://learn.microsoft.com/en-us/dynamics365/business-central/sales-order-agent-item-availability

- **Process sales quotes and orders with Sales Order Agent**

  Clarified how activation dates control email processing, including behavior on deactivation/reactivation, and that copied or moved older emails are ignored unless the received date is after activation. Noted that forwarding an old email creates a new message attributed to the forwarder, which may require manual customer selection during review, and added links to related setup and testing guidance.

  https://learn.microsoft.com/en-us/dynamics365/business-central/sales-order-agent-process