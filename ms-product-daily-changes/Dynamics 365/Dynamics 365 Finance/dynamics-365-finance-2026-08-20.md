# Dynamics 365 Finance
**Date created:** 2026-08-20 UTC  
**Tags:** Compliance, Configuration, Guidance  

## Moderate Changes

- **VAT declaration (Austria)**

  Added support for Austria’s new 4.9% reduced VAT rate by introducing KZ124 for taxable deliveries and KZ125 for intra‑community acquisitions, and updated Section 5 input tax mappings for KZ065. Refined ER configuration guidance to import VAT Declaration XML/Excel (AT) formats under the Tax declaration model and pointed to Dataverse-based import steps, helping organizations remain compliant with upcoming Austrian VAT requirements.

  https://learn.microsoft.com/en-us/dynamics365/finance/localizations/austria/emea-aut-vat-declaration-austria

- **Set up advanced bank reconciliation import by using Electronic reporting**

  Updated the setup guidance to specify File type selection and handling of ZIP archives that contain multiple files, including support for multiple file types via semicolons. These clarifications help ensure imports process correctly and reduce configuration errors.

  https://learn.microsoft.com/en-us/dynamics365/finance/accounts-payable/import-BAI2-ER

- **Regulatory updates**

  Added entries for Norway and Austria: Norway details changes to authorization scopes for VAT Return Submission API integrations effective September 2026, with links to registration and environment setup. Austria notes upcoming VAT declaration format changes effective July 2026, guiding customers to prepare for compliance.

  https://learn.microsoft.com/en-us/dynamics365/finance/localizations/global/regulatory-updates