# Dynamics 365 Project Operations
**Date created:** 2026-08-19 UTC  
**Tags:** Billing, Configuration, Guidance, Troubleshooting  

## New Articles

- **Bulk update tasks on the task grid**

  Introduced a how-to guide for project managers to bulk update Start date, Finish date, % Complete, and Assigned to across multiple tasks directly from the task grid. Explains prerequisites and permissions, how to open and use the Edit tasks pane, and behavior for summary tasks and scheduling after date changes. Clarifies how resource assignments are handled (Reassign vs Add Assignment), what happens when % Complete or Finish date aren’t available, and that bulk updates don’t change resource bookings. Provides undo guidance, a field behavior reference, and a Common issues section with resolutions.

  https://learn.microsoft.com/en-us/dynamics365/project-operations/project-management/bulk-update-tasks

- **Post costs between balance sheet and profit and loss accounts (Preview)**

  Introduces the Post costs feature for integrated ERP deployments, explaining when costs post to P&L versus balance sheet and how to move them using Post costs. Details supported scenarios—T&M contract lines and internal projects—and exclusions such as fixed price and investment projects. Provides enablement steps via Feature management and clarifies that costs can’t be moved if revenue is already accrued or invoiced. Highlights new support for internal projects to hold costs on the balance sheet and later move them to P&L.

  https://learn.microsoft.com/en-us/dynamics365/project-operations/project-accounting/post-costs-overview

- **Reconcile accrued revenue**

  Adds a step-by-step guide to detect and correct accrued revenue (WIP) imbalances after invoicing or adjustments. Covers prerequisites, roles and privileges, number sequences, and batch processing, plus where to access the reconciliation workspace. Explains detection views and filters (Transactions, Projects, Ledger Accounts), symmetric vs. asymmetric corrections, and the end-to-end process from investigation to posting and verification. Shares best practices such as aligning subledger and general ledger exchange rates and answers FAQs on empty results and reversals.

  https://learn.microsoft.com/en-us/dynamics365/project-operations/invoicing/reconcile-accrued-revenue

## Major Changes

- **Migrate fully invoiced billing milestones at cutover**

  Expanded guidance now covers progress-based billing lines using a schedule of values, helping teams handle cutover without disrupting financials. Adds instructions to mark previously invoiced percentages as invoiced without impacting Accounts receivable or General ledger, reducing reconciliation risk. Introduces a new dual-write value mapping for transaction status (0 -> 192350000) alongside the existing mapping (4 -> 192350001) to improve data alignment. Includes an end-to-end procedure for partially invoiced progress-based lines—switching map versions, creating the schedule of values, setting the next billed percentage, pausing relevant maps, invoicing, and reverting maps—so migrations complete reliably.

  https://learn.microsoft.com/en-us/dynamics365/project-operations/advanced-configuration/migrating-invoiced-milestones