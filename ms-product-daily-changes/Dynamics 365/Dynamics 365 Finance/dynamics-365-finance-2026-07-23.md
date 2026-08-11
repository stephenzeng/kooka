# Dynamics 365 Finance
**Date created:** 2026-07-23 UTC  
**Tags:** AI, Administration, Agent, Other  

## New Articles

- **Decouple settlement from payment journal posting**

  Introduced a feature that lets customer and vendor payment journals post immediately while settlements are queued for background or on-demand processing. Describes configuration, processing cadence, and available actions to monitor or intervene in queued settlements. Explains status states, failure handling with manual retry, and that payments are not reversed if settlement fails. Highlights key limitations and that settlement logic remains unchanged, helping finance teams reduce posting latency while controlling settlement execution.

  https://learn.microsoft.com/en-us/dynamics365/finance/cash-bank-management/delayed-settlements

- **Changes to customer and vendor transaction settlement storage**

  Announced a new 10.0.49 architecture that writes settlement and exchange-adjustment state to companion tables (CustTransState, VendTransState) in parallel with existing fields. There are no functional or integration-breaking changes today, although a slight overhead is possible, and background backfill plus ongoing self-healing maintain data consistency. Outlines feature flags/kill switches and a roadmap to eventually read from the new tables and deprecate legacy fields. Provides an FAQ on enablement, performance, backfill duration, and compatibility to prepare customers and partners for the transition.

  https://learn.microsoft.com/en-us/dynamics365/finance/cash-bank-management/settlement-data-storage

- **What's new or changed in Dynamics 365 Finance 10.0.49 (September 2026)**

  Published release notes covering schedules, turned-on-by-default features, and module updates across AR, Budgeting, Cash and bank management, Fixed assets, and Subscription billing. Highlights include delayed settlement posting, bank reconciliation preview and performance improvements, accounting date advancement under budget control, diagnostics for budget control data, and reporting currency handling for fixed assets. Lists features becoming mandatory, items removed from Feature management, and references to platform updates, fixes, and regulatory changes. Helps admins and users plan adoption, validation, and change management for the release.

  https://learn.microsoft.com/en-us/dynamics365/finance/get-started/whats-new-changed-10-0-49

## Major Changes

- **Account reconciliation**

  Added comprehensive guidance to bulk mitigate reconciliation exceptions using grouped views driven by Account Reconciliation Agent suggestions. Users can review grouped exceptions by key attributes, edit or override bulk actions, and submit with confirmations while handling failures and skipped items. New controls let users adjust grouping and filters, reset to AI-suggested defaults, and understand impacts on agent summaries, with references to setup and undo actions. This improves scale, consistency, and speed in exception resolution.

  https://learn.microsoft.com/en-us/dynamics365/finance/general-ledger/account-reconciliation

- **Set up and configure the Account reconciliation agent (production ready preview)**

  Updated prerequisites by raising the minimum Finance version to 10.0.46 and removing now-unneeded preview dependencies and connections. Streamlined identity and connection setup, simplified the PowerShell deployment (removed DynamicsAXConnectionName), and refreshed the list of flows to reflect the latest activation set. These changes reduce setup complexity, align with current platform requirements, and better reflect the agent’s production-ready configuration.

  https://learn.microsoft.com/en-us/dynamics365/finance/general-ledger/configure-acct-recon-agent

- **Foreign currency revaluation using FIFO/LIFO for bank accounts**

  Introduced a new FIFO/LIFO-based exchange adjustment method for bank transactions, with detailed matching logic that pairs withdrawals to deposit layers to compute realized gains and losses. Expanded country applicability to Czech Republic, Estonia, Lithuania, and Latvia, and updated setup steps to choose exchange difference type and number sequences for the new process. Provides a worked example and replaces prior generic guidance with precise configuration and reporting instructions. This helps organizations achieve more accurate, auditable FX adjustments aligned with local requirements.

  https://learn.microsoft.com/en-us/dynamics365/finance/localizations/europe/emea-foreign-currency-revaluation

## Moderate Changes

- **Budget control overview**

  Expanded “Over budget permissions” with detailed behavior for allowing, threshold-based blocking, or fully preventing over-budget processing, plus a recommendation matrix for common scenarios. Added an important note for 10.0.49 on automatic accounting date advancement for budget-controlled PRs and POs, clarifying how dates adjust across closed or on-hold periods without rolling into a new fiscal year. These updates help finance teams configure controls that match policy and avoid posting disruptions.

  https://learn.microsoft.com/en-us/dynamics365/finance/budgeting/budget-control-overview-configuration

- **Account structures overview**

  Removed prior guidance suggesting account structures and advanced rules validate only Ledger account types and not non-ledger types. This correction prevents misconfiguration and ensures users rely on current validation behavior when designing structures and rules.

  https://learn.microsoft.com/en-us/dynamics365/finance/general-ledger/configure-account-structures

- **Electronic invoicing for Poland**

  Added setup steps for ASP parameters for Sales e-invoice (PL) format 316.34+, including zero tax rate lookup configuration for P_12 XML population. Clarified how the External item number maps to the Indeks element for both incoming vendor invoices and outgoing customer invoices. These changes improve compliance and data accuracy in Polish e-invoicing scenarios.

  https://learn.microsoft.com/en-us/dynamics365/finance/localizations/poland/gs-e-invoicing-pol-get-started

- **Settlement overview**

  Clarified that when balance summary accounts or financial dimensions differ between invoice and payment transactions, the system creates an additional settlement-type transaction to align balances and dimensions. This helps users interpret settlement results and reconcile outcomes more accurately.

  https://learn.microsoft.com/en-us/dynamics365/finance/cash-bank-management/settlement-overview

- **Set up and process bridged payments**

  Documented a 10.0.49 feature that improves performance when selecting bridge transactions during bank clearance through optimized querying and selection. Updated the procedure to reference the feature and highlight filtering options during clearance for faster matching. This reduces processing time and improves throughput in reconciliation workflows.

  https://learn.microsoft.com/en-us/dynamics365/finance/accounts-receivable/set-up-and-process-bridged-payments