# Microsoft Fabric
**Date created:** 2026-08-04 UTC  
**Tags:** AI, Administration, Analytics, Automation, Security  

## New Articles

- **Create a cross-tenant OneLake shortcut**

  Introduced a step-by-step guide for creating cross-tenant OneLake shortcuts using delegated authentication. The article explains producer and consumer roles, when to choose cross-tenant shortcuts versus external data sharing, and required prerequisites such as roles, IDs, and credentials. It provides detailed UI steps for configuring connections, authenticating with an organizational account or service principal, selecting source items, and finalizing the shortcut. Related links help readers find same-tenant guidance, delegated authentication details, connection management, and external data sharing.

  https://learn.microsoft.com/en-us/fabric/onelake/shortcuts/create-cross-tenant-onelake-shortcut

- **Intelligence Sheets FAQ for Fabric Plan**

  Added a comprehensive FAQ covering what Intelligence Sheets are, how they differ from Planning Sheets, and how to build and format reports. It explains data behaviors (PBIX imports, semantic model reuse), feature support (filters, styling, themes, comments, sharing), and practical how-tos like creating matrix visuals and P&L reports. The FAQ also addresses embedding visuals, hierarchy handling, auto-fit options, and troubleshooting missing semantic models to speed up adoption and reduce setup issues.

  https://learn.microsoft.com/en-us/fabric/iq/plan/faq-intelligence

- **Use simulation measures in a planning sheet**

  Published a how-to guide for creating and managing simulation measures in planning sheets. It covers configuration options, adjusting values via sliders with parent-child propagation, and editing or locking simulations to control updates. The guide also explains deleting simulations and performing bulk edits with filters and level targeting to streamline scenario analysis and what-if planning.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-how-to-use-simulation-measures

## Major Changes

- **Azure Billing for Your Fabric Capacity**

  Significantly expanded and restructured guidance on how Fabric capacity usage maps to Azure billing. Added detailed explanations of invoice meters, including naming patterns and OneLake-specific suffixes, plus an alphabetical list of meter groups with workload descriptions. Introduced instructions to retrieve the authoritative meter list via the Azure Retail Prices API and a new section on storage-related meters (OneLake tiers, BCDR, cache, SQL/Cosmos DB, mirroring). Clarified how to reconcile Azure charges with the Fabric Capacity Metrics app, with examples and regional pricing notes, helping admins validate costs with confidence.

  https://learn.microsoft.com/en-us/fabric/enterprise/azure-billing

- **Billing for AI Functions**

  Clarified bring-your-own-model billing for pandas and PySpark AI Functions: Fabric doesn’t charge for custom endpoint model calls, though LLM providers bill token usage; Fabric compute charges still apply. Updated the billing table to clearly separate built-in Fabric LLM endpoint calls (billed as AI Functions) from custom endpoint calls (no Fabric model-call charge). Modernized the language models section by removing older GPT-4.1 entries and the retirement column, leaving only gpt-5.1 and gpt-5-mini with current consumption rates. This reduces confusion and helps teams plan costs accurately across built-in and custom AI workflows.

  https://learn.microsoft.com/en-us/fabric/data-science/ai-functions/billing

- **Create a same-tenant OneLake shortcut**

  Re-scoped the article to focus solely on creating same-tenant OneLake shortcuts and retitled it accordingly. Removed cross-tenant instructions and folded delegated identity guidance into the dedicated OneLake shortcut security page, with a tip pointing to the cross-tenant article. Streamlined the procedure and added an explicit step for configuring service principal details when using delegated identity. This separation clarifies which guide to use and reduces setup errors for same-tenant scenarios.

  https://learn.microsoft.com/en-us/fabric/onelake/shortcuts/create-onelake-shortcut

## Moderate Changes

- **Foundry Tools in Fabric (preview)**

  Updated the OpenAI language models coverage by removing references to retiring GPT-4.1 variants, default model migration guidance, and the Retirement Date column. The consumption table now lists only gpt-5.1 and gpt-5-mini with current details, reducing outdated guidance and simplifying model selection.

  https://learn.microsoft.com/en-us/fabric/data-science/ai-services/ai-services-overview

- **Get started with OneLake security**

  Revised guidance to reflect a default of Delegated identity mode for the SQL analytics endpoint. To enforce OneLake security, Admins or Members must switch the endpoint to User’s identity mode, with steps linked for clarity.

  https://learn.microsoft.com/en-us/fabric/onelake/security/get-started-onelake-security

- **OneLake shortcut security**

  Clarified the permissions model for creating, reading, updating, and deleting shortcuts, including combined OneLake security roles and Fabric permissions for each operation. Separated authentication guidance for same-tenant (passthrough or delegated) versus cross-tenant (delegated only) scenarios and noted that switching between passthrough and delegated requires recreating the shortcut. Related links now point to distinct same-tenant and cross-tenant creation guides to improve navigation.

  https://learn.microsoft.com/en-us/fabric/onelake/onelake-shortcut-security

- **Known limitations in plan**

  Added a new limitation stating that automatic application database creation isn’t supported when deploying plan items via CI/CD with a service principal. This helps teams adjust deployment pipelines and plan for manual or alternative setup steps to avoid failures.

  https://learn.microsoft.com/en-us/fabric/iq/plan/overview-limitations