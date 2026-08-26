# Power Platform
**Date created:** 2026-08-26 UTC  
**Tags:** Best Practices, Compliance, Configuration, Governance, Guidance, Security  

## New Articles

- **Manage SharePoint document visibility in Dataverse solutions**

  Introduced architecture guidance to align SharePoint document access with Dataverse record-level security by limiting discoverability and navigation. Provides end-to-end setup steps, including Entra ID group preparation, environment and site configuration, custom SharePoint permission level (disabling directory browsing), site group assignment, disabling site search, and optional Copilot discovery restrictions. Details enabling native SharePoint integration in Dataverse, required permissions for Document and Document Location records, and optional controls via Conditional Access with auditing and monitoring using Microsoft Purview. Covers business scenarios for when to use or avoid the pattern, and considerations across reliability, security, operational excellence, performance, and user experience.  
  https://learn.microsoft.com/en-us/power-platform/architecture/reference-architectures/sharepoint-dataverse-security

## Major Changes

- **Power Platform inventory**

  Added a Sovereign clouds section explaining availability in US Government clouds (GCC, GCC High, DoD) and introduced a matrix showing which resources (apps, flows, environments, agents, and more) are inventoried per cloud. Clarified that connector inventory isn’t available in these government clouds and noted the feature isn’t available in 21Vianet (China) or air-gapped environments. Updated Known limitations to reflect these constraints, helping regulated organizations plan inventory, governance, and compliance strategies with accurate coverage expectations.  
  https://learn.microsoft.com/en-us/power-platform/admin/power-platform-inventory

## Moderate Changes

- **Overview of Power Platform and Copilot Studio reference architectures**

  Updated the reference architectures index by removing the “Streamline document processing with AI Builder” entry and adding “Manage SharePoint document visibility in Dataverse solutions.” This keeps the catalog current and highlights a new security and governance-focused pattern for controlling SharePoint document exposure.  
  https://learn.microsoft.com/en-us/power-platform/architecture/reference-architectures/

- **Microsoft Dataverse reference architectures and solution ideas**

  Added a new solution entry linking to guidance on managing SharePoint document visibility for records stored in Dataverse. This helps teams reduce oversharing while retaining native SharePoint document management in model-driven apps.  
  https://learn.microsoft.com/en-us/power-platform/architecture/products/microsoft-dataverse