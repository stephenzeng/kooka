# Dev and Admin for Dynamics 365 Business Central
**Change date:** 2026-08-07 UTC  
**Tags:** Administration, Agent, AI, Monitoring  

## New Articles

- **Update 28.4 for Microsoft Dynamics 365 Business Central 2026 Release Wave 1**

  Introduced the 28.4 “What’s new” article with feature highlights, including GA for Payables Agent Known Senders, GA for E-Document payments, and a public preview to validate Peppol invoices from purchase drafts. Provided upgrade guidance for online and on-premises customers, with paths for version 28 and earlier. Improved Field Service integration now honors the Dataverse “Convert to Customer Asset” setting for new synchronizations while preserving existing couplings. Noted that Copilot and agent data may move across geographies and can be managed via the Copilot & agent capabilities page, and confirmed no localization updates in this release. Included links to Microsoft Support hotfixes and curated partner/user resources.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/whatsnew/whatsnew-update-28-4

## Moderate Changes

- **Compilation scope overview**

  Clarified server configuration by renaming the setting to ExtensionAllowedTargetLevel, which governs whether extensions target Cloud or OnPrem. This helps administrators use the correct parameter and avoid misconfiguration during publishing.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/devenv-compilation-scope-overview

- **Turn off or limit telemetry trace Events**

  Updated configuration guidance to use the Set-NAVServerConfiguration PowerShell cmdlet for Diagnostic Trace Level, removing references to the Administration tool and direct CustomSettings.config edits. Added a pointer to the “Configuring Business Central Server” article for deeper setup details.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/administration/disable-limit-telemetry-events

- **What's new and planned in Business Central**

  Refreshed the version table by adding 28.4 (August 2026) with a link to its update article and pruning older 28.1 entries. This keeps the page focused on the most current releases for easier discovery.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/whatsnew/overview

- **Resources for partners**

  Expanded the Agents section with a new Expense Agent walkthrough and noted preview availability in AU, AT, CA, DK, FR, DE, NZ, ES, UK, and US. Introduced a “Get started building agents” subsection covering design/coding, evaluations, MCP server, and Copilot Studio, and reorganized agent resources for clearer navigation.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/readiness/readiness-ready-to-go

- **Analyzing Report Telemetry**

  Renamed on-prem parameters to align with behavior: ReportTimeout for execution timeouts and ReportMaxRows for row limits. The guidance clarifies how these settings cancel long-running or large reports to control resource usage.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/administration/telemetry-reports-trace

- **Dynamics 365 Business Central on-premises 2025 release wave 2 updates**

  Added Update 27.10 with KB 5123579 and August 2026 release/build details. This helps admins track the latest cumulative update and plan deployments.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/deployment/update-versions-27

- **Dynamics 365 Business Central on-premises 2026 release wave 1 updates**

  Added Update 28.4 with KB 5123580 and associated August 2026 build numbers. The versions table now reflects the latest CU for streamlined maintenance planning.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/deployment/update-versions-28

- **Business Central upgrade compatibility matrix**

  Extended the compatibility matrix with new rows, including 27.10 (minimum compatible 28.5) and 26.16 mappings, and adjusted prior 27.9/28.4 and 26.15/27.10/28.4 entries. This provides clearer upgrade paths for recent cumulative updates and notes that the prior release wave include is no longer updated.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/upgrade/upgrade-v14-v15-compatibility