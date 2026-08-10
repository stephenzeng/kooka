# Microsoft Fabric
**Date created:** 2026-07-15 UTC  
**Tags:** Administration, AI, Analytics, Automation, Governance, Monitoring, Other, Programming  

## New Articles

- **Insert Attachment Columns in PowerTable Sheet**

  Introduced a step-by-step guide to add attachment columns in PowerTable, including purpose, use cases, and key limits like 25 MB per file and multiple files per record. Clarifies that access is enforced by row-level permissions and that only users with record access can view attachments. Provides detailed procedures to insert the column and upload one or more files, with a link to supported file types.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-how-to-insert-columns/how-to-insert-attachment-columns

- **Insert Button Columns in PowerTable Sheet**

  Added instructions for creating and configuring button columns to automate user actions. Explains how to set labels and actions, open static or formula-driven URLs, and trigger existing or new automations from a sheet. Includes screenshots and guidance to save and apply settings for consistent behavior.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-how-to-insert-columns/how-to-insert-button-columns

- **Insert Formula Columns in PowerTable Sheet**

  Published a how-to for adding formula columns using the built-in editor and context assistant for functions and references. Details formatting options such as currency and decimal precision, and how to materialize formulas as physical database columns with proper types and permissions. Helps users build calculated insights directly in PowerTable.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-how-to-insert-columns/how-to-insert-formula-columns

- **Insert Reference Columns in PowerTable Sheet**

  Introduced guidance to configure reference columns that display values from another table. Covers selecting schema/table/column, mapping records with chosen match keys, and using “Match multiple” when many results are expected. Clarifies that reference columns are read-only and update automatically as source data changes, with tips for display configuration.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-how-to-insert-columns/how-to-insert-reference-columns

- **Apply Conditional Formatting in PowerTable Sheet**

  Added a tutorial to build and manage conditional formatting rules at column or row scope. Explains configuring conditions and styles, combining multiple conditions with AND/OR, and using prefixes/suffixes for column-scoped formats. Includes instructions to view, edit, duplicate, enable/disable, and delete rules for ongoing maintenance.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-how-to-apply-conditional-formatting

- **Audit Logs in PowerTable**

  Introduced comprehensive audit and writeback logging, with searchable and filterable views across data, access, and table changes. Details exporting logs, refreshing, and using Revert Changes to roll back updates, including behavior for sequential edits and unsupported scenarios. Adds a Writeback Logs page with rich transaction metadata and optional “Last Updated Details” columns to track recent edits.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-how-to-view-audit-logs

## Major Changes

- **Introduction to CI/CD in Microsoft Fabric**

  Rewrote the article from an ALM overview into a comprehensive CI/CD guide centered on Fabric REST APIs. Added platform overview, enterprise reference architecture, and integration and delivery layers (Git integration, deployment pipelines, variable library). Expanded coverage of source control and CI automation across GitHub and Azure DevOps with service principals, plus tooling and IaC options (Fabric CLI, Terraform, fabric-cicd). Improved deployment guidance for Git-connected workspaces, added diagrams, and refreshed related links to new CI/CD resources.

  https://learn.microsoft.com/en-us/fabric/cicd/cicd-overview

- **Customize AI Functions with pandas**

  Consolidated and expanded configuration guidance for AI Functions, separating global and per-function settings for LLMs and embeddings with clear code samples. Clarified custom endpoint setup using OpenAI-compatible /openai/v1 endpoints, including api_type selection (responses for OpenAI models, chat_completions for non-OpenAI Foundry), JSON schema requirements for response_format, and limitations such as no support for ai.embed or ai.similarity with custom Foundry resources. Added scenarios for routing via Azure API Management with subscription keys and optional deployment targeting, and updated examples and placeholders accordingly.

  https://learn.microsoft.com/en-us/fabric/data-science/ai-functions/pandas/configuration

- **Microsoft Fabric site reliability engineering (SRE) model**

  Substantially restructured and expanded the SRE guidance to deepen coverage of service monitoring, incident response, and continuous improvement. Added a “Stay informed about service issues” section with status/health messages, in-product banners (preview), Teams and email notifications (preview), and a Service Health dashboard, including admin controls. Clarified SLI/SLO prerequisites, enhanced alerting practices, and automation patterns, and detailed incident workflows like TTN0 notifications, tiered engagement, and mitigation techniques. Updated terminology and examples to improve accuracy and relevance.

  https://learn.microsoft.com/en-us/fabric/enterprise/fabric-site-reliability-engineering-model

## Moderate Changes

- **Delta change data feed in mirroring for Fabric**

  Removed the folder structure section that previously described OneLake layout details when CDF is enabled, including the _change_data folder and Parquet record schema. This streamlines the article and reduces reliance on internal layout specifics that can change.

  https://learn.microsoft.com/en-us/fabric/mirroring/extended-capabilities-delta-change-data-feed

- **AI Functions: Transform data at scale with AI**

  Updated the overview to state that Dataflow Gen2 and Data Warehouse SQL now use the same base model (gpt-5-mini) with low reasoning effort. This clarifies current behavior and sets consistent expectations for model performance across services.

  https://learn.microsoft.com/en-us/fabric/data-science/ai-functions/overview