# Power Apps
**Date created:** 2026-08-20 UTC  
**Tags:** Automation, Best Practices, Configuration, Get Started, Guidance, Licensing, Security, Troubleshooting  

## Major Changes

- **How to: Application Lifecycle Management (ALM) for code apps**

  Substantially expanded ALM guidance for code apps with end-to-end steps using the Power Apps CLI, including publishing via pa app push. Clarifies automatic solution selection, how to explicitly target a solution with --solution-id, and how to validate or discover the solution ID. Details first vs. subsequent publish behavior, adding apps to solutions, and CI/CD usage via a SOLUTION_ID variable. Updates prerequisites for initialized apps and notes requirements for environments without Dataverse.

  https://learn.microsoft.com/en-us/power-apps/developer/code-apps/how-to/alm

- **Quickstart: Create a Code App Using the Power Apps CLI**

  Overhauled the quickstart to center on the Power Apps CLI workflow from project creation through publish. Adds clear steps for pa app init (interactive or inline), local run with pa app run, and publishing with pa app push. Removes legacy PAC CLI auth/environment steps and clarifies local network and browser profile considerations. Links to next steps for data connections, Dataverse, flows, and CLI reference.

  https://learn.microsoft.com/en-us/power-apps/developer/code-apps/how-to/create-an-app-from-scratch

- **How to: Create and Manage Connections with the Power Apps CLI**

  Expanded from basic connection creation to a comprehensive guide for creating, discovering, and managing connections and data sources using the Power Apps CLI. Adds practical SQL and SharePoint examples, covering datasets, tables, and stored procedures, plus remove/refresh commands. Introduces solution-based connection references for ALM and shows how to update apps to use generated models and services. Includes run/publish steps and tips to ensure correct parameters.

  https://learn.microsoft.com/en-us/power-apps/developer/code-apps/how-to/create-connection

- **Manage Telemetry Settings for the Power Apps CLI**

  Retitled and refocused guidance to manage telemetry via pa telemetry enable/disable/status with examples and a command table. Explains configuration through userSettings.json, including properties and OS-specific setup scripts. Describes telemetry modes (remote, remote + console, console only), piping console output to files, and updated examples using pa commands. Improves structure and terminology and adds a link to the CLI reference.

  https://learn.microsoft.com/en-us/power-apps/developer/code-apps/how-to/telemetry

## Moderate Changes

- **Power Apps Code Apps Architecture for Development and Runtime**

  Updated architecture guidance to use the Power Apps CLI and the pa app push command. Improves terminology and section organization and refines alt text to clarify development and runtime concepts.

  https://learn.microsoft.com/en-us/power-apps/developer/code-apps/architecture

- **Power Apps CLI Command Reference**

  Added a Global options section explaining --help usage at any command level and guidance for pa --version. Streamlined intros, reorganized headings, and removed specific package version lists to keep the reference focused and current.

  https://learn.microsoft.com/en-us/power-apps/developer/code-apps/reference/cli

- **How to: Connect your code app to Azure SQL**

  Shifted the connection setup to the Power Apps CLI and updated all commands to the pa syntax. Shows creating the SQL connection via shared_sql, saving the connection ID, adding the data source with explicit flags, and publishing with pa app push.

  https://learn.microsoft.com/en-us/power-apps/developer/code-apps/how-to/connect-to-azure-sql

- **How to: Connect to Copilot Studio**

  Migrated steps to a CLI-first workflow using pa connection list and pa app add data-source. Replaces maker portal steps with CLI connection creation using shared_microsoftcopilotstudio and aligns phrasing and references accordingly.

  https://learn.microsoft.com/en-us/power-apps/developer/code-apps/how-to/connect-to-copilot-studio

- **How to: Connect Your Code App to Dataverse**

  Updated to the new pa app add data-source syntax and clarified prerequisites for using the Power Apps CLI with initialized code apps. Explains adding tables and using generated services for CRUD, and removes outdated PAC CLI limitations.

  https://learn.microsoft.com/en-us/power-apps/developer/code-apps/how-to/connect-to-dataverse

