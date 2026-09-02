# Power Apps
**Date created:** 2026-09-02 UTC  
**Tags:** Automation, Best Practices, Configuration, Get Started, Guidance, Monitoring, Performance, Security, Troubleshooting  

## New Articles

- **Power Apps CLI environment variables**

  Introduced a comprehensive reference for all PA_CLI_* environment variables, including how they map to CLI options and their precedence relative to command-line arguments, defaults, and prompts. The article includes secure handling guidance for secrets, plus PowerShell and Bash examples for setting variables. It catalogs variables across authentication, global options, app initialization, running and sharing apps, solutions/connectors/data sources, Dataverse APIs and Power Automate flows, and telemetry/output controls, helping teams standardize CI/CD and local workflows.

  https://learn.microsoft.com/en-us/power-apps/developer/code-apps/reference/environment-variables

## Major Changes

- **Power Apps CLI command reference**

  Added a new “pa solution” command group with “pa solution list,” including search, JSON output, pagination, and an environment variable for filtering. Expanded “pa app init” with parameters for description, entry point, app type, and app URL, and added “--org-url” to “pa app add data-source” to streamline setup. Documented broad environment variable mappings across many commands (apps, auth, connections, connectors, flows, Dataverse APIs) for automation and consistency. Linked to the new environment variables reference to centralize configuration and governance.

  https://learn.microsoft.com/en-us/power-apps/developer/code-apps/reference/cli

- **Create and edit canvas apps with AI code generation tools**

  Removed preview status and reworked the guidance to reflect general availability and modern coding agents that support MCP servers. Clarified prerequisites: create the app first, save it in the target environment, and enable coauthoring before connecting from an AI tool. Shifted installation to marketplace-based agent plugins (including VS Code steps), added the unified /canvas-app skill and new /add-data-source, and provided fallback steps when commands aren’t available. Greatly expanded troubleshooting (SDK checks, correct Studio URL, plugin issues, missing resources) and added Security considerations to align with organizational policies.

  https://learn.microsoft.com/en-us/power-apps/maker/canvas-apps/create-canvas-external-tools

## Moderate Changes

- **How to: Application Lifecycle Management (ALM) for code apps**

  Updated guidance to use the PA_CLI_SOLUTION_ID environment variable when targeting a solution, replacing SOLUTION_ID. Revised the --solution-id option description and CI/CD examples to reflect the new variable, improving consistency with the CLI’s environment variable conventions.

  https://learn.microsoft.com/en-us/power-apps/developer/code-apps/how-to/alm

- **Component library**

  Refreshed step-by-step guidance and UI references for creating, saving, publishing, and updating component libraries, including use of the Save and Publish icons and visibility of version notes. Clarified customization behavior and local copy implications, refined import and multi-select flows, and added a proactive “Check for updates” action. Documented limitations such as downloaded copies not being importable and reinforced considerations when deleting referenced libraries.

  https://learn.microsoft.com/en-us/power-apps/maker/canvas-apps/component-library

- **Overview of creating performant apps**

  Expanded performance considerations to include client/device characteristics, geography, and on-premises data gateway location. Added links to Monitor for canvas apps and overall app performance telemetry to help makers diagnose and track performance issues in production.

  https://learn.microsoft.com/en-us/power-apps/maker/canvas-apps/create-performant-apps-overview

- **How to: Get context data**

  Documented a new app context property, appUrl, and updated the code sample to demonstrate reading ctx.app.appUrl. The IAppContext table now includes appUrl, enabling scenarios that require referencing the app’s URL at runtime.

  https://learn.microsoft.com/en-us/power-apps/developer/code-apps/how-to/retrieve-context

- **Get started with formulas in canvas apps**

  Clarified that behavior formulas belong on On... properties (such as OnSelect, OnVisible, OnHidden, OnStart) and that action functions like Navigate or Collect shouldn’t be used in value-expecting properties (Text, Visible, Fill). Added references to the formula reference and an in-depth guide for the full rules and list of state-changing functions.

  https://learn.microsoft.com/en-us/power-apps/maker/canvas-apps/working-with-formulas