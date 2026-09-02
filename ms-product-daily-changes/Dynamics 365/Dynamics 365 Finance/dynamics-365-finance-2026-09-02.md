# Dynamics 365 Finance
**Date created:** 2026-09-02 UTC  
**Tags:** Automation, Compliance, Configuration, Get Started, Guidance  

## Major Changes

- **Onboarding for electronic invoicing in Saudi Arabia**

  Overhauled onboarding guidance and scripts to align with ZATCA requirements and clarify simulation vs. production setup. Updated CSR parameters (SHA256 default, CN and certificateTemplateName values) and expanded field descriptions to reduce setup errors. Upgraded the onboarding script to v1.3 with an -environment switch, centralized endpoint variables, and improved error handling; API calls now adapt to the selected environment. Refreshed examples and instructions for obtaining and storing CCSID/PCSID in Azure Key Vault and clarified compliance checks, improving reliability and audit readiness.

  https://learn.microsoft.com/en-us/dynamics365/finance/localizations/mea/gs-e-invoicing-sa-onboarding

## Moderate Changes

- **Cross-LATAM localization overview**

  Reorganized the article around a unified Cross-LATAM framework, with clear prerequisites, feature enablement guidance, and links to country or region overviews. Added a consolidated features section via Electronic Reporting and streamlined structure by removing redundant tables and sections, improving discoverability and setup consistency.

  https://learn.microsoft.com/en-us/dynamics365/finance/localizations/iberoamerica/latam-overview

- **What's new or changed in Invoice capture**

  Added a Sept 2026 section for version 2.9.x introducing AI Recognition (preview) that combines OCR and LLMs to improve invoice data extraction accuracy. Documented fixes for duplicate captures from identical files and formatting enforcement issues, and standardized headings and wording across prior entries to improve clarity.

  https://learn.microsoft.com/en-us/dynamics365/finance/get-started/whats-new-invoice-capture