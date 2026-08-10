# Dynamics 365 Finance
**Date created:** 2026-07-15 UTC  
**Tags:** Administration, Automation  

## Major Changes

- **Advanced bank reconciliation setup process**

  Overhauled setup guidance with clearer end-to-end procedures for configuring Advanced bank reconciliation. Introduced explicit “Transaction types” and detailed mapping of bank statement codes to Finance transaction types per bank account. Expanded configuration instructions for General settings and Automation with field-by-field explanations to help reduce errors and improve matching accuracy. These updates make it easier to enable, tune, and automate reconciliation consistently across accounts.

  https://learn.microsoft.com/en-us/dynamics365/finance/cash-bank-management/configure-advanced-bank-reconciliation

- **Set up bank reconciliation matching rules**

  Expanded guidance to provide step-by-step setup for matching rules and a comprehensive breakdown of actions, including availability in base vs. Modern experiences and key parameters. Added prerequisites for Modern-only actions and new sections on creating, managing, and running matching rule sets by default, on import, or on demand. This improves implementation consistency and helps teams automate reconciliation with predictable, auditable results.

  https://learn.microsoft.com/en-us/dynamics365/finance/cash-bank-management/set-up-bank-reconciliation-matching-rules

## Moderate Changes

- **Create a depreciation proposal**

  Moved the depreciation performance feature from preview to general availability and clarified differences between budget vs. actual proposals to explain total variances. Improved performance and reliability with optimized batch processing, prevention of empty/duplicate journals, enhanced caching, broader asset ID support, and stronger multi-entity behavior. Guidance emphasizes running in batch for stability and throughput.

  https://learn.microsoft.com/en-us/dynamics365/finance/fixed-assets/tasks/create-depreciation-proposal

- **Foreign currency revaluation for bank accounts**

  Expanded coverage to include Hungary and added configuration details for exchange difference type (FIFO/LIFO) and related number sequences. Clarified setup for exchange rates and ledger postings and streamlined execution steps, helping organizations run bank revaluations accurately across supported countries.

  https://learn.microsoft.com/en-us/dynamics365/finance/localizations/europe/emea-foreign-currency-revaluation

- **Import ISO20022 credit transfer configuration**

  Enhanced the import procedure with clearer repository navigation in Dataverse and explicit selection steps. Added guidance for choosing the correct structured vs. unstructured configuration and introduced a confirmation step to avoid duplicate imports.

  https://learn.microsoft.com/en-us/dynamics365/finance/localizations/europe/import-iso20022-credit-transfer-configuration