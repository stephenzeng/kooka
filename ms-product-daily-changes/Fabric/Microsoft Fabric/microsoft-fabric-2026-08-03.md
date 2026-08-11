# Microsoft Fabric
**Date created:** 2026-08-03 UTC  
**Tags:** Administration, Analytics, Automation, Monitoring, Other, Security  

## New Articles

- **Configure Workflow Triggers, Actions, and Conditions**

  Introduced a comprehensive how-to for building automation workflows in PowerTable. It covers configuring triggers (create, update, delete, form submit, button), a wide range of actions (create/update/delete records, find records, bulk create, stored procedures), and advanced logic with conditional and repeating groups. The article also explains how to manage automations (enable/disable, duplicate, delete), save workflows, and use run history with retry and refresh to monitor execution.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-how-to-create-automation/how-to-configure-automation-workflows

- **Build a Sample Automation in PowerTable**

  Added an end-to-end tutorial that implements an order-processing flow. It retrieves inventory, branches on stock availability, creates orders when possible, and updates inventory accordingly. It also handles out-of-stock cases by flagging items for restock and updating timestamps, with detailed configuration steps and screenshots.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-how-to-create-automation/how-to-create-sample-automation

- **PowerTable Frequently Asked Questions**

  New FAQ clarifying setup prerequisites and architecture. It explains required workspace roles to create items and databases, why a Fabric SQL database is needed before creating a sheet, and the purpose of the companion SQL analytics endpoint. It also covers naming considerations and links to feature-specific FAQs.

  https://learn.microsoft.com/en-us/fabric/iq/plan/resources/powertable-general-faq

- **PowerTable Sheets Creation FAQ**

  New FAQ detailing the sheet creation experience and data sourcing. It explains initial connection setup and authentication, reusing connections, and the difference between sheet edits and committed database changes. Guidance covers choosing existing versus new tables, importing structure, identity column behavior, supported file types, current Fabric SQL scope, and enabling SCD Type II/III.

  https://learn.microsoft.com/en-us/fabric/iq/plan/resources/powertable-sheets-creation-faq

- **Troubleshoot Spark application code, data, and library errors**

  New troubleshooting guide focused on application code, data transformations, and library/environment failures. It addresses Delta Lake and streaming exceptions, common user code errors, and package installation issues, with concrete remediation steps and Spark UI pointers. The guide includes code examples and links to related Spark troubleshooting topics.

  https://learn.microsoft.com/en-us/fabric/data-engineering/troubleshoot-spark-code-runtime-errors

- **Troubleshoot Spark memory and performance issues**

  Comprehensive guide for diagnosing executor failures and performance bottlenecks, including exit codes and common scenarios like OOM, data skew, and shuffle pressure. Provides actionable tuning steps for memory, partitions, AQE, timeouts, caching, broadcast joins, and Pandas UDFs, plus scaling guidance. Includes quick-reference configurations, anti-patterns to avoid, and notes on distinguishing platform infrastructure errors from workload issues.

  https://learn.microsoft.com/en-us/fabric/data-engineering/troubleshoot-spark-memory-performance

- **Troubleshoot Spark session, configuration, and platform errors**

  New guide for resolving session startup and submission failures, configuration missteps, and platform-level errors. It covers timeouts, Spark submit failures, service-enforced terminations, and invalid configuration patterns with clear corrective actions. Platform-specific issues like native execution engine and metastore errors are explained with workarounds and recovery steps.

  https://learn.microsoft.com/en-us/fabric/data-engineering/troubleshoot-spark-session-configuration-errors

- **Troubleshoot Spark SQL and schema errors**

  New guide addressing SQL behavior differences, cross-version compatibility, and common AnalysisException scenarios. It provides step-by-step fixes for missing tables/views, ambiguous or mismatched columns, schema write conflicts, and Delta-specific issues, with practical code/config examples. Targeted sections accelerate resolution for frequent errors such as “table or view not found” and Parquet schema inference failures.

  https://learn.microsoft.com/en-us/fabric/data-engineering/troubleshoot-spark-sql-schema-errors

