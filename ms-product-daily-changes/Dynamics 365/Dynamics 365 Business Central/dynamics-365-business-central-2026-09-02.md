# Dynamics 365 Business Central
**Date created:** 2026-09-02 UTC  
**Tags:** Best Practices, Configuration, Guidance, Troubleshooting  

## Major Changes

- **Revalue general ledger account balances**

  Expanded and restructured guidance on G/L currency revaluation, introducing source currency tracking and when to use revaluation versus alternative approaches, with auditor considerations. Clarifies setup on the G/L Account Card, including allowed posting currencies via Source Currency Posting, enabling/disabling revaluation, and selecting realized/unrealized gains and losses accounts. Details how the G/L Currency Revaluation batch job operates at balance level per account, currency, and dimension (not at transaction level), and explains ACY implications with a reminder to run Adjust Exchange Rates after ACY rate updates. Adds comparisons with customer/vendor exchange rate adjustments, rounding behavior differences between documents and journals, and practical examples to choose the right method. Includes known considerations, troubleshooting scenarios for unexpected results, and best practices to improve accuracy and governance.

  https://learn.microsoft.com/en-us/dynamics365/business-central/finance-revalue-account-balances