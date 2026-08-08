# Dynamics 365 Finance
**Change date:** 2026-08-07 UTC  
**Tags:** Administration  

## Moderate Changes

- **Availability of Electronic Invoicing Service features by country or region**

  Updated availability to move Poland and Singapore from Preview to General availability and added a new GA entry for France (via EDICOM). Clarified capability scope by marking several GA entries as “format generation only,” helping organizations plan rollouts and integrations more accurately.

  https://learn.microsoft.com/en-us/dynamics365/finance/localizations/global/e-invoicing-country-specific-availability

- **Electronic invoicing for France**

  Added a procedure to mass-generate payment responses for eligible invoices submitted to EDICOM and fully paid, improving operational efficiency. Clarified AR response workflow and noted that AP refusal responses are only allowed for vendor invoices received through the Electronic documents process and listed in the receipt log, supporting correct compliance handling.

  https://learn.microsoft.com/en-us/dynamics365/finance/localizations/france/emea-fra-einv-ereport

- **Prepare your environment to interoperate with HMRC's MTD VAT web service**

  Introduced ReverseCharge and PVA classifier results (from format version 32.32) with explicit VAT return box behavior, and guided mapping of tax codes to these results. Advised ordering these conditions at the top of ReportFieldLookup and clarified box references for existing results to ensure accurate VAT classification and reporting.

  https://learn.microsoft.com/en-us/dynamics365/finance/localizations/united-kingdom/emea-gbr-mtd-vat-integration-setup

- **Electronic invoicing for Poland**

  Raised the required ER format version for Sales e-invoice (PL) to 329.40 and updated parameter configurations, including a new TaxExemptsLookUp. Clarified how additional invoice data populates XML and introduced the CorrectionType property (values 1–3) to ensure correct generation of the Faktura/Fa/TypKorekty element, improving compliance and data quality.

  https://learn.microsoft.com/en-us/dynamics365/finance/localizations/poland/gs-e-invoicing-pol-get-started