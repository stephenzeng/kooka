# Dynamics 365 Supply Chain Management
**Date created:** 2026-08-20 UTC  
**Tags:** Configuration, Guidance, Troubleshooting  

## New Articles

- **Can't Reduce Product Receipt Quantity Below Invoiced Quantity**

  Introduces guidance that receipt corrections cannot reduce quantities below what’s already invoiced, by design, to protect inventory integrity and valuation. Explains symptoms and error messages, and clarifies the underlying rationale. Provides step-by-step options to reverse or credit the vendor invoice, confirm no change if the invoice is correct, or use a return order for excess quantities. Highlights the difference between Correct and Cancel actions and links to related references.

  https://learn.microsoft.com/en-us/troubleshoot/dynamics-365/supply-chain/procurement/cant-correct-product-receipt-quantity-below-invoiced

- **Purchase Requisition Submit, Workflow, or Approval Unavailable**

  Explains common reasons why submission or workflow actions may be unavailable, focusing on draft eligibility, workflow state and assignments, and user security. Outlines how to verify the Workflow message processing batch job and interpret batch history, clarifying its role versus draft submission eligibility. Provides least-privilege guidance and when to escalate to Microsoft Support, with links for configuring the workflow batch job.

  https://learn.microsoft.com/en-us/troubleshoot/dynamics-365/supply-chain/procurement/purchase-requisition-workflow-actions-unavailable

- **Canceled Purchase Orders Can't Be Finalized**

  Describes the scenario where canceled purchase orders can’t be finalized because the source document header remains In process. Identifies the data-state cause and provides a practical sequence to reprocess accounting distributions by requesting changes, re-submitting for workflow approval, confirming, and then finalizing. Notes considerations for workflow approvers and includes related references.

  https://learn.microsoft.com/en-us/troubleshoot/dynamics-365/supply-chain/procurement/unable-to-finalize-cancelled-purchase-orders