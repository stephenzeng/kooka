# Power Apps
**Date created:** 2026-08-07 UTC  
**Tags:** Automation, Programming  

## New Articles

- **Publish Power Apps Code Apps with a Service Principal**

  Introduced guidance for publishing Power Apps code apps non-interactively using a Microsoft Entra service principal to enable CI/CD scenarios. Explains required identifiers, the difference between app registrations and enterprise applications, and the one-time prerequisite to share the app with the service principal. Provides environment variable configuration for service principal authentication in PowerShell and Bash, and details build and publish steps using npm build and pa app push --non-interactive. Notes non-interactive authentication behavior and exit code handling, with links to related CLI and ALM references.

  https://learn.microsoft.com/en-us/power-apps/developer/code-apps/how-to/use-service-principal

## Major Changes

- **Quickstart: Web API with client-side JavaScript and Visual Studio Code**

  Updated the JavaScript SPA quickstart to require a redirect bridge page for MSAL Browser v5, adding src/redirect.html and switching the redirect URI to http://localhost:1234/redirect.html. Refreshed tooling and scripts, including updated package dependencies, a start script that serves both index and redirect pages, and a resolver configuration for package exports. Expanded prerequisites and refined authentication and API call steps, with clearer Entra app registration guidance, Workspace Trust notes, and updated troubleshooting references.

  https://learn.microsoft.com/en-us/power-apps/developer/data-platform/webapi/quick-start-js-spa

## Moderate Changes

- **Power Apps CLI command reference**

  Added a --non-interactive parameter to pa app push to support unattended app publishing. Updated guidance to reference service principal–based authentication for CI/CD pipelines.

  https://learn.microsoft.com/en-us/power-apps/developer/code-apps/reference/cli

- **Quickstart: Execute a Dataverse SDK for .NET Request in C#**

  Modernized the quickstart for Visual Studio 2026 and .NET 10 LTS, with clearer project setup, NuGet installation, and step-by-step execution. Replaced inline code with a GitHub code-include and improved explanations for using ServiceClient and IOrganizationService, including follow-on exercises.

  https://learn.microsoft.com/en-us/power-apps/developer/data-platform/org-service/quick-start-org-service-console-app