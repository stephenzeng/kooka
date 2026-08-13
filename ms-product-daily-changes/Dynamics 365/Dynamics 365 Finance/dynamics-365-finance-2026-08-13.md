# Dynamics 365 Finance
**Date created:** 2026-08-13 UTC  
**Tags:** Compliance, Configuration, Guidance  

## Major Changes

- **Export customer electronic invoices**

  Updated Türkiye e-invoice guidance with detailed configuration for Invoice type (e-Invoice vs e-Archive) and clear rules for how ProfileID is populated in UBL-TR XML. Added a comprehensive scenario matrix with ProfileID codes and introduced a Requires commercial approval option that enforces TICARIFATURA when needed. Provided end-to-end steps to control and override ProfileID at the transaction level via Invoice profile for sales orders and free text invoices, plus instructions for generating, reviewing (ER jobs), and sending (ER destinations) e-invoices. These updates improve compliance, reduce configuration errors, and give finer control over invoice scenarios.

  https://learn.microsoft.com/en-us/dynamics365/finance/localizations/turkiye/emea-turkiye-customer-electronic-invoices

- **Export of customer electronic packing slips**

  Added guidance to select an invoice profile during packing slip posting to set the ProfileID in the UBL-TR DespatchAdvice XML. Included step-by-step instructions and a mapping of profile options to ProfileID values (None, TEMELIRSALIYE, HKSIRSALIYE, IDISIRSALIYE) with recommended usage. Noted that the chosen scenario is written to XML and cannot be changed after generation, supporting correct regulatory classification and downstream processing.

  https://learn.microsoft.com/en-us/dynamics365/finance/localizations/turkiye/emea-turkiye-customer-packing-slips

## Moderate Changes

- **Use exchange difference invoicing**

  Added guidance to apply exchange difference invoicing selectively for specific vendor or customer groups by configuring realized gain/loss accounts in the Currency revaluation posting profile. Clarified the account lookup hierarchy and emphasized setting Lowest level of defaulting to Account so group-specific rules take precedence, with examples of expected behavior. These updates help ensure accurate postings and consistent application of revaluation policies.

  https://learn.microsoft.com/en-us/dynamics365/finance/localizations/turkiye/emea-tur-exchange-difference-invoicing