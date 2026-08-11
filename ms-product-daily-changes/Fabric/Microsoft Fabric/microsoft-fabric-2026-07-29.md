# Microsoft Fabric
**Date created:** 2026-07-29 UTC  
**Tags:** Administration, Analytics, Governance, Monitoring, Other, Programming, Security  

## New Articles

- **Configure Hierarchy Layout in PowerTable**

  Introduced a step-by-step guide to configure and work with the Hierarchy layout in PowerTable. Explains selecting Primary Key, Hierarchy, and Display columns and how these settings drive pinned columns, parent-child structure, and expand/collapse behavior. Details managing records, inserting child rows with auto-filled hierarchy values, moving items between parents, and viewing full hierarchy paths, with screenshots to aid setup and usage.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-layouts/how-to-configure-hierarchy-layout

- **SQL Queries**

  Added documentation for creating SQL-based queries in Infobridge that generate new queries without altering the originals. Provides UI steps to start a SQL Query, reference existing queries, and build a sample query using query references. Highlights how the resulting query appears in the Queries list and how the Query References pane supports authoring.

  https://learn.microsoft.com/en-us/fabric/iq/plan/infobridge-transform-queries/how-to-sql-query

- **Comments and Collaboration in PowerTable**

  Introduced guidance on PowerTable commenting and collaboration, including adding comments to cells, rows, and columns with @mentions and Teams notifications. Covers threaded replies, resolve/reopen, a dedicated Comments column with Status and Assignee, and viewing all comments in a centralized panel. Explains configuration options (indicators, notifications, delete/reset) and how security roles govern who can view, add, or star comments.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-how-to-add-comments

## Moderate Changes

- **[!INCLUDE [fabric-activator](../includes/fabric-activator.md)] limitations**

  Updated Teams notifications guidance: only recently active group chats can be selected and Teams channels are not supported. Removed prior references to shared channels while keeping the restriction that private channels can’t receive messages, helping users avoid unsupported destinations.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/data-activator/activator-limitations

- **Aggregation and Statistical Functions**

  Removed preview status to reflect general availability and updated descriptive text accordingly. Functional guidance and examples remain the same for continuity.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-reference-formulas/math-functions/aggregation-statistical-functions

- **Arithmetic Functions**

  Updated to general availability by removing all preview references and note includes. The function descriptions and examples are unchanged.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-reference-formulas/math-functions/arithmetic-functions

- **Conditional Statements**

  Reflects GA by removing preview labels and the preview note. No changes to behavior or examples.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-reference-formulas/conditional-statements

- **Date functions: Create, format, and convert dates**

  Removed preview indicators to mark general availability. Content and guidance remain intact.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-reference-formulas/date-functions/create-format-convert-dates

- **Exponential and Logarithmic Functions**

  De-previewed the content to indicate GA and removed preview note includes. Functional descriptions and examples are unchanged.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-reference-formulas/math-functions/exponential-logarithmic-functions

- **Financial Functions**

  Updated to GA by removing the preview note and labels. No changes to the functional guidance.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-reference-formulas/math-functions/financial-functions

- **Append queries in Infobridge**

  Removed the preview note to reflect GA for Append Query. Instructions and capabilities are unchanged.

  https://learn.microsoft.com/en-us/fabric/iq/plan/infobridge-transform-queries/how-to-append-query

- **Insert button columns in PowerTable**

  De-previewed the feature by removing the preview note. Procedures remain the same.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-how-to-insert-columns/how-to-insert-button-columns

- **Introduction to inserting PowerTable columns**

  Removed the preview note to indicate GA. Instructional content is unchanged.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-how-to-insert-columns/how-to-insert-columns-introduction

- **Insert data input columns in planning sheet**

  Updated to GA by removing preview wording and note includes. No procedural changes.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-how-to-insert-columns/how-to-insert-data-input-columns

- **Insert formula columns in PowerTable**

  Consolidated update reflecting GA by removing preview indicators and the preview note. No changes to the how-to steps beyond status clarification.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-how-to-insert-columns/how-to-insert-formula-columns

- **Write back transformed data from Infobridge**

  Marked Infobridge in Plan as GA by removing preview labels and note includes. Guidance continues to support direct writeback to Microsoft Fabric SQL without behavioral changes.

  https://learn.microsoft.com/en-us/fabric/iq/plan/infobridge-how-to-write-back-data

- **Infobridge in Plan**

  Updated to GA by removing preview labels and notes, with minor wording adjustments. Functional description remains consistent.

  https://learn.microsoft.com/en-us/fabric/iq/plan/infobridge-overview

- **Intelligence Sheets in Plan**

  De-previewed the article by removing preview from title and content. Keeps the same no-code reporting and planning integration guidance.

  https://learn.microsoft.com/en-us/fabric/iq/plan/intelligence-overview

