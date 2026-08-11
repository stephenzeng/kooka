# Dynamics 365 Finance
**Date created:** 2026-08-05 UTC  
**Tags:** AI, Administration, Analytics, Automation, Security  

## Moderate Changes

- **Set up and configure the Account reconciliation agent (production ready preview)**

  Streamlined setup by removing numerous PowerShell Enable-TriggerFlow commands from the configuration steps. This reduces complexity and the risk of misconfiguration, aligning guidance with the current automation model.

  https://learn.microsoft.com/en-us/dynamics365/finance/general-ledger/configure-acct-recon-agent

- **Register an integration point in the ID-porten web portal**

  Updated required API scopes for direct VAT submission in Norway: removed mvameldingvalidering and added altinn:instances.read and altinn:instances.write (with openid and mvameldinginnsending retained). This ensures correct authorization and successful end-to-end submission.

  https://learn.microsoft.com/en-us/dynamics365/finance/localizations/norway/emea-nor-vat-return-integration-point

- **Invoice capture solution advanced settings**

  Updated guidance to rename the connector to Microsoft 365 Outlook, clarified admin prerequisites, and simplified Dataverse connection steps. These changes reduce setup friction and improve accuracy when configuring channels.

  https://learn.microsoft.com/en-us/dynamics365/finance/accounts-payable/invoice-capture-advanced-settings

- **Invoice capture FAQ**

  Removed the outdated FAQ about minimum supported Finance versions and made minor clarity edits. This helps avoid confusion and keeps the FAQ focused on current behavior.

  https://learn.microsoft.com/en-us/dynamics365/finance/accounts-payable/invoice-capture-faq

- **Maintain vendor bank account information**

  Removed feature toggle instructions and consolidated guidance for reviewing vendor bank changes, running pre-note validation, updating the primary payment method, and marking reviews complete. The update reflects current functionality and clarifies a consistent review workflow.

  https://learn.microsoft.com/en-us/dynamics365/finance/accounts-payable/maintain-vendor-bank-info

- **Mobile invoice approvals**

  Simplified prerequisites by removing legacy version and hotfix requirements and updated notes on the invoice total display parameter. The guidance aligns with current app behavior and makes onboarding faster.

  https://learn.microsoft.com/en-us/dynamics365/finance/accounts-payable/mobile-invoice-approvals

- **Alignment date scenarios**

  Refreshed all examples to 2023–2028 timelines with recalculated billing periods, unit prices, and parameters across multiple alignment and proration scenarios. Current-dated scenarios improve accuracy and applicability for planning and billing analysis.

  https://learn.microsoft.com/en-us/dynamics365/finance/accounts-receivable/sb-alignment-date-examples

- **Vendor invoice center workspace overview**

  Corrected the definition of the Manual entry “Without errors” status to indicate invoices are complete and eligible for automation. This clarification helps users correctly transition items into automated processing.

  https://learn.microsoft.com/en-us/dynamics365/finance/accounts-payable/vendor-invoice-workspace

- **Vendor payments workspace**

  Removed the requirement to configure system currency and exchange rate settings for Power BI visuals in the workspace. This simplifies setup and reflects current visualization dependencies.

  https://learn.microsoft.com/en-us/dynamics365/finance/accounts-payable/Vendor-payments-workspace