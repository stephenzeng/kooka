# Dynamics 365 Finance
**Date created:** 2026-09-03 UTC  
**Tags:** Compliance, Configuration, Guidance, Troubleshooting  

## Major Changes

- **How to use France e-reporting in Dynamics 365 Finance**

  Updated the report generation experience to clearly separate outputs by data type (transactions vs. payments), document direction (outgoing vs. incoming), and reporting period derived from the VAT regime. Introduced rules that generate files only after a period is complete and automatically carry forward pending items, reducing manual reconciliation. Added a step-by-step monthly example for the standard VAT regime, showing ten‑day transaction periods and how initial (IN) and rectifying (RE) transmissions are produced. Clarified EDICOM integration behavior that auto-sets TypeCode to RE and the requirement to set it manually when not integrated, ensuring corrections are properly flagged.

  https://learn.microsoft.com/en-us/dynamics365/finance/localizations/france/emea-fra-e-reporting-experience

- **How to prepare your Dynamics 365 Finance for French e-Reporting**

  Expanded setup guidance to explain how FR‑eRep GenerateReportFile groups outputs by data type, document direction, and reporting period, with each file covering exactly one period. Detailed how reporting periods are derived from the declarant’s VAT regime, including ten‑day transaction periods for the monthly regime, monthly periods for payments and simplified regimes, and bimonthly civil periods for the franchise regime. Added instructions for handling rectifying transmissions using the FR‑eRep TypeCode field, including expected behavior when EDICOM integration is enabled, so corrections are consistently identified.

  https://learn.microsoft.com/en-us/dynamics365/finance/localizations/france/emea-fra-e-reporting-preparation

## Moderate Changes

- **Fix Financial Dimension Errors in Dynamics 365 Finance**

  Updated troubleshooting to verify required financial dimensions on both Account and Offset account and to allow blanks only when aligned with business processes. Clarified suspended value behavior (hidden in lookups, rejected at validation/posting) and advised against reactivating values solely for diagnosis. Added guidance for system‑generated transactions and historical data after account structure changes, including reviewing XDS/security role restrictions and temporarily relaxing structures during low‑activity windows to resolve failures.

  https://learn.microsoft.com/en-us/troubleshoot/dynamics-365/finance/general-ledger/common-dimension-related-errors

- **France e-reporting (electronic reporting of transactions) overview**

  Added a Reporting periods section explaining how transmissions are organized by VAT regime and period, including monthly ten‑day transaction periods for the standard regime, monthly periods for simplified, and bimonthly civil periods for franchise in base. Reinforced that each transmission covers a single period, corrections are submitted as rectifying transmissions, and the VAT regime must be selected during report generation.

  https://learn.microsoft.com/en-us/dynamics365/finance/localizations/france/emea-fra-e-reporting