- **Troubleshoot Spark storage, file, and authentication errors**

  New troubleshooting guide covering storage connectivity, file access, and authentication failures across ABFS, JDBC, mounted paths, and token providers. It maps common error codes to causes and actions, and provides diagnostic steps and command examples. The content includes quick-reference tables and links to related troubleshooting guides.

  https://learn.microsoft.com/en-us/fabric/data-engineering/troubleshoot-spark-storage-connectivity-errors

## Major Changes

- **Automation in PowerTable**

  Substantially expanded and reorganized the automation concepts to clarify capabilities and design patterns. Added detailed coverage of triggers, logic, and actions, including bulk operations and cascading updates. New sections illustrate basic and advanced workflows with conditional and repeating groups, plus guidance on next steps for configuration and samples.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-concept-automation

- **Edit and bulk edit data**

  Overhauled guidance with a comprehensive FAQ on editing workflows and commit behavior. Clarifies pending changes versus database saves, how to configure and apply multiple bulk actions, and how to preview and selectively undo batched edits. Explains when to use row/form editors vs. bulk edit vs. find/replace, and details what is captured in data versus access audit tabs.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-how-to-bulk-edit-data

- **Spark errors overview in Microsoft Fabric**

  Reframed from an all-in-one troubleshooting page to a concise overview that routes readers to specialized articles. Removed embedded deep-dive sections and introduced a simpler category table linking to new guides for memory/performance, SQL/schema, storage/connectivity/auth, session/configuration/platform, and application code/data/library issues. Related content was updated to reflect the new structure.

  https://learn.microsoft.com/en-us/fabric/data-engineering/troubleshoot-spark

## Moderate Changes

- **Mirror Azure Monitor in Microsoft Fabric (preview)**

  Updated security guidance to require a custom role for creating connections and aligned the roles table accordingly. Clarified that connections run under the selected authentication mode and outlined operational implications for organizational accounts.

  https://learn.microsoft.com/en-us/fabric/mirroring/catalog-mirroring/azure-monitor

- **Tutorial: Configure the Mirror Azure Monitor solution in Microsoft Fabric (preview)**

  Revised prerequisites and permission steps to use a dedicated custom role for connection creation, with alternatives for applicable built-in roles. Updated authentication and workspace identity guidance, including cross-tenant service principal requirements for connection access.

  https://learn.microsoft.com/en-us/fabric/mirroring/catalog-mirroring/azure-monitor-tutorial

- **Configure display properties for a column**

  Added an FAQ clarifying that changing the Display Name only affects the sheet label and doesn’t rename the database column. Documented how the Description field appears on hover to convey business context and definitions.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-how-to-configure-columns/how-to-configure-display-column-properties

- **Configure general properties for a column**

  Introduced an FAQ distinguishing Input Type (UI) from Data Type (SQL). Clarified that Image input type changes display only and supports URLs or Base64 strings, and that default values apply to new records without altering existing rows.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-how-to-configure-columns/how-to-configure-general-column-properties

- **Configure single select column in a PowerTable sheet**

  Added FAQs explaining how distinct values, user-added options, and lookup scopes work, and what gets stored (keys vs. display values). Guidance also covers self-referential lookups, hierarchical dropdowns, and dependent filters between columns.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-how-to-configure-columns/how-to-configure-lookup-relation-columns

- **Insert formula columns in PowerTable**

  Added an FAQ explaining why pasting formulas isn’t supported and how to reference columns during typing with Ctrl+Space. Clarified persistence and when formulas write to the database versus recalculating in the sheet.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-how-to-insert-columns/how-to-insert-formula-columns

- **Apply conditional formatting in PowerTable**

  Added an FAQ on when to apply formatting to entire rows versus individual cells. Clarified where rules are stored and how they can be toggled without deletion.

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-how-to-apply-conditional-formatting

- **Insert, import, duplicate, and delete rows**

  Added an FAQ detailing form-based vs. grid insert behavior, inserting multiple blank rows, and how Apply stages pending changes. Clarified Bulk Edit scope and how imports classify rows into insert, update, and error categories before committing. 

  https://learn.microsoft.com/en-us/fabric/iq/plan/powertable-how-to-insert-rows-import-data

## Minor Changes