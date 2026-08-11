# Dynamics 365 Sales
**Date created:** 2026-08-11 UTC  
**Tags:** Compliance, Configuration, Guidance, Security, Troubleshooting  

## Major Changes

- **Review and approve Data Enrichment suggestions**

  Expanded prerequisites to clarify user eligibility and which records are analyzed. Replaced the prior consent flow with automatic enrollment for reading relevant emails and Teams meetings, updated notification details, and noted that enrollment can fail if permissions are missing. Clarified that analysis typically completes in about four hours and only evaluates opportunity-relevant communications. Added step-by-step instructions to enable or disable suggestions via Personal Settings using the Sales agents toggle.

  https://learn.microsoft.com/en-us/dynamics365/sales/use-data-enrichment-agent

## Moderate Changes

- **Set up and configure AI-powered Data Enrichment**

  Restructured prerequisites into clear subsections and clarified data handling: emails are read from Exchange and Teams meeting data is processed in place without being stored in Dynamics 365. Added seller-level controls to disable the agent for email and meeting data, and replaced consent with per-seller enrollment that happens automatically the first time an opportunity is opened. Existing role, licensing, and tenant admin requirements remain unchanged for Teams connectivity.

  https://learn.microsoft.com/en-us/dynamics365/sales/data-enrichment-agent-configure

- **Edit AI-powered Data Enrichment settings**

  Updated guidance to use an enrollment model instead of explicit seller consent for when analysis occurs. Sellers are automatically enrolled when they first open an opportunity, and enrollment is managed per seller.

  https://learn.microsoft.com/en-us/dynamics365/sales/data-enrichment-agent-edit-settings

- **FAQs about AI-powered Data Enrichment for opportunities**

  Replaced consent-based explanations with guidance that the opportunity owner may have disabled the agent and provided steps to re-enable suggestions. Added a new FAQ on disabling suggestions for an account, clarifying that disabling stops analysis of emails and meeting data and prevents new suggestions from being generated.

  https://learn.microsoft.com/en-us/dynamics365/sales/data-enrichment-agent-faqs