- **Complex tables requiring Power Apps licenses | Microsoft Docs**

  Updated the list of Dynamics 365 apps that install complex tables, replacing Marketing and Project Service Automation with Customer Insights and Project Operations. Ensures licensing references reflect current app names.

  https://learn.microsoft.com/en-us/power-apps/maker/data-platform/data-platform-complex-entities

- **Combo box modern control in canvas apps**

  Revised Appearance options by removing Appearance.Filled and adding Appearance.FilledLighter, with Appearance.FilledDarker clarified as the default. Refines the Outline description to note a transparent background and consolidates default notes.

  https://learn.microsoft.com/en-us/power-apps/maker/canvas-apps/controls/modern-controls/modern-control-combobox

- **Date picker modern control in canvas apps**

  Updated the Appearance table to replace Appearance.Filled with Appearance.FilledLighter while retaining Appearance.FilledDarker as the default. Clarifies that Appearance.Outline uses an outlined border with a transparent background.

  https://learn.microsoft.com/en-us/power-apps/maker/canvas-apps/controls/modern-controls/modern-control-date-picker

- **Dropdown modern control in canvas apps**

  Replaced Appearance.Filled with Appearance.FilledLighter and clarified that FilledDarker is the default. Refined descriptions for how FilledDarker, FilledLighter, and Outline affect background and transparency.

  https://learn.microsoft.com/en-us/power-apps/maker/canvas-apps/controls/modern-controls/modern-control-dropdown

- **Number Input modern control in canvas apps**

  Updated Appearance options to use Appearance.FilledLighter instead of Appearance.Filled and clarified the FilledDarker description. Aligns documentation with the current property values.

  https://learn.microsoft.com/en-us/power-apps/maker/canvas-apps/controls/modern-controls/modern-control-number-input

- **Text Input modern control in canvas apps**

  Replaced the Appearance.Filled option with Appearance.FilledLighter and clarified descriptions, noting FilledDarker as the default. Ensures property guidance matches the latest control behavior.

  https://learn.microsoft.com/en-us/power-apps/maker/canvas-apps/controls/modern-controls/modern-control-text-input

- **Recent updates to modern controls in canvas apps**

  Updated the Appearance enum to remove Appearance.Filled and add Appearance.FilledLighter. Clarifies that FilledDarker is typically the default and refines descriptions to match actual options.

  https://learn.microsoft.com/en-us/power-apps/maker/canvas-apps/controls/modern-controls/modern-control-updates

- **Power Apps code apps overview**

  Clarified the purpose and scope of code apps and streamlined prerequisites to focus on IDE, Node.js, npm, Git, and the Power Apps CLI. Removed references to deprecated npm-based CLI notes and improved image alt text.

  https://learn.microsoft.com/en-us/power-apps/developer/code-apps/overview

- **Troubleshoot Adding a Data Source**

  Rewrote troubleshooting to align with the Power Apps CLI, including updated pa commands for data sources and auth. Adds stepwise validation (configuration, environment, parameters), expands network/security checks, and improves guidance for traffic analysis and escalation details.

  https://learn.microsoft.com/en-us/power-apps/developer/code-apps/troubleshoot-add-datasource

- **Troubleshoot Power Apps CLI Issues with Zscaler**

  Updated guidance to use pa commands and added a secure validation flow for certificates and NODE_EXTRA_CA_CERTS. Emphasizes avoiding insecure workarounds, refines troubleshooting scenarios, and updates allowlisting and escalation requirements.

  https://learn.microsoft.com/en-us/power-apps/developer/code-apps/troubleshoot-zscaler-issues

- **How to: Use Environment Variables in Code App Data Sources**

  Updated instructions to the new pa app add data-source syntax with revised flags and pa app init for setup. Emphasizes avoiding hardcoded values and enabling ALM across environments.

  https://learn.microsoft.com/en-us/power-apps/developer/code-apps/how-to/use-environment-variables

- **Use IFRAME and Web Resource Controls in Model-Driven Apps**

  Expanded security guidance for IFRAMEs, including sandbox behavior when restricting cross-frame scripting. Reworked cross-origin communication using postMessage with targetOrigin and origin validation, and clarified CSP frame-ancestors and X-Frame-Options requirements while removing outdated Silverlight guidance.

  https://learn.microsoft.com/en-us/power-apps/developer/model-driven-apps/use-iframe-and-web-resource-controls-on-a-form