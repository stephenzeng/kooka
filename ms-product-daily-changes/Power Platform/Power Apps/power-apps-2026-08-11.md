# Power Apps
**Date created:** 2026-08-11 UTC  
**Tags:** Analytics, Automation, Best Practices, Configuration, Get Started, Guidance, Monitoring, Performance, Troubleshooting  

## Major Changes

- **Create and Update Table Definitions Using the Web API**

  Expanded and clarified the end-to-end process for creating and updating Dataverse table definitions, including required properties and ensuring the primary name column is included. Updated guidance on label handling with MSCRM.MergeLabels and associating components to solutions with MSCRM.SolutionUniqueName. Added comprehensive examples with complete bodies, explicit label structures, and LogicalName-based updates, plus notes on preserving localized labels and publishing via PublishXml. Included references to SDK alternatives in .NET and Python to help developers choose the right tooling.

  https://learn.microsoft.com/en-us/power-apps/developer/data-platform/webapi/create-update-entity-definitions-using-web-api

- **Manage Microsoft Dataverse Customer Tables**

  Deepened guidance on account, contact, and customeraddress relationships, with clearer explanations of embedded versus non-embedded address records and key columns. Introduced admin controls to disable empty address creation and enable address deletion, with detection scripts and bulk delete automation using PAC CLI, SDK, Web API, and PowerShell. The updates make large-scale address data governance and clean-up more reliable and repeatable.

  https://learn.microsoft.com/en-us/power-apps/developer/data-platform/customer-entities-account-contact

- **Customize Table Definitions (Microsoft Dataverse) | Microsoft Docs**

  Restructured the article and added coverage for the Dataverse SDK for Python, including an operations matrix and notes on unsupported Python scenarios. Consolidated CRUD guidance, enhanced creation option explanations, and clarified capability behaviors (including that certain capabilities can’t be disabled once enabled). Updated links to related topics and removed outdated items to streamline planning and implementation.

  https://learn.microsoft.com/en-us/power-apps/developer/data-platform/customize-entity-metadata

## Moderate Changes

- **Azure Synapse Link Advance Configuration**

  Clarified that Append only mode supports only the Year partitioning strategy and other strategies aren’t honored. This helps prevent mispartitioned writes that could cause data inconsistencies and unreliable downstream processing.

  https://learn.microsoft.com/en-us/power-apps/maker/data-platform/azure-synapse-link-advanced-configuration

- **Compose HTTP Requests and Handle Errors**

  Added guidance for retrieving the Web API URL from the discovery service and expanded HTTP header usage, including options to bypass business logic for bulk operations, control label merging, enforce session consistency for elastic tables, and suppress callback jobs. These updates improve performance, reduce unintended side effects, and provide clearer patterns for solution-aware operations.

  https://learn.microsoft.com/en-us/power-apps/developer/data-platform/webapi/compose-http-requests-handle-errors

- **Create Custom Messages in Microsoft Dataverse**

  Added a rationale-focused section on when to use Custom APIs instead of Custom Process Actions, emphasizing a plugin-based pattern without workflow designer dependencies. Refined comparisons and language to help makers choose the right extensibility model.

  https://learn.microsoft.com/en-us/power-apps/developer/data-platform/custom-actions

- **Create and edit generative pages with AI code generation tools**

  Refocused guidance to recommend GitHub Copilot CLI as the primary AI code generation approach, highlighting benefits like access to the latest models, broad availability, and generating multiple pages and tables in one run. Clarified how this complements the in-browser experience and standardized terminology around the Power Apps skill.

  https://learn.microsoft.com/en-us/power-apps/maker/model-driven-apps/generative-page-external-tools

- **Generate a page using natural language**

  Reorganized the “how to build” section and introduced AI code generation tools (e.g., GitHub Copilot CLI) as a recommended path with clear benefits for code-first workflows. Added a link to deeper guidance and clarified the in-browser authoring experience, its audience, and regional availability.

  https://learn.microsoft.com/en-us/power-apps/maker/model-driven-apps/generative-pages

- **Explore data on a grid page**

  Added multiselect filtering for additional column types, including common text fields like Name and Phone Number, while clarifying existing behavior for lookup-style columns. Updated visuals to demonstrate the new filtering experience.

  https://learn.microsoft.com/en-us/power-apps/user/grid-filters

- **Troubleshoot Canvas Apps if Live Monitor Is Unsupported**

  Added methods to capture intermittent issues for later analysis, including recommended identifiers and contextual fields. Provided Power Fx examples for trace telemetry and Patch-based logging to Dataverse/SharePoint, with setup guidance and best practices for safe, manageable logging.

  https://learn.microsoft.com/en-us/troubleshoot/power-platform/power-apps/create-and-use-apps/monitor-alternatives-canvas-apps

- **How to: Get context data**

  Documented a new context property, dataverseOrgUrl, and updated examples to show how to access it via ctx.app.dataverseOrgUrl. This enables apps to reliably reference the environment’s Dataverse URL.

  https://learn.microsoft.com/en-us/power-apps/developer/code-apps/how-to/retrieve-context

- **Reference Dataverse schema definitions by name or MetadataId**

  Clarified that you no longer need to expand both OptionSet and GlobalOptionSet to retrieve option definitions, and updated examples to reflect current responses and additional option properties. The guidance simplifies how to reference tables, columns, relationships, and choices by name or MetadataId.

  https://learn.microsoft.com/en-us/power-apps/developer/data-platform/webapi/retrieve-metadata-name-metadataid