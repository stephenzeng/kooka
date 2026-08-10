# Dynamics 365 Business Central
**Date created:** 2026-07-18 UTC  
**Tags:** Administration, Agent, AI, Automation, Other  

## Major Changes

- **Sales Order Agent overview**
  Expanded capabilities now let the agent create either a sales quote or a sales order and explicitly perform inventory checks. Introduced a relevance validation model that filters out out-of-scope or risky messages and attachments, with telemetry tracking for filtered content, and reaffirmed that designated users must review and approve outgoing messages. Added a new path when no contact is found, offering options to create a contact, use another contact one time, or update an existing contact’s email. Enhanced item discovery with layered matching (exact IDs, AI-based semantic attributes, and fuzzy search) across defined tables, noting that results depend on product data quality.
  https://learn.microsoft.com/en-us/dynamics365/business-central/sales-order-agent

- **Set up Sales Order Agent**
  Added support for multiple agent instances per company, each with its own mailbox, folder, rules, signature, and metrics. Reorganized setup to include language/region/time zone, refined email monitoring (explicit mailbox and folder, optional subfolder, mark-as-read), and a new “Send quotes for confirmation” option that interacts with review and order creation settings. Improved attachment handling guidance (formats, limits, and surfaced reasons for skipped files), switched to periodic mailbox monitoring, and added a “Try it out” mode to generate tasks without sending emails. Included best practices for testing with real emails, updated Copilot credits guidance, and renamed the permission set to “SOA - EDIT.”
  https://learn.microsoft.com/en-us/dynamics365/business-central/sales-order-agent-setup

## Moderate Changes

- **Process sales quotes and orders with Sales Order Agent**
  Updated email processing so the agent handles all emails in the configured folder from the activation date, tags processed emails to prevent reprocessing, and can optionally mark emails as read. Clarified outcomes when stopping tasks and refined the KPI overview to emphasize actionable insights.
  https://learn.microsoft.com/en-us/dynamics365/business-central/sales-order-agent-process

- **Reverse and correct production order transactions**
  Added step-by-step guidance to manually reverse output via the Output Journal, including setting Applies-To Entry to back out related capacity and item ledger entries. Clarified that the system posts these entries as positive adjustments, ensuring accurate inventory and cost corrections.
  https://learn.microsoft.com/en-us/dynamics365/business-central/production-cancel-production-orders-that-have-consumption

- **Setting up manufacturing**
  Noted that manufacturing features require the Premium experience and provided a link to enable it. This helps admins ensure the correct licensing and experience are in place before configuring manufacturing.
  https://learn.microsoft.com/en-us/dynamics365/business-central/production-configure-production-processes

- **Create production orders**
  Rewrote the introduction to define production orders and their components and clarified differences between automatically planned and manually created orders. This improves understanding of planning context and setup requirements before creation.
  https://learn.microsoft.com/en-us/dynamics365/business-central/production-how-to-create-production-orders

- **Batch post consumption**
  Expanded the introduction to explain what posting consumption does and when automatic flushing or warehouse activities apply. Added guidance on using the consumption journal to enter or calculate usage across multiple production lines for accurate costing.
  https://learn.microsoft.com/en-us/dynamics365/business-central/production-how-to-post-consumption

- **Batch post output and run times**
  Clarified that posting output records completed quantities, setup and run times, updates progress and capacity ledger entries, and for final operations, updates finished-goods inventory. Highlighted using the output journal to register results for multiple released orders to streamline execution tracking.
  https://learn.microsoft.com/en-us/dynamics365/business-central/production-how-to-post-output-quantity

- **Set up work centers and machine centers**
  Expanded definitions of work and machine centers and how calendars, capacity, efficiency, and costs shape scheduling and costing. Added guidance on using work center groups and identifying capacity-constrained resources, and refined the capacity hierarchy for clearer planning decisions.
  https://learn.microsoft.com/en-us/dynamics365/business-central/production-how-to-set-up-work-and-machine-centers

- **View Load on Work and Machine Centers**
  Revised the introduction to emphasize comparing available capacity to load, identifying bottlenecks or underutilization, and applying finite capacity scheduling where needed. Connected these insights to planned and released orders, potential delays, and the Work Center Task List for follow-up.
  https://learn.microsoft.com/en-us/dynamics365/business-central/production-how-to-view-the-load-on-work-centers

- **Work with Production Families in Manufacturing**
  Clarified the concept and benefits of production families and when to use a family production order. Highlighted scenarios where one operation yields multiple related items to reduce scrap and setup time, supported by a practical example.
  https://learn.microsoft.com/en-us/dynamics365/business-central/production-how-work-family

- **Manufacturing overview**
  Broadened coverage to include planning, capacity, execution, costing, quality, subcontracting, and analytics, and clarified posting of consumption, output, scrap, and operation time. Replaced a narrow reversal task with comprehensive guidance for reversing and correcting production transactions, and updated the Premium-experience guidance.
  https://learn.microsoft.com/en-us/dynamics365/business-central/production-manage-manufacturing

- **Block or unblock lots**
  Reworked examples to separate inspection status from inspection result and introduced a restriction model (Block, Allow finished only, Allow) that changes by open vs. finished inspections. Added tables showing how policies affect Sales and Transfer permissions and clarified how “Only the newest inspection/re-inspection” determines which inspection governs restrictions, including re-inspection behavior.
  https://learn.microsoft.com/en-us/dynamics365/business-central/qms-lot-blocking-unblocking

- **Inspect the quality of production output**
  Added instructions to print or email inspection reports directly from the Quality Inspection page and described three report types: Certificate of Analysis, Non Conformance Report, and Inspection Report. Explained that report content adapts to inspection data and that default Word layouts can be customized.
  https://learn.microsoft.com/en-us/dynamics365/business-central/qms-production-output-testing

- **Purchase receipt inspections without warehouse handling**
  Documented how to print or email inspection reports and explained the purposes of Certificate of Analysis, Non Conformance Report, and Inspection Report. Clarified dynamic content behavior and availability of customizable default Word layouts.
  https://learn.microsoft.com/en-us/dynamics365/business-central/qms-purchase-receipt-testing-simple

- **Quality management setup and configuration**
  Clarified the “Certificate of Analysis Contact” setting and how it populates the signature block with contact details, or remains empty if not set. Added a note on “Purchase Orders Trigger” explaining auto-release on posting, inspection creation, and how failures can leave inspections that may be duplicated on retry depending on the creation option.
  https://learn.microsoft.com/en-us/dynamics365/business-central/qms-setup

- **Set up service management**
  Noted that Service Management features require the Premium experience and provided a link to enable it. This ensures admins configure the correct experience before using service capabilities.
  https://learn.microsoft.com/en-us/dynamics365/business-central/service-setup-service

- **Synchronize customers and companies**
  Clarified metafield deletion behavior: removing a value or record in Business Central does not delete it in Shopify. Users must delete the metafield in Shopify; subsequent sync removes the local metafield record.
  https://learn.microsoft.com/en-us/dynamics365/business-central/shopify/synchronize-customers

- **Enable Premium features**
  Retitled and focused the article on how to enable the Premium experience, adding a clear procedure via Company Information. Consolidated licensing and permissions guidance, including who can change the setting, the need to refresh assignments, and the limitation that Essentials users cannot sign in to a Premium company.
  https://learn.microsoft.com/en-us/dynamics365/business-central/ui-experiences