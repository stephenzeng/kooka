# Dynamics 365 Finance
**Date created:** 2026-07-21 UTC  
**Tags:** Administration, Analytics, Automation  

## New Articles

- **Collection letter automation overview for Dynamics 365 Finance**

  Introduced a new overview of collection letter automation that explains customer-level evaluation and how the oldest qualifying invoice sets the collection stage. Clarifies that each run generates a single communication per customer, which includes only eligible invoices. Describes the Track step option for progression tracking and how it prevents unnecessary repeat communications. Highlights prioritization rules where overdue processing supersedes pre-dunning reminders, and provides key considerations, FAQs, and links to next steps for setup.

  https://learn.microsoft.com/en-us/dynamics365/finance/accounts-receivable/cm-collection-letter-automation

## Major Changes

- **Budget planning**

  Rewrote and reorganized the article from a lab-style guide into a structured how-to, improving discoverability and task clarity. Added prerequisites (including sign-in and Excel add-in guidance) and updated scenarios to FY2026 with clearer steps for organizational hierarchy setup, security configuration, and role requirements. Expanded coverage of building scenarios, defining budget plan columns via the Excel add-in, and creating layouts and Excel templates. Consolidated guidance for creating and activating budget planning processes with stage rules and default/alternate layouts, and added a process simulation from General ledger through allocation, Excel editing, publishing, and workflow—ending with a streamlined auto-approve workflow configuration.

  https://learn.microsoft.com/en-us/dynamics365/finance/budgeting/budget-plan

- **Troubleshoot cash flow forecasting**

  Expanded troubleshooting for Cash flow forecasting and Cash overview with clearer setup prerequisites such as defining the Date dimension with a future end date. Added guidance for common issues, including using separate liquidity accounts per bank, resolving forecasts that display by main account instead of bank account, and fixing purchase order forecast errors caused by Sales tax settlement periods misaligned with tax dates. Clarified Entity store measurement checks and refresh behavior, and refined performance recommendations for batch jobs (daily New calculations and weekly Total recalculations).

  https://learn.microsoft.com/en-us/dynamics365/finance/cash-bank-management/cash-flow-forecasting-tsg

- **Create new checks or reuse existing checks**

  Added a new feature description for reusing checks, including prerequisites (regional availability, fixed number sequences, parameter enablement, and eligibility conditions) and steps to enable it in Cash and bank management. Provided a guided process to reuse a check in Accounts payable payment journals and updated the article title and description to reflect both creating and reusing checks. Clarified temporary bank account deactivation during blank check creation and automatic reactivation after processing.

  https://learn.microsoft.com/en-us/dynamics365/finance/cash-bank-management/create-check-with-blank-status

## Moderate Changes

- **Reverse a vendor payment**

  Reorganized and clarified the end-to-end workflows for reversing posted checks, with step-by-step instructions for immediate and review-based reversals and an updated comparison. Improved outcome descriptions for intercompany transactions, vendor payments, and customer refunds, and added troubleshooting for posting failures after account structure changes and the “No more checks for account” error.

  https://learn.microsoft.com/en-us/dynamics365/finance/accounts-payable/reverse-vendor-payment