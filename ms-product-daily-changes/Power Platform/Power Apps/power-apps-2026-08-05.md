# Power Apps
**Date created:** 2026-08-05 UTC  
**Tags:** Administration, AI, Monitoring, Programming  

## New Articles

- **Power Apps CLI command reference**

  Introduced a comprehensive reference for the Power Apps CLI, covering command groups such as app, auth, connection, connector, and telemetry with parameters, usage, and examples. Centralizes guidance for creating and managing code apps, handling authentication, configuring connections, listing connectors, and managing telemetry. Includes prerequisites, notes, and guidance links to streamline adoption and standardize command usage across teams.

  https://learn.microsoft.com/en-us/power-apps/developer/code-apps/reference/cli

## Major Changes

- **Add a Dataverse action or function to a code app**

  Updated the guide to use the Power Apps CLI, replacing legacy npm-based commands with pa app workflows. Added clearer steps to discover operations (find-dataverse-api) and add them (add dataverse-api), including how definitions are pulled from Dataverse metadata and related files are regenerated. Clarified typing for parameters/returns, refreshed examples, and added guidance on updating operations and troubleshooting stale generated files.

  https://learn.microsoft.com/en-us/power-apps/developer/code-apps/how-to/add-dataverse-action-function

- **Add Power Automate flows to a code app**

  Migrated to the Power Apps CLI with new commands for listing, adding, removing, and pushing flows, replacing deprecated npm-based commands. Documented idempotent updates, OpenAPI download, and automatic generation of typed models/services and configuration updates. Added guidance for running locally and publishing, and clarified limitations and prerequisites for supported triggers and solution-aware flows.

  https://learn.microsoft.com/en-us/power-apps/developer/code-apps/how-to/add-flows

- **Create a connection from the Power Apps CLI**

  Rewrote the article to use pa connector list and pa connection create, replacing legacy commands. Clarified environment selection via power.config.json, updated option explanations, and described JSON outputs to help automate setup. Provided refreshed examples and links to related CLI references for consistent configuration.

  https://learn.microsoft.com/en-us/power-apps/developer/code-apps/how-to/create-connection

- **Create a code app by using the Power Apps CLI**

  Overhauled the quickstart to center on the Power Apps CLI, guiding users through creating a project with a Vite template, initializing with pa app init, running with pa app run, and publishing with pa app push. Removed deprecated npm CLI references and streamlined steps for a faster setup experience. Clarified local network access considerations and added links to related topics for data, actions/functions, flows, and CLI reference.

  https://learn.microsoft.com/en-us/power-apps/developer/code-apps/how-to/npm-quickstart

- **How to sign in and manage accounts with the Power Apps CLI**

  Replaced legacy authentication instructions with pa auth login, status, switch, and logout for modern account management. Clarified behavior with multiple or no accounts and standardized examples and terminology. Added links to initialization and reference topics to help developers quickly set up and switch contexts.

  https://learn.microsoft.com/en-us/power-apps/developer/code-apps/how-to/sign-in-manage-accounts

## Moderate Changes

- **Receive Azure Synapse Link for Dataverse notifications in Power Apps**

  Shifted monitoring guidance to the Synapse Link Profile Entity State table, especially for low-latency sync scenarios, and removed general reliance on external table state. Emphasized key columns and how to use LastSynchronizedOnTime with SyncLatencyMilliseconds to measure latency, including append-only behavior, to improve operational visibility.

  https://learn.microsoft.com/en-us/power-apps/maker/data-platform/azure-synapse-link-notifications

- **Choose finance and operations data in Azure Synapse Link for Dataverse**

  Updated monitoring guidance to rely on the Synapse Link Profile Entity State table for initialization and activation status instead of the external table state. Clarified event definitions for Initialize complete and Activated to set accurate expectations during table selection and initialization.

  https://learn.microsoft.com/en-us/power-apps/maker/data-platform/azure-synapse-link-select-FnO-data

- **Prompt columns in Microsoft Dataverse**

  Clarified when prompt columns execute and that test runs do not consume credits. Documented that prompt columns consume both AI Builder credits and Copilot Credits, and added step-by-step instructions to monitor credit usage via Power Automate’s Automation center with filtering and export options.

  https://learn.microsoft.com/en-us/power-apps/maker/data-platform/prompt-column