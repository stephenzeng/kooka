# Microsoft Viva
**Date created:** 2026-07-16 UTC  
**Tags:** Administration, Analytics, Automation, Governance, Monitoring, Programming  

## New Articles

- **Consuming data from Organizational data in Microsoft 365 into Viva Glint**

  Introduced end-to-end guidance for bringing employee data from Organizational data in Microsoft 365 into Viva Glint. The article explains reserved versus custom attributes, how automatic and manual mappings work, and which reserved attributes are excluded. It outlines a one-time onboarding flow for existing customers, options to enable or disable imports, and how to adjust mappings later. Auditing notes help administrators monitor imports and troubleshoot issues.

  https://learn.microsoft.com/en-us/viva/glint/setup/modis-data-consumption

- **Importing people data via Organization data in M365 to Viva Glint**

  Added a comprehensive import guide covering prerequisites and permissions, creating the data connection, enabling Viva Glint, preparing data, and mapping both reserved and custom attributes. The steps include configuring attribute access, validating the dataset, and monitoring ingestion. The guidance clarifies required schema fields, data-sharing requirements, error handling for invalid records, supported import types and connectors (CSV, Workday, SuccessFactors, ADLS, API), and file size limits.

  https://learn.microsoft.com/en-us/viva/glint/setup/modis-data-import

- **Viva Glint Raw Data Export APIs**

  Introduced a how-to for exporting Viva Glint raw data via Microsoft Graph, including app registration, authentication, and permission setup (SentimentSurvey.Export.All). The guide details three core API operations—Export, Status, and Download—with required headers, parameters, and sample cURL/PowerShell calls. It also lists supported job statuses and common errors to streamline automation and troubleshooting.

  https://learn.microsoft.com/en-us/viva/glint/setup/viva-glint-raw-data-export-apis

## Major Changes

- **Key roles for Viva Glint**

  Added the Organizational Data Source Administrator role with responsibilities spanning data schema management, HRIS integrations, data quality monitoring, and collaboration with IT/HRIS teams. The guidance recommends assigning this role to Viva Glint Administrators for effective data management and ingestion. A comparison clarifies how this role differs from the Viva Glint Tenant Administrator and Service Administrator, helping organizations align access with duties.

  https://learn.microsoft.com/en-us/viva/glint/start/role-definitions

- **Set up attributes in Viva Glint**

  Introduced end-to-end steps to configure Viva Glint attributes for Organizational data in Microsoft 365, including dataset upload, pre-ingestion validation, and date format selection. The update explains how to map Glint custom attributes to Organizational data reserved or custom attributes, with recommendations for automatic and manual mappings and an option to maintain a separate manager hierarchy. Final review and completion steps cover both immediate and deferred data import scenarios.

  https://learn.microsoft.com/en-us/viva/glint/setup/send-employee-attributes

- **Export Copilot metrics from the Microsoft Copilot Dashboard**

  Added day-level exports (last 28 days) alongside week-level exports (last six months) and summarized key differences in duration, refresh, data freshness, use cases, and metric availability. Clarified that VFAM now governs both export types and updated steps to choose between “Export by week” or “Export by day,” including data freshness windows. Metrics availability was overhauled to flag which metrics are week-only versus available in both, and FAQs were updated with distinct refresh cadences and examples.

  https://learn.microsoft.com/en-us/viva/insights/org-team-insights/export-copilot-metrics

## Moderate Changes

- **Viva Glint Activity Audit Log**

  Added six new audit events covering enable/disable actions for Organizational data and SFTP imports, plus attribute setup and migration. These entries improve traceability for data ingestion changes and onboarding activities.

  https://learn.microsoft.com/en-us/viva/glint/setup/activity-audit-log

- **Viva Glint employee attribute fundamentals**

  Introduced the concept of reserved attributes and how they link to Organizational data, along with date attribute requirements for connectors. Increased the custom attribute limit to 123 when using Organizational data imports and added clear naming rules. Updated compliance language to reflect Microsoft’s approach to data protection and responsible data handling.

  https://learn.microsoft.com/en-us/viva/glint/setup/attribute-fundamentals

- **Choose a Viva Glint data upload method**

  Added Organizational data in Microsoft 365 as a third upload option, supporting automated connectors and manual CSV uploads for centralized data management. Clarified that the “Learn more” guidance applies to SFTP and web app uploads.

  https://learn.microsoft.com/en-us/viva/glint/setup/choose-upload-method

- **Connect to the Microsoft Copilot Dashboard for Microsoft 365 customers**

  Clarified day-level export behavior regarding license assignment and removal: exports within two days may not reflect changes, while later exports will. Noted that previously exported files are not retroactively updated.

  https://learn.microsoft.com/en-us/viva/insights/org-team-insights/copilot-dashboard

- **Use the Viva Glint Employee attribute template**

  Clarified supported file formats and encodings: CSV must be comma-delimited with UTF-8 (with or without BOM); XLSX must have a single worksheet; People Import and SFTP support both formats. Noted that Organizational data imports support UTF-8 encodings and introduced “Reserved attribute mapping” terminology for updating Glint attributes via Organizational data.

  https://learn.microsoft.com/en-us/viva/glint/setup/create-employee-attribute-template

- **Set up Secure File Transfer Protocol (SFTP) in Viva Glint**

  Added a “Use SFTP” toggle to control ingestion without removing existing connection details. Split the configuration into enabling the toggle and reviewing or entering field information to reduce setup errors.

  https://learn.microsoft.com/en-us/viva/glint/setup/set-up-sftp

- **Update attributes in Viva Glint**

  Expanded steps for scenarios using Organizational data, including a pre-ingestion validation to surface file, ingestion, and schema issues earlier. Added guidance to review and update reserved attribute mappings and clarified hierarchy group level behavior and mapping immutability, with refreshed UI steps and screenshots.

  https://learn.microsoft.com/en-us/viva/glint/setup/update-attributes

- **Meet and plan with Viva Glint data stakeholders**

  Added guidance to leverage Organizational data for Viva Glint imports, including a tip to coordinate with the Organizational Data Administrator and existing HRIS connectors. Updated planning tasks to include configuring connectors in Week 1 and mapping reserved attributes in Week 2, with links to supporting documentation.

  https://learn.microsoft.com/en-us/viva/glint/setup/upload-employee-data