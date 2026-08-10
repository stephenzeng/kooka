# Microsoft Fabric
**Date created:** 2026-07-13 UTC  
**Tags:** Administration, AI, Agent, Analytics, Automation, Other  

## New Articles

- **Insert Columns in PowerTable**

  Introduced end-to-end guidance for inserting columns in PowerTable during creation and after setup. Explains Visual, Database, and Formula columns, including how each impacts the source database and when to use them. Details supported column types (data, formula, lookup, reference, attachment, roll up, button) and their behaviors. Helps teams choose the right column approach for schema changes versus UI-only enhancements.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-how-to-insert-columns/how-to-insert-columns-introduction

- **Insert Database Columns in PowerTable**

  Added a step-by-step guide for creating database-backed columns directly from PowerTable with notes on required permissions. Covers selecting data types, configuring nullability, setting default values (manual or formula), and how defaults apply to existing versus new rows. Explains post-creation property configuration and confirms that changes synchronize to the source database. Enables governed, consistent schema updates without leaving the workspace.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-how-to-insert-columns/how-to-insert-database-column

- **Insert Visual Columns in PowerTable**

  Published guidance on adding visual columns that enrich sheets without altering the source database. Describes how to create visual columns and when to use Multiselect Relationship, Reference, Relation, Rollup, Button, and Attachment types. Helps builders extend UI and relationships safely without impacting underlying schemas.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-how-to-insert-columns/how-to-insert-visual-columns

- **Design Dashboards with Charts, KPIs, and Matrices**

  Introduced a comprehensive tutorial for building interactive dashboards in intelligence sheets. Walks through creating line and Marimekko charts, variance visuals, filters, matrices with automatic variance calculations, and formula columns for derived metrics. Includes steps for KPI cards, layout and styling, custom headers, and rich text comments to create polished, explainable dashboards.

  https://learn.microsoft.com/en-us/fabric/iq/plan/intelligence-how-to-create-dashboards

## Moderate Changes

- **Tutorial: Create and activate a Fabric Activator rule**

  Updated the tutorial to reflect UI and terminology changes from Data Activator to Activator, including renaming “Run User Data Function” to “Run Function.” Clarifies parameter passing with @property references, adds an explicit save step, and refines guidance for Teams and email actions and rule conditions. Improves accuracy and reduces setup friction for creating reliable activation rules.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/data-activator/activator-tutorial

- **Release status of AI and Copilot experiences in Fabric**

  Expanded capability descriptions across workloads, including notebook code generation and refactoring, diagnostics with approval-based fixes, data agents, AI functions/services, and Foundry Tools coverage. Added details for SQL experiences (Query Editor, SSMS, VS Code) with inline T-SQL, chat-based generation, and plan analysis, plus AI Auto-Summary for semantic models. Provides clearer scope and direct links to setup and usage guidance while retaining release statuses.

  https://learn.microsoft.com/en-us/fabric/fundamentals/copilot-ai-feature-state

- **What is Copilot in Fabric?**

  Replaced the embedded experience table with a single reference to the consolidated AI and Copilot release status page. Reduces duplication and keeps readers aligned with the most current list of capabilities and availability.

  https://learn.microsoft.com/en-us/fabric/fundamentals/copilot-fabric-overview