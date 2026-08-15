# Dynamics 365 Finance
**Date created:** 2026-08-15 UTC  
**Tags:** Compliance, Configuration, Guidance  

## Major Changes

- **Data collection and classification for the French e-reporting**

  Added a detailed section mapping field lineage from the e-reporting union views (EReportingTransactionReportTypeUnionView and EReportingPaymentReportTypeUnionView) to their underlying physical table fields. Included mapping tables, identified which date fields control reporting period filters, and outlined where fields are computed, constant, blank, or conditionally sourced. Also clarified configurable criteria and the behavior of the “Date of VAT register.” These updates improve traceability, reduce configuration errors, and support audit-ready reporting.

  https://learn.microsoft.com/en-us/dynamics365/finance/localizations/france/emea-fra-e-reporting-details

- **VAT setup details for VAT declarations in the United Kingdom**

  Corrected the VAT return Box 3 formula to “box 1 + box 2” and refined guidance for handling reverse charge versus postponed VAT accounting (PVA) using VAT Declaration JSON (UK) format version 32.32 or later with ReportFieldLookup values per sales tax code. Clarified how the “Empty tax base for outgoing tax” marker affects Box 6 and documented an alternative where PVA transactions can be excluded from Box 6 at reporting time while ReverseCharge remains included; Boxes 4 and 7 are unchanged. The changes improve reporting accuracy and introduce a configuration approach that can remove the need for a reverse charge rule in applicable scenarios.

  https://learn.microsoft.com/en-us/dynamics365/finance/localizations/united-kingdom/emea-gbr-mtd-vat-integration-declaration

## Moderate Changes

- **Prepare your environment to interoperate with HMRC's MTD VAT web service**

  Expanded setup guidance for VAT declaration result values, including ReverseCharge and PVA scenarios that require VAT Declaration JSON (UK) format version 32.32 or later and explicit tax code mapping. Added instructions to prioritize specific ReverseCharge/PVA conditions over generic rules, plus new subsections for classifier definition and application-specific parameter setup, with tips to prevent misclassification and ensure company-specific replication across legal entities.

  https://learn.microsoft.com/en-us/dynamics365/finance/localizations/united-kingdom/emea-gbr-mtd-vat-integration-setup