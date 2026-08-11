# Microsoft 365 Copilot connectors
**Date created:** 2026-07-25 UTC  
**Tags:** Administration, AI, Security  

## Major Changes

- **Submit a federated connector**

  Removed legacy prerequisites for submission, including the need for a business development engagement and a signed legal agreement for use of MCP tools. This streamlines the path for partners to submit federated connectors and reduces onboarding friction. Core gallery requirements are unchanged, helping publishers focus on current validation criteria without extra administrative steps.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/submit-federated-connector

## Moderate Changes

- **Deploy the ServiceNow Catalog connector**

  Clarified OIDC setup by directing admins to explicitly select the User Claim (sub or oid) and to switch if user resolution fails, and set Scope Restriction/Auth Scope to Useraccount scoped (useraccount). Updated the OIDC metadata URL to the v2.0 endpoint to prevent configuration errors and improve sign-in reliability.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/servicenow-catalog-deployment

- **Deploy the ServiceNow Knowledge Copilot connector**

  Updated OIDC guidance to require an explicit User Claim selection (sub or oid) and to use Useraccount scoped (useraccount) for Scope Restriction/Auth Scope. Switched the Microsoft Entra ID metadata URL to the v2.0 endpoint, improving configuration accuracy and troubleshooting outcomes.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/servicenow-knowledge-deployment

- **ServiceNow Knowledge Copilot connector overview**

  Expanded indexing details to include comments and attachments within knowledge articles, with supported formats such as Office, OpenDocument, PDF, text/markup, web archives, email, and ZIP. Documented limits and exclusions: image files aren’t indexed, and each article indexes up to 100 attachments with a combined 20 MB cap—helping plan content for optimal retrieval.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/servicenow-knowledge-overview

- **Deploy the ServiceNow Tickets Copilot connector**

  Clarified OIDC configuration by requiring an explicit User Claim choice (sub or oid) and setting Scope Restriction/Auth Scope to Useraccount scoped (useraccount). These updates reduce identity-mapping issues and improve deployment reliability.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/servicenow-tickets-deployment