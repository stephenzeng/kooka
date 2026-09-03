# Dynamics 365 Business Central
**Date created:** 2026-09-03 UTC  
**Tags:** Best Practices, Configuration, Guidance, Security, Troubleshooting  

## Major Changes

- **Set up Sales Order Agent**

  Overhauled setup guidance with a clearer permissions and access model, including required system permissions (Configure All Agents, Manage Agent Tasks), key permission sets (AGENT - ADMIN, D365 Agent, SOA - EDIT), and license entitlements. Streamlined user access management with step-by-step instructions for adding users from both the configuration page and the agent card, and clarified the Can Configure behavior. Introduced guidance for changing agent language/region, managing permission sets for the agent account, and a troubleshooting workflow to resolve permission errors. Added diagnostics instructions to review agent tasks, steps, and logs via the Agents page, including when to use the Agent - Diagnostics permission set, and refined prerequisites, configuration steps, and mailbox/email handling details.

  https://learn.microsoft.com/en-us/dynamics365/business-central/sales-order-agent-setup

## Moderate Changes

- **FAQ for Sales Order Agent**

  Increased the PDF attachment processing limit from 10 to 50 pages and clarified how permission sets govern data/object access while UI roles control visible elements. Added guidance to assign required extension permission sets when customizations or ISV solutions affect pages or business logic used by the agent, reducing permission-related errors.

  https://learn.microsoft.com/en-us/dynamics365/business-central/faqs-sales-order-taker-agent

- **Connect e-documents to Microsoft 365 applications**

  Expanded Service Integration V2 to support SharePoint and OneDrive in addition to Outlook. Added setup steps for creating document/archive folders, applying shared links, enabling the connector, and using Receive to import PDFs, along with requirements for read/write access, a 20 MB PDF size limit, and using the same Microsoft Entra tenant.

  https://learn.microsoft.com/en-us/dynamics365/business-central/finance-connect-edocuments-microsoft365

- **Italian subcontracting**

  Added guidance explaining that the Subcontracting app does not support subcontractor locations when bins or warehouse handling settings (Bin Mandatory, Require Pick/Put-away/Receive/Shipment) are enabled. Instructed users to replace subcontracting locations on vendor cards with locations that don’t use bins or warehouse handling before migration to prevent issues.

  https://learn.microsoft.com/en-us/dynamics365/business-central/LocalFunctionality/Italy/italian-subcontracting