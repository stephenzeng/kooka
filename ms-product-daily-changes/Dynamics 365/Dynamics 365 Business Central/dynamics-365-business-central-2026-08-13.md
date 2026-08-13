# Dynamics 365 Business Central
**Date created:** 2026-08-13 UTC  
**Tags:** Configuration, Guidance, Troubleshooting  

## Moderate Changes

- **Expense Agent Overview**

  Clarified regional AI subprocessor requirements: U.S. environments use Anthropic Claude and require enabling Anthropic as a subprocessor in Microsoft 365 Admin Center, while other regions use OpenAI GPT with no extra configuration. This helps admins meet compliance needs and avoid setup interruptions.

  https://learn.microsoft.com/en-us/dynamics365/business-central/expense-management/expense-agent

- **Set up Expense Agent**

  Updated prerequisites to a single, region-specific requirement: enable the Anthropic subprocessor for U.S. tenants; no additional AI subprocessor setup is needed elsewhere. This streamlines deployment and reduces misconfiguration risk.

  https://learn.microsoft.com/en-us/dynamics365/business-central/expense-management/expense-agent-configuration-page

- **Responsible AI FAQ for Expense Agent (preview)**

  Clarified that the U.S. uses Anthropic Claude and other regions use OpenAI GPT, and generalized references to “AI” across capabilities. The evaluation guidance was revised to reflect region-specific models, improving transparency and expectation setting.

  https://learn.microsoft.com/en-us/dynamics365/business-central/expense-management/faqs-expense-agent

- **Item availability in Sales Order Agent (preview)**

  Added troubleshooting guidance for price calculations, explaining how the agent uses a temporary sales document and how extensions can lead to a price of 0. Provides steps to reproduce, view the call stack, enable error notifications, and identify extensions that must check IsTemporary before running custom logic, helping resolve pricing failures.

  https://learn.microsoft.com/en-us/dynamics365/business-central/sales-order-agent-item-availability