# Dynamics 365 Finance
**Date created:** 2026-08-07 UTC  
**Tags:** Administration, Analytics  

## Major Changes

- **What's new or changed in Dynamics 365 Finance 10.0.49 (September 2026)**

  Expanded the release notes with significant Electronic Reporting (ER) enhancements, including native GS1 barcode formats, new DIV and MOD functions, and improvements for print management copies, validation control, and memory guidance for large runs. A new mandatory behavior ensures model mappings always respect the Run draft option, aligning environments for predictable execution. Several ER capabilities were removed from feature management and are now on by default, streamlining setup and reducing configuration overhead. These updates improve reporting accuracy, performance, and governance for finance operations.

  https://learn.microsoft.com/en-us/dynamics365/finance/get-started/whats-new-changed-10-0-49

## Moderate Changes

- **Bank foreign currency revaluation**

  Added a troubleshooting section that outlines checks for missing gain/loss amounts and explains causes of unusually large voucher lines in legacy revaluation, with guidance to enable the enhanced revaluation logic and reset historical data where needed. The updates clarify steps and decision points so finance teams can resolve reconciliation anomalies faster and prevent repeat issues.

  https://learn.microsoft.com/en-us/dynamics365/finance/cash-bank-management/bank-revaluation

- **Post detailed payments for vendor and customers**

  Clarified that payment journals with fees won’t support bank transaction summarization; Finance creates separate bank transactions when fees are present. This helps teams anticipate additional reconciliation lines and adjust processes accordingly.

  https://learn.microsoft.com/en-us/dynamics365/finance/general-ledger/summary-payment