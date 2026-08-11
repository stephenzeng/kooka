# Microsoft Viva
**Date created:** 2026-07-30 UTC  
**Tags:** Administration, Analytics, Governance  

## New Articles

- **Export data from the Agent Dashboard**

  Introduced guidance for exporting row-level Agent 365 metrics and metadata directly from the Agent Dashboard, with distinct day and week export options. Covers prerequisites (licensing, roles) and admin controls in VFAM, including switches for enabling exports and allowing identifiable data. Provides step-by-step export instructions, explains processing behavior and retrieval via Previous exports, and outlines differences in granularity and freshness between day- and week-level files. Details output formats, including ZIP packages with CSV schemas for de-identified and identifiable exports, plus when PeopleMetadata is included. Includes FAQs to help troubleshoot ID mismatches, visibility of export options, and timing differences between dashboard views and exported data.

  https://learn.microsoft.com/en-us/viva/insights/org-team-insights/export-agent-data

- **How Microsoft Organizational Data Service works**

  Explained what public organizational data is and how Microsoft Organizational Data Service distributes it across Microsoft 365 experiences such as Profile, Copilot, and Viva apps. Clarifies that data availability varies by application and documents the precedence between Microsoft Entra ID and the Organizational Data Service for profile attributes. Illustrates precedence with practical scenarios and links to related configuration resources to help admins manage source priority effectively.

  https://learn.microsoft.com/en-us/viva/how-org-data-service-works

## Major Changes

- **View and customize your general settings**

  Added a comprehensive section on admin notification emails sent when users request access to the Copilot Dashboard or Copilot Analytics. The new guidance explains who is notified, what the emails contain, and how admins can disable these notifications in the Viva Insights web app while still reviewing requests in the Request Center. This helps administrators control alert volume without disrupting approval workflows and includes an example email for clarity.

  https://learn.microsoft.com/en-us/viva/insights/advanced/admin/general-settings

## Moderate Changes

- **Import organizational data using API-based import (preview)**

  Updated terminology to use “Microsoft Organizational Data Service” across workflows and instructions, including C#, PowerShell, custom apps, and API calls. This aligns naming and reduces confusion when building or automating imports.

  https://learn.microsoft.com/en-us/viva/import-org-data-api

- **Set up connection between data source and Microsoft Organizational Data Service for API-based import**

  Renamed the service throughout the page (title, H1, descriptions, UI paths, and an option label) to “Microsoft Organizational Data Service.” No procedural steps changed, ensuring existing setup processes continue to work as documented.

  https://learn.microsoft.com/en-us/viva/import-org-data-api-set-up

- **Import organizational data with Azure Blob Storage connector**

  Replaced references to “Organizational Data in Microsoft 365” with “Microsoft Organizational Data Service” and updated related UI navigation, role assignment guidance, and connection steps. Clarified a step requiring a global admin to sign in to the service to streamline provisioning.

  https://learn.microsoft.com/en-us/viva/import-org-data-azure

- **Map attributes and set access for Microsoft 365, Copilot, and Viva apps**

  Aligned terminology and UI labels to “Microsoft Organizational Data Service” across mapping and access configuration steps. The update improves consistency in provisioning, data connections, and settings without altering procedures.

  https://learn.microsoft.com/en-us/viva/map-attributes-set-access

- **Use your organizational data in Microsoft 365 and Microsoft Viva**

  Rebranded the feature to “Microsoft Organizational Data Service” across titles, headings, and guidance, including access instructions and requirements. Updated references in related areas (Copilot Dashboard, Viva Insights, Workforce Insights, People Skills) and refreshed roles and permissions tables to reflect the new service name.

  https://learn.microsoft.com/en-us/viva/organizational-data

- **Microsoft Organizational Data Service - Attribute reference**

  Standardized terminology to the new service name across headings, descriptions, and notes. Attribute definitions and mappings remain unchanged to preserve compatibility with existing implementations.

  https://learn.microsoft.com/en-us/viva/orgdata-attributes

- **Understand how organizational data is used and retained in Microsoft 365**

  Removed the section about Microsoft User Profile precedence examples and updated the article to use “Microsoft Organizational Data Service” across content and headings. Clarified the scope of exports and audit logs under the new naming to better set expectations for data handling.

  https://learn.microsoft.com/en-us/viva/orgdata-data-usage

- **Upload and maintain data through the Microsoft 365 admin center**

  Updated terminology, headings, FAQs, and tips to reference “Microsoft Organizational Data Service,” including clarifications on upload behavior such as EffectiveDate and precedence. Adjusted a mapping table header and aligned wording without changing features or procedures.

  https://learn.microsoft.com/en-us/viva/insights/advanced/admin/upload-org-data-admin-center