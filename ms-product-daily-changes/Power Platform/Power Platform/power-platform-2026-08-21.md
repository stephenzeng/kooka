# Power Platform
**Date created:** 2026-08-21 UTC  
**Tags:** Analytics, Best Practices, Configuration, Consumption, Guidance, Monitoring  

## Major Changes

- **Business continuity and disaster recovery**

  Added comprehensive disaster recovery testing guidance, including clear distinctions between real DR and SSDR drills and a prescriptive validation checklist across platform, integration, analytics, operational readiness, documentation, and support. Expanded virtual network pairing guidance to require explicit failover and failback testing and validation. Updated FAQs to clarify managed environment licensing and billing language and streamlined terminology, folding the former “Document your business continuity plan” content into the new testing and validation guidance.

  https://learn.microsoft.com/en-us/power-platform/admin/business-continuity-disaster-recovery

## Moderate Changes

- **Power Platform inventory sample queries**

  Added UI-based guidance to identify an agent’s harness in the Power Platform admin center and noted that harness isn’t yet available in metadata, with interim fields to use for classification. Introduced a “List agents with their harness” section with a ready-to-run KQL query that returns one row per agent and an optional filter for GitHub Copilot harness agents.

  https://learn.microsoft.com/en-us/power-platform/admin/inventory-sample-queries

- **Power Platform inventory schema reference**

  Streamlined the Copilot Studio agents section by removing the inline API field table and directing readers to the external Microsoft Copilot Studio Agent inventory schema. This reduces duplication and keeps the reference aligned with the authoritative schema without introducing new fields.

  https://learn.microsoft.com/en-us/power-platform/admin/inventory-schema

- **Manage costs for agents powered by the GitHub Copilot harness**

  Reworked guidance to use the Harness column in the Power Platform admin center to identify GitHub Copilot harness agents, with step-by-step filtering instructions. Clarified harness values (GitHub Copilot, Standard, Copilot Chat), noted that only GitHub Copilot agents use consumption-based billing for all activity, and pointed to updated, ready-to-run inventory queries while the Harness value remains UI-only.

  https://learn.microsoft.com/en-us/power-platform/admin/manage-usage-github-copilot-harness