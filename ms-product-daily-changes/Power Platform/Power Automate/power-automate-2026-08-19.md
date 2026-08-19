# Power Automate
**Date created:** 2026-08-19 UTC  
**Tags:** Automation, Best Practices, Configuration, Guidance  

## New Articles

- **Call Microsoft Copilot Studio agents from Power Automate**

  Introduced a how-to guide for invoking Microsoft Copilot Studio agents from Power Automate cloud flows using the Copilot Studio connector. Explains support by agent harness: standard harness agents run in cloud flows, while GitHub Copilot harness agents are orchestrated inside Copilot Studio workflows via an agent node. Provides step-by-step instructions for the Execute Agent and wait action, including input options (locale, conversation ID, environment) and how to use outputs, plus an alternative non-blocking Execute Agent action. Also covers adding and configuring an agent node for GitHub Copilot harness agents and links to related guidance.

  https://learn.microsoft.com/en-us/power-automate/call-copilot-studio-agent

## Moderate Changes

- **Create an object‑centric event log**

  Expanded ingestion guidance to support delta tables in Fabric Lakehouse in addition to CSV sources, and renamed “Target CSV schema” to “Target schema.” Clarified modeling rules, step descriptions, and examples (including multi‑object references and attribute duplication) and standardized terminology for consistency, helping authors design cleaner, future-proof schemas.

  https://learn.microsoft.com/en-us/power-automate/object-centric-create-event-log

- **Ingest an object-centric event log**

  Removed the prior limitation about Fabric Lakehouses with schema support enabled, reflecting updated platform support. Clarified data source selection and mapping requirements for event/object attributes and mandatory fields to reduce ingestion errors.

  https://learn.microsoft.com/en-us/power-automate/object-centric-ingest-event-log

- **Export OCPM semantic model into Fabric workspace**

  Removed preview status and updated wording across the article to reflect general availability. Clarified guidance on column naming, relationships, composite model usage, and refresh behavior so teams can deploy and maintain the model with greater confidence.

  https://learn.microsoft.com/en-us/power-automate/object-centric-semantic-model

- **Normalized schema JSON authoring**

  Updated the guidance to GA by removing preview notes and refining instructions throughout. Clarified CSV requirements (including UTF‑8), rules for joins (no nested or chained), key placement, attribute levels, and Delta‑Parquet and OneLake/Fabric path conventions. Standardized terminology and warnings to help authors avoid common mistakes and produce reliable normalized imports.

  https://learn.microsoft.com/en-us/power-automate/process-mining-normalized-import-authoring-guide

- **Create a process from normalized schema**

  Reflected general availability by removing the preview label and notices. Made small wording improvements in prerequisites and mapping descriptions to streamline setup without changing procedures or feature behavior.

  https://learn.microsoft.com/en-us/power-automate/process-mining-normalized-import-ux-guide