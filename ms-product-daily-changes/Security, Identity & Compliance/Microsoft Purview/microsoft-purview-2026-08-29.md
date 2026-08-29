# Microsoft Purview
**Date created:** 2026-08-29 UTC  
**Tags:** Compliance, Configuration, Deprecation, Get Started, Guidance, Monitoring, Security  

## New Articles

- **Use Microsoft Purview data loss prevention policies for non-Microsoft connected apps (preview)**

  Introduced a how-to guide for applying Microsoft Purview DLP policies to non-Microsoft connected apps such as Box, Dropbox, Google Workspace, and Salesforce via Microsoft Defender for Cloud Apps connectors. The article details prerequisites, connector setup, and step-by-step policy creation using the Custom template scoped to non-Microsoft app locations. It outlines key limitations (no mixing with Microsoft 365 locations, admin units not supported, advanced rules only, no policy tips/user overrides, no simulation) and app-specific attribute availability. Monitoring guidance includes support for Activity explorer and alerts, with Content explorer not supported, and known issues such as no classification for encrypted files and PDFs.

  https://learn.microsoft.com/en-us/purview/dlp-non-microsoft-connected-applications

- **Use Microsoft Purview sensitivity label policies for non-Microsoft connected apps (preview)**

  Added guidance for using auto-labeling policies to apply sensitivity labels in non-Microsoft connected apps (initially Box and Google Workspace) through Microsoft Defender for Cloud Apps. The article covers prerequisites, connector setup, and steps to create and scope auto-labeling policies using the Custom template, along with important constraints (no mixing with Microsoft 365 locations, no admin units, and no simulation). It documents app-specific attribute availability, monitoring via Activity explorer (Content explorer not supported), and known issues including limitations with encrypted/PDF files and cross-policy label replacement behavior in Box and Google Workspace.

  https://learn.microsoft.com/en-us/purview/information-protection-non-microsoft-connected-apps

## Major Changes

- **Use data loss prevention policies for non-Microsoft cloud apps**

  Announced retirement of the Instances policy location in Microsoft Purview DLP on January 6, 2027, aligned to the retirement of Microsoft Defender for Cloud Apps file policies. Organizations should recreate policies using dedicated non-Microsoft connected app locations in Purview. Migration guidance is provided to help plan and transition policies ahead of the retirement date.

  https://learn.microsoft.com/en-us/purview/dlp-use-policies-non-microsoft-cloud-apps

- **Assign permissions in eDiscovery**

  Clarified that app-only authentication for eDiscovery cmdlets in Security & Compliance PowerShell is unsupported and recommended moving automations to Microsoft Graph APIs. The article emphasizes that any subsequent steps are best-effort guidance and do not change the unsupported status, and it removes a specific cmdlet example to generalize the guidance. This helps teams plan a supported path for automation and integration.

  https://learn.microsoft.com/en-us/purview/edisc-permissions

## Moderate Changes

- **Automatically apply a sensitivity label to Microsoft 365 data**

  Added new guidance and an example for using auto-labeling policies with advanced rules to label Exchange email by subject using regex pattern matching. The update clarifies that no mail flow rule or DLP policy is required and that evaluation occurs in transit, with steps to target Exchange, run simulation, and review results.

  https://learn.microsoft.com/en-us/purview/apply-sensitivity-label-automatically

- **Learn about data loss prevention**

  Expanded protected locations to include Non-Microsoft connected apps (preview) such as Box, Dropbox, Google Workspace, and Salesforce. This update highlights broader coverage for safeguarding sensitive data across third-party cloud services.

  https://learn.microsoft.com/en-us/purview/dlp-learn-about-dlp

- **Data loss prevention and Microsoft Teams**

  Clarified that in cross-tenant chats, DLP enforcement is based on the hosting tenant that initiated the conversation. Examples illustrate that only the hosting tenant’s policies apply to its users in that thread, guiding admins to scope and test policies accordingly.

  https://learn.microsoft.com/en-us/purview/dlp-microsoft-teams

- **Data Loss Prevention policy reference**

  Updated the locations table to “Non-Microsoft connected apps (preview)” with location type set to Cloud app instance, added data-at-rest support details, and included requirements and connector setup guidance with links. Also simplified the “Document name matches patterns” condition by removing regex references while retaining wildcard guidance.

  https://learn.microsoft.com/en-us/purview/dlp-policy-reference

- **Enable sensitivity labels for files in SharePoint and OneDrive**

  Revised Multi-Geo instructions for enabling OneNote sensitivity labels, directing admins to repeat the Set-SPOTenant step for each geo location. This reflects updated support and ensures consistent configuration across all regions.

  https://learn.microsoft.com/en-us/purview/sensitivity-labels-sharepoint-onedrive-files

- **What's new in Microsoft Purview**

  Added August 2026 updates introducing preview capabilities for non-Microsoft connected apps: DLP policies for data at rest and sensitivity label auto-labeling using Defender for Cloud Apps connectors. This expands governance and protection to popular third-party cloud services using the same classification engine as Microsoft 365.

  https://learn.microsoft.com/en-us/purview/whats-new