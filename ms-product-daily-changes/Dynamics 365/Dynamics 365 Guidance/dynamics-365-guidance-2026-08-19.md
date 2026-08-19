# Dynamics 365 Guidance
**Date created:** 2026-08-19 UTC  
**Tags:** Automation, Best Practices, Compliance, Configuration, Governance, Guidance, Licensing, Monitoring, Performance, Security  

## New Articles

- **Hybrid Integration with Dynamics 365 Finance and Operations Apps**

  Introduced a reference architecture for hybrid integrations between Dynamics 365 finance and operations apps and on-premises systems using BizTalk Server and Azure services. Covers real-time APIs, asynchronous messaging, event-driven, and batch patterns with detailed inbound/outbound dataflows. Outlines components such as Azure Service Bus, Azure Key Vault, and Microsoft Entra ID (OAuth 2.0) and explains where each pattern fits. Provides guidance on security, scalability, resilience, reuse vs. rebuild decisions, and cost optimization with links to related resources.

  https://learn.microsoft.com/en-us/dynamics365/guidance/reference-architectures/finance-operations-hybrid-integration

- **Automate Purchase Requisition and Supplier Invoice Approvals**

  Added a reference architecture that automates purchase requisition and supplier invoice approvals across Dynamics 365 Finance and Supply Chain Management using Power Automate and standard approvals. Describes sourcing dynamic approvers from an external project management app via SQL through the on-premises data gateway, sending approval notifications in Teams and Outlook, and feeding decisions back into Dynamics 365 workflows. Includes an architecture diagram, dataflows, component list, implementation steps for workflows, business events, and cloud flows, plus cost and licensing considerations and related training.

  https://learn.microsoft.com/en-us/dynamics365/guidance/reference-architectures/finance-operations-purchase-requisition-external-project-management

- **Resilient Inbound Integration for Supply Chain Management**

  Published a resilient, decoupled inbound integration pattern connecting external LOB systems to Dynamics 365 Supply Chain Management via Azure Application Gateway (WAF), API Management, Service Bus, Logic Apps, Key Vault, Managed Identities, and Application Insights. Details an end-to-end dataflow with correlation, durable queueing, custom service endpoints, integration tables, batch jobs, business events, and webhook callbacks. Provides scenarios and examples with deep guidance on security, reliability, performance, and operational best practices. Includes step-by-step implementation procedures across Azure networking, APIM policies, Service Bus and Logic Apps orchestration, and Dynamics 365 components.

  https://learn.microsoft.com/en-us/dynamics365/guidance/reference-architectures/finance-operations-resilient-inbound-integration-external-system

- **Dynamics 365 Finance Architecture for Utility Companies**

  Introduced a contract-to-collection reference architecture integrating Dynamics 365 Finance with MECOMS 365 and MEEP. Explains the end-to-end flow from contracting through billing, payments, and financial posting with a component breakdown and architecture diagram. Highlights design considerations for scalability, maintainability, compliance, and operational efficiency through automation and manage-by-exception. Offers guidance to optimize cost for cloud-scale operation.

  https://learn.microsoft.com/en-us/dynamics365/guidance/reference-architectures/finance-utilities-contract-collection

## Moderate Changes

- **Add a mobile lookup control to the Field Service mobile app**

  Updated the article to reflect general availability by removing preview labels and prerelease disclaimers. Guidance remains unchanged, improving clarity and signaling production readiness for deployment.

  https://learn.microsoft.com/en-us/dynamics365/guidance/resources/field-service-mobile-add-lookup