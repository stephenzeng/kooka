# Microsoft 365 Copilot connectors
**Date created:** 2026-08-19 UTC  
**Tags:** Configuration, Get Started, Guidance, Identity, Security, Troubleshooting  

## New Articles

- **Set up the BambooHR service for BambooHR connector ingestion**
  Added an administrator setup guide to prepare BambooHR for Copilot connector ingestion. It walks through creating a BambooHR developer account, registering an app, configuring the Microsoft OAuth redirect URL, and selecting required read-only scopes. The article explains how to obtain client credentials and provides a checklist to streamline setup with screenshots for clarity. It also points to deployment guidance so admins can proceed from setup to rollout.
  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/bamboohr-admin-setup

- **Deploy the BambooHR connector**
  Introduced step-by-step deployment instructions for the BambooHR Copilot connector in the Microsoft 365 admin center. The guide covers prerequisites, configuring the instance URL, OAuth 2.0 consent, and staged rollout options. It details default access behavior, identity mapping using email in Microsoft Entra, and sync cadence (15-minute incremental, daily full), plus customization for user and content settings. The article clarifies which properties are indexed and which customizations are unsupported, and links to setup, overview, and troubleshooting resources.
  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/bamboohr-deployment

- **BambooHR connector overview**
  Published an overview of the BambooHR connector, describing scenarios, capabilities, and constraints. It explains people data indexing, natural language queries in Copilot, and near-real-time sync, along with identity mapping via email. The doc outlines limitations like predefined schema and tenant-wide visibility, and lists the indexed profile properties. It also includes example prompts, guidance for using the connector with Copilot agents, and notes on permissions and citation behavior.
  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/bamboohr-overview

- **Troubleshoot issues with the BambooHR connector**
  Added troubleshooting guidance for common BambooHR connector issues with actionable fixes. It addresses authentication failures by verifying credentials, required scopes, and redirect URLs before reauthorizing. The article clarifies user mapping requirements, emphasizing exact email matches between BambooHR and Microsoft Entra, and provides support contact details. Related setup, deployment, and overview links help admins quickly move from diagnosis to resolution.
  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/bamboohr-troubleshooting

- **Set up the Azure SQL and Microsoft SQL Server services**
  Released an admin setup guide for Azure SQL and SQL Server connectors, focusing on secure and reliable data access. It covers installing the Microsoft Graph connector agent for SQL Server, creating a read-access service account, and configuring Microsoft Entra app registration for Azure SQL. The article includes assigning database roles and configuring firewall rules with Microsoft 365 client IP ranges by region. A checklist and next steps help admins transition directly to deployment.
  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/mssql-admin-setup

- **Deploy the Azure SQL and Microsoft SQL Server connectors**
  Introduced comprehensive deployment instructions for Azure SQL and SQL Server connectors in the Microsoft 365 admin center. The guide explains prerequisites, choosing the right authentication method (Entra ID OIDC for Azure SQL, Windows auth via connector agent for SQL Server), and rollout patterns. It details access control and identity mapping with supported ACL formats, plus content settings such as required full crawl SQL, watermarking, optional incremental crawl, and soft delete. Admins also get guidance on property management, semantic labels, and scheduling syncs, with links to related articles.
  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/mssql-deployment

- **Azure SQL and Microsoft SQL Server connectors overview**
  Published an overview describing how the connectors index relational data for Copilot and Microsoft Search. It summarizes key capabilities like SQL query-based indexing, ACL enforcement, scheduled crawls, semantic search, and Copilot Q&A, while calling out supported versions and data type mappings. The document clarifies limitations (same-tenant requirement for Azure SQL, OLTP constraints, and no rich content indexing) and explains record-level permissions using Allowed/Deny lists with supported ID formats. Example prompts and a link to deployment help teams get started quickly.
  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/mssql-overview

- **Troubleshoot issues with the Azure SQL and Microsoft SQL Server connectors**
  Added a troubleshooting guide focused on common crawl failures and how to resolve them. It identifies transport-level errors as likely network issues and advises reviewing network logs and contacting support as needed. The article also flags nonalphanumeric column names in SELECT statements and recommends using aliases to ensure successful indexing. Links to setup, deployment, and overview content provide a clear path for remediation.
  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/mssql-troubleshooting