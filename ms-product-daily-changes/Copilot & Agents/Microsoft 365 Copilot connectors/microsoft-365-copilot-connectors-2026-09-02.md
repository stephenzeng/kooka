# Microsoft 365 Copilot connectors
**Date created:** 2026-09-02 UTC  
**Tags:** Configuration, Get Started, Guidance, Troubleshooting  

## Major Changes

- **Microsoft-built connectors gallery**

  Expanded the gallery with new categories and a broad set of Microsoft-built connectors across productivity, CRM, developer tools, and more. Listings were reorganized to place connectors in clearer categories (for example, moving Notion under Productivity) and some entries were removed from the catch-all section. This improves discoverability and helps admins and makers find relevant connectors faster for their scenarios.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/connectors-gallery-microsoft

- **Federated connectors overview**

  Reworked the catalog structure with a wider, clearer set of categories and added many new federated data sources across industries and toolsets. The admin experience and controls content remains unchanged, while the connectors list and categorization were significantly expanded. These updates make it easier to navigate options and plan deployments based on data source coverage.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/federated-connectors-overview

- **Set up the Salesforce service for Salesforce CRM connector ingestion**

  Added support details for indexing more Salesforce objects—such as Events, Tasks, and Campaigns—plus related comments and attachments, and clarified discovery across Microsoft 365 experiences. Updated OAuth setup to use the Flows Enablement section and to enable Client Credentials Flow alongside Authorization Code and Credentials Flow, removing the prior guidance to clear PKCE. Introduced guidance on Salesforce Refresh Token Rotation, recommending separate authorizations per connector connection to avoid token invalidation and sign-in failures. These changes streamline secure configuration and broaden the data available to Copilot.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/salesforce-crm-admin-setup

- **Salesforce CRM connector overview**

  Expanded the documented scope of indexed Salesforce data to include Account, Contact, Opportunity, Lead, Case, Event, Task, and Campaign objects. Updated limitations and the data types table to add Event, Task, Campaign, Comment, and Attachment with details on captured fields. This clarifies exactly which Salesforce content is searchable and usable across Microsoft 365 experiences.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/salesforce-crm-overview

## Moderate Changes

- **Deploy the Salesforce CRM connector**

  Updated deployment guidance to reflect a broader set of indexed Salesforce objects, including Events, Tasks, Campaigns, Comments, and Attachments. Clarified how content becomes discoverable in Microsoft 365 Copilot and Microsoft Search to set accurate expectations for end users.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/salesforce-crm-deployment

- **Troubleshoot issues with the Salesforce CRM connector**

  Removed an outdated sign-in issue related to PKCE and added new guidance on how attachments are handled. Clarified that Copilot uses text extracted from attachments (not the original files), and that up to 20 MB of attachment content per record is processed in ascending file size, with only file names indexed after the limit is reached.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/salesforce-crm-troubleshooting