# Dynamics 365 Finance
**Date created:** 2026-07-30 UTC  
**Tags:** Administration, Governance  

## New Articles

- **France e-reporting (electronic reporting of transactions) implementation details**

  Introduced a comprehensive implementation guide for how France e-reporting data is collected, selected, and classified. Clarifies criteria used by the Populate Report Data action, including B2B/B2C rules, source entities, counterparty checks, and handling of tax direction/origin, reverse charge, and conditional tax. Details settlement requirements for payments and the behavior when Date of VAT register is enabled. Provides a selection matrix and exclusions to prevent double-counting, helping teams produce compliant, accurate reports.

  https://learn.microsoft.com/en-us/dynamics365/finance/localizations/france/emea-fra-e-reporting-details

- **France e-reporting (electronic reporting of transactions) experience**

  Added an end-to-end how-to for running France e-reporting in Dynamics 365 Finance using Electronic messages. Explains how to collect and review data, manage inclusions/exclusions, generate transactions-only, payments-only, or full XML reports, and regenerate corrections using TypeCode RE. Covers status transitions, batch scheduling, handling multiple VAT registrations within a single flow, and where generated XML files are stored. This guidance streamlines operational execution and improves traceability from data preparation through submission.

  https://learn.microsoft.com/en-us/dynamics365/finance/localizations/france/emea-fra-e-reporting-experience

- **France e-reporting (electronic reporting of transactions) preparation**

  Added setup guidance for configuring France e-reporting, including required ER configurations and setting the default model mapping. Provides instructions to configure application-specific parameters (such as TransCategoryCodeLookup), import the predefined Electronic messages setup, and define message and item additional fields and action parameter mappings. Describes executable classes used, security roles, and filtering guidance for accurate record selection, including scenarios with multiple VAT registrations. These steps help teams complete configuration faster and produce consistent, compliant output.

  https://learn.microsoft.com/en-us/dynamics365/finance/localizations/france/emea-fra-e-reporting-preparation

## Major Changes

- **France e-reporting (electronic reporting of transactions) overview**

  Retitled the content as an overview and removed detailed implementation and usage guidance. The article now focuses on core context and availability while directing procedural and configuration details to dedicated guides. This separation reduces duplication, clarifies navigation, and helps users quickly find task-specific instructions without wading through lengthy setup content.

  https://learn.microsoft.com/en-us/dynamics365/finance/localizations/france/emea-fra-e-reporting

## Moderate Changes

- **Financial tags**

  Updated guidance to enable financial tags for sales and purchase orders via the feature management page with direct references. Clarified availability: procurement document support begins in version 10.0.49 and later, with a link to the dedicated procurement financial tags article. This helps admins enable the feature correctly and align configurations with supported versions.

  https://learn.microsoft.com/en-us/dynamics365/finance/general-ledger/financial-tag