- **Microsoft Spark Utilities (MSSparkUtils) for Fabric**

  Added a Lakehouse utilities section for mssparkutils.lakehouse with overview and examples for create, get, update, delete, and list operations. Improves developer guidance for programmatically managing Lakehouse artifacts.

  https://learn.microsoft.com/en-us/fabric/data-engineering/microsoft-spark-utilities

- **Govern Fabric data**

  Expanded Recommended actions to let data owners in My items view all related entities for an action and open them with one click. Updated screenshots for admins and data owners to reflect the enhanced experience, improving discoverability and governance workflows.

  https://learn.microsoft.com/en-us/fabric/governance/onelake-catalog-govern

- **What Is Plan?**

  Removed all preview labels and the preview callout to reflect GA. Updated availability to note Plan in Fabric IQ is now worldwide under the Microsoft Fabric SKU and that new billing meters are billable.

  https://learn.microsoft.com/en-us/fabric/iq/plan/overview

- **Known Limitations in Plan**

  Converted from preview to GA by removing preview labels and callouts. No changes to the listed limitations.

  https://learn.microsoft.com/en-us/fabric/iq/plan/overview-limitations

- **Prerequisites for Plan**

  De-previewed tenant settings and text, updating references from “(preview)” to GA language. Steps and requirements remain the same.

  https://learn.microsoft.com/en-us/fabric/iq/plan/overview-prerequisites

- **Region Availability for Plan**

  Updated to GA and simplified guidance by removing the explicit “Unsupported regions” list. Now states availability across all Fabric-supported regions and directs readers to the Fabric region availability page for the authoritative list.

  https://learn.microsoft.com/en-us/fabric/iq/plan/overview-regions

- **User Roles in Plan**

  Removed preview status and note includes to reflect GA. Role definitions and capabilities are unchanged.

  https://learn.microsoft.com/en-us/fabric/iq/plan/overview-roles

- **What is a cube?**

  Removed the preview note to reflect GA with no functional changes. The conceptual guidance remains as before.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-concept-cube

- **Row-Level Security (RLS) Behavior in Fabric Plan**

  Updated to GA by removing preview references and the preview note. Clarified wording that RLS applies in Plan and that connections use embedded tokens, aligning terminology without changing behavior.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-concept-row-level-security

- **Configure advanced settings**

  Removed the preview note from writeback advanced settings to reflect GA. No changes to configuration steps.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-writeback/planning-how-to-configure-advanced-settings

- **Export Data from Planning Sheets**

  De-previewed the article by removing the preview note and labels. Export steps are unchanged.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-how-to-export-data

- **Create a planning sheet**

  Updated to GA by removing preview references and revising instructions to create a Plan item. Noted global availability under the Microsoft Fabric SKU and that new billing meters are now enabled.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-how-to-get-started

- **Insert blank rows**

  Reflected GA by removing preview labels and the preview note. Functionality and steps remain the same.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-how-to-insert-rows-blank

- **Insert data input rows**

  Removed preview designation and note to indicate GA. The insertion process is unchanged.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-how-to-insert-rows-data-input

- **Manage inserted rows**

  De-previewed the feature by removing the note and preview labels. Procedures are unchanged.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-how-to-manage-inserted-rows

- **Set up writeback to persist data**

  Updated to GA by removing preview references and the preview note. The writeback setup steps remain the same.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-writeback/planning-how-to-persist-data

- **Analyze planning outcomes with scenarios**

  Removed the preview note to indicate GA for scenarios. No modifications to the procedures.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-how-to-set-up-scenarios

- **Planning Sheets in Plan**

  Converted to GA by removing preview labels and the preview note. Structure and guidance are unchanged.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-overview

- **Apply conditional formatting in PowerTable**

  De-previewed the feature by removing the preview note. Steps and behavior remain consistent.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-how-to-apply-conditional-formatting

- **Configure display and formatting settings in PowerTable**

  Removed the preview note to reflect GA. No instructional changes.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-how-to-configure-display-formatting-settings

- **Group rows in PowerTable**

  De-previewed Group By by removing the preview note. No changes to functionality or steps.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-how-to-group-rows

- **Random and Lookup Functions**

  Updated to GA by removing preview references and the preview note. Functional guidance is unchanged.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-reference-formulas/math-functions/random-lookup-functions

- **Fabric region availability**

  Updated the regions table to remove “Plan (preview)” from Not available lists in several regions, signaling expanded availability. Regions such as East US 2, South Central US, Australia East, and Japan West no longer list Plan as unavailable.

  https://learn.microsoft.com/en-us/fabric/admin/region-availability

- **Rounding and Formatting Functions**

  Reflected GA by removing preview labels and the feature note. No changes to function behavior or examples.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-reference-formulas/math-functions/rounding-formatting-functions

- **Tenant settings index**

  Updated tenant settings descriptions to remove “(preview)” from Plan-related settings, reflecting GA. No changes to the underlying capabilities.

  https://learn.microsoft.com/en-us/fabric/admin/tenant-settings-index

- **Text Formatting Functions**

  De-previewed the page by removing preview labels and note. Functional content remains the same.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-reference-formulas/text-functions