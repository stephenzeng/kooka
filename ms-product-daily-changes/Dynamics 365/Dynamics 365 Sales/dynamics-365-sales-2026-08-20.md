# Dynamics 365 Sales
**Date created:** 2026-08-20 UTC  
**Tags:** Analytics, Automation, Best Practices, Compliance, Configuration, Deprecation, Get Started, Governance, Guidance, Identity, Licensing, Security, Troubleshooting  

## New Articles

- **Activate Sales Development agent**
  
  Added a step-by-step guide to activate the Sales Development agent in Microsoft Teams. Clarifies required licenses, admin roles, and enabling Copilot Frontier and Agent 365 public preview. Details how to select users or groups, apply policy templates, and provision resources like Teams, Exchange, OneDrive, and SharePoint. Explains identity choices, domain selection, and where to manage updates post-creation.

  https://learn.microsoft.com/en-us/dynamics365/sales/sales-dev-agent/activate-agent

- **Sales Development agent architecture**
  
  Introduced an architecture overview for the Sales Development agent. Summarizes key components and data flows with centrally maintained details via shared content. Helps architects and admins understand how the agent operates and integrates.

  https://learn.microsoft.com/en-us/dynamics365/sales/sales-dev-agent/architecture

- **Outreach email architecture**
  
  Added a focused overview of the outreach email architecture used by the Sales Development agent. Highlights how email generation and delivery are structured, with deeper details sourced from shared content. Equips teams to design and troubleshoot outreach scenarios.

  https://learn.microsoft.com/en-us/dynamics365/sales/sales-dev-agent/architecture-outreach-email

- **Configure send time for the Sales Development agent**
  
  Published guidance to configure send time for outreach in Microsoft Teams. Explains how send-time logic works, and provides recommendations for follow-up cadence and campaign expiry. Consolidates steps and best practices into an easy-to-follow setup.

  https://learn.microsoft.com/en-us/dynamics365/sales/sales-dev-agent/configure-send-time

- **Copy configuration from one Sales Development agent to another**
  
  Added procedures to export a source agent’s configuration and import it to a target agent. Provides prerequisites, validation steps, and common mistakes to avoid. Includes troubleshooting tips and security recommendations for handling configuration files. Streamlines replication of proven settings across agents.

  https://learn.microsoft.com/en-us/dynamics365/sales/sales-dev-agent/copy-configuration

- **Create a Sales Development agent instance**
  
  Introduced steps to create an agent instance from Microsoft Teams Store or the Microsoft 365 Copilot Agent Store. Covers prerequisites, identity settings (name and email alias), and domain choices. Describes provisioning outcomes and expected timelines. Notes how admins can later change username, alias, and domain in Microsoft Entra or the Microsoft 365 admin center.

  https://learn.microsoft.com/en-us/dynamics365/sales/sales-dev-agent/create-instance

- **Sales Development agent email conversation patterns**
  
  Published best practices for handling common email conversation flows. Explains continuity, personalization, and scenarios such as colleague handoffs and CC replies, including current limitations. Helps ensure smoother prospect engagement and consistent follow-ups.

  https://learn.microsoft.com/en-us/dynamics365/sales/sales-dev-agent/email-conversation-patterns

- **Get reports from the Sales Development agent**
  
  Added guidance to obtain and interpret agent reports. Details when to use Campaign summary, Individual prospect, and Stage export reports, and how to read key metrics. Explains exporting prospect status data to CSV for deeper analysis.

  https://learn.microsoft.com/en-us/dynamics365/sales/sales-dev-agent/get-reports

- **Integrate the Sales Development agent with Dynamics 365**
  
  Introduced an end-to-end setup for connecting the agent to Dynamics 365 Sales. Covers granting access, enabling and publishing the Dataverse MCP server, and approving it via recommended tools. Provides next steps to complete CRM integration and operationalize the agent.

  https://learn.microsoft.com/en-us/dynamics365/sales/sales-dev-agent/integrate-with-dynamics

- **Launch live outreach with the Sales Development agent**
  
  Added instructions to initiate live outreach from Microsoft Teams. Walks through the launch flow and clarifies which CRM actions the agent performs during execution. Helps teams move from testing to production outreach with confidence.

  https://learn.microsoft.com/en-us/dynamics365/sales/sales-dev-agent/launch-live

- **Multilingual capabilities of the Sales Development agent**
  
  Introduced an overview of multilingual support for outreach. Provides guidance on configuring language targeting and explains search and testing behaviors. Helps teams tailor campaigns to regional audiences effectively.

  https://learn.microsoft.com/en-us/dynamics365/sales/sales-dev-agent/multilingual

- **Onboard the Sales Development agent**
  
  Published an onboarding guide that frames the configuration approach for the agent. Covers defining playbooks, setting guidelines, providing product knowledge, and configuring email and outreach. Accelerates initial setup with structured, reusable guidance.

  https://learn.microsoft.com/en-us/dynamics365/sales/sales-dev-agent/onboard-agent

- **Sales Development agent overview (preview)**
  
  Added an overview covering AI processing, cross-geo data flows, and EU compliance considerations. Explains installation transparency, supported content, required permissions, and current limitations. Provides a clear entry point for evaluating readiness and governance requirements, plus how to submit feedback.

  https://learn.microsoft.com/en-us/dynamics365/sales/sales-dev-agent/sales-development-agent-overview

- **Scale the Sales Development agent across teams**
  
  Introduced guidance for scaling agent adoption across multiple teams. Centralizes best practices for repeatable rollout and governance. Helps organizations standardize usage while maintaining control.

  https://learn.microsoft.com/en-us/dynamics365/sales/sales-dev-agent/scale-agent

- **Test the Sales Development agent in chat**
  
  Added instructions for testing the agent by uploading prospect lists and running realistic scenarios in chat. Provides steps to validate behaviors and outcomes before going live. Enables safer, evidence-based rollout.

  https://learn.microsoft.com/en-us/dynamics365/sales/sales-dev-agent/test-agent

## Moderate Changes

- **MCP tools for Copilot in Dynamics 365 Sales**
  
  Removed two SharePoint MCP tools from the documented list: msdyn_GetDocumentSearchResults and msdyn_SalesAnswerFromDocuments, including their parameters and outputs. This clarifies current tool availability and prevents reliance on removed capabilities.

  https://learn.microsoft.com/en-us/dynamics365/sales/copilot-in-sales-tools

- **Removed or deprecated features in Dynamics 365 Sales**
  
  Added a deprecation notice for SharePoint MCP tools msdyn_GetDocumentSearchResults and msdyn_SalesAnswerFromDocuments, effective August 2026. Advises customers to update any customizations that depend on these tools and references the MCP server overview for alternatives and next steps.

  https://learn.microsoft.com/en-us/dynamics365/sales/deprecations-sales