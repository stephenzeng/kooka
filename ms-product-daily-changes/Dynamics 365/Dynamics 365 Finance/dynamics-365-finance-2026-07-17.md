# Dynamics 365 Finance
**Date created:** 2026-07-17 UTC  
**Tags:** Administration, Automation  

## Major Changes

- **Automatic settlement and prioritization**

  Expanded and reorganized guidance for configuring automatic settlement and settlement priority to improve accuracy and consistency. Added a Default automatic settlement section with an illustrative table and step-by-step instructions for defining and ordering priority attributes (such as transaction type, due date, cash discount date, transaction date, amount, and voucher). Included detailed scenarios covering cash discount handling, overpayment behavior, and remaining credits, plus important considerations for interactions with manual marking and discount eligibility. Updated examples and tables for clarity and consistency.

  https://learn.microsoft.com/en-us/dynamics365/finance/accounts-receivable/automatic-settlement-prioritization

## Moderate Changes

- **Cash application in advanced bank reconciliation**

  Clarified the automatic customer account matching logic in bank reconciliation rules: the system matches the Related bank account to the customer’s IBAN first, then falls back to the bank account number. Explained that when a match is found, the customer account is auto-selected to create and post the payment journal; disabling this option requires manual account selection.

  https://learn.microsoft.com/en-us/dynamics365/finance/cash-bank-management/apply-cash-adv-bank-rec

- **Set up advanced bank reconciliation import by using Electronic reporting**

  Updated guidance to set up Advanced Bank Reconciliation imports with Electronic Reporting, explicitly covering ISO 20022 CAMT.053, MT940, and BAI2. Added clear steps to pick and validate the correct ER configuration per format, align bank account settings, and follow the import workflow, with a caution that mismatched formats can cause import failures.

  https://learn.microsoft.com/en-us/dynamics365/finance/accounts-payable/import-BAI2-ER