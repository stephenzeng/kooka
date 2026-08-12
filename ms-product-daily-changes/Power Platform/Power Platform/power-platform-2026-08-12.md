# Power Platform
**Date created:** 2026-08-12 UTC  
**Tags:** Analytics, Automation, Best Practices, Configuration, Governance, Guidance, Licensing, Monitoring, Performance, Security  

## New Articles

- **Integrate Dynamics 365 finance and operations apps with Power Platform**

  Introduced a reference architecture for integrating Dynamics 365 finance and operations apps with Power Platform and Azure to support engineer-to-order scenarios. Details Dataverse roles for data, plugins, and orchestration alongside Azure components such as Service Bus, Functions, Key Vault, and a dedicated integration identity. Defines integration patterns: virtual entities for read, dual-write for finalized quote lines (excluding financial posting entities), and OData for operational data. Covers pricing composition, recap finalization/locking, user roles, licensing notes, requirements, and operational considerations across reliability, security, performance, and experience.

  https://learn.microsoft.com/en-us/power-platform/architecture/reference-architectures/finance-and-operations-dataverse

- **Manage Copilot credit allocations programmatically**

  Introduced a tutorial for managing Copilot credit allocations via the Power Platform API and Admin SDKs for PowerShell, C#, and Python. Explains how to view available credits (entitlement ID MCSMessages), allocate credits using allocationsV2, and control overage with the TenantPool enforcement rule. Includes prerequisites, admin center steps, API version 2024-10-01 guidance, and complete code samples to accelerate automation.

  https://learn.microsoft.com/en-us/power-platform/admin/programmability-tutorial-manage-copilot-credit-allocations

## Major Changes

- **Create cross-tenant isolation reports**

  Added a step to locate the environment for a reported connection and a new section that explains report contents, including the connections array fields and that reports include blocked attempts. Provided a comprehensive PowerShell script and instructions to enumerate environments, list their connections, and match by connectionId to identify the environment. Included a related API reference for listing connections in an environment and refined wording in automation tabs to improve clarity.

  https://learn.microsoft.com/en-us/power-platform/admin/programmability-tutorial-cross-tenant-reporting

## Moderate Changes

- **Overview of Power Platform and Copilot Studio reference architectures**

  Added a new entry under “Integrate with external systems” for integrating finance and operations data with Dataverse. Highlights scenarios such as estimation, pricing, quoting, and production planning to guide solution design.

  https://learn.microsoft.com/en-us/power-platform/architecture/reference-architectures/

- **Power Platform inventory sample queries**

  Added a query to identify GitHub Copilot harness–created Copilot Studio agents using isCLIAgent in PowerPlatformResources. Helps admins quickly audit and report on these agents with projected key metadata and ordered results.

  https://learn.microsoft.com/en-us/power-platform/admin/inventory-sample-queries

- **Microsoft Dataverse reference architectures and solution ideas**

  Added a reference architecture entry on integrating finance and operations data with Dataverse, leveraging Power Platform and Azure. Provides patterns and scenarios to guide end-to-end solution planning.

  https://learn.microsoft.com/en-us/power-platform/architecture/products/microsoft-dataverse

- **View license consumption for Dynamics 365 finance and operations apps**

  Clarified that User License Consumption applies only to cloud-hosted environments connected to Microsoft Entra ID and the Power Platform admin center. Noted that on-premises deployments aren’t supported and provided a link to the on-premises license usage summary.

  https://learn.microsoft.com/en-us/power-platform/admin/view-license-consumption-finops-apps