# Power Query
**Date created:** 2026-08-21 UTC  
**Tags:** Best Practices, Configuration, Get Started, Guidance, Performance, Security  

## Major Changes

- **Best Practices When Working with Power Query**
  
  Extensively overhauled the best practices article with clearer guidance on selecting purpose-built connectors and improved data type recommendations. Revamped performance guidance with actionable sections (filter early, perform expensive steps last, and develop on a limited subset). Reworked data profiling coverage, strengthened modular design advice with query references and grouping, and expanded future-proofing scenarios with practical transformations. Enhanced sections on parameters and custom functions with clearer use cases and step-by-step context. Content was reorganized throughout for clarity and depth.

  https://learn.microsoft.com/en-us/power-query/best-practices

- **Overview of query evaluation and query folding in Power Query**
  
  Restructured the article to clearly separate query evaluation from query folding, and added guidance on what an M script is and how to edit it. Expanded the evaluation flow for external and non-external sources, clarified folding behavior and lazy evaluation, and defined outcomes (full, partial, none). Added practical instructions to verify folding in Power Query Online using step indicators, query plan, and native query views, and outlined which connectors support folding. Language and anchors were refined for consistency and easier navigation.

  https://learn.microsoft.com/en-us/power-query/query-folding-basics

## Moderate Changes

- **Power Query get data experience overview**
  
  Clarified differences between Desktop and Online stages, including connection settings, authentication, and destination behavior. Consolidated Navigator guidance (multi-select and object limits), refined the limitation workaround, and specified product-specific save/load commands across Excel, Power BI Desktop, Power Query Online, and Analysis Services. These updates help users choose the right path and execute load actions confidently across hosts.

  https://learn.microsoft.com/en-us/power-query/get-data-experience

- **What is Power Query?**
  
  Expanded the conceptual overview to clarify that Power Query transforms data while the hosting product controls where data is loaded, and distinguished Online vs. Desktop experiences (connectors, authentication, destinations, and host features). Strengthened explanations of transformations and dataflows, emphasizing repeatability and that source data isn’t modified. Added a comprehensive M example to illustrate real-world automation and how to work with code in Advanced Editor.

  https://learn.microsoft.com/en-us/power-query/power-query-what-is-power-query

- **Privacy Levels in Power Query**
  
  Expanded guidance on privacy level classifications, the Fast Combine option, and how privacy levels interact with folding and blocking scenarios. Provided explicit steps to set and verify privacy levels across Power Query Online, Power Query Desktop, Power BI Desktop, and Excel, with clearer dialogs and scope distinctions. Minor refinements improve accuracy and help users configure secure, predictable data movement.

  https://learn.microsoft.com/en-us/power-query/privacy-levels