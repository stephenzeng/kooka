# Dynamics 365 Sales
**Date created:** 2026-07-21 UTC  
**Tags:** Administration, Agent, AI, Analytics, Automation, Governance, Security  

## Moderate Changes

- **Set up product families | MicrosoftDocs**

  Added a new section with clear steps to add products or bundles to a product family, including using Revise for published items and publishing changes. Clarified reparenting considerations with a link to detailed guidance, helping admins manage product hierarchies safely.

  https://learn.microsoft.com/en-us/dynamics365/sales/create-product-family

- **Set up and configure AI-powered Data Enrichment**

  Updated prerequisites and configuration to include Teams meeting data (transcripts or AI summaries) alongside email. Clarified that seller consent is required before any analysis and that data is read in place without being stored in CRM; sources are now explicitly listed as Outlook and Teams.

  https://learn.microsoft.com/en-us/dynamics365/sales/data-enrichment-agent-configure

- **Edit AI-powered Data Enrichment settings**

  Expanded data source coverage to include Outlook interactions and Teams meetings using transcripts or Microsoft 365 Copilot summaries. Updated consent requirements to encompass Teams meeting data in addition to email.

  https://learn.microsoft.com/en-us/dynamics365/sales/data-enrichment-agent-edit-settings

- **FAQs about AI-powered Data Enrichment for opportunities**

  Expanded data sources to include Teams meeting content and clarified consent for both emails and meetings. Added guidance on which meetings are analyzed (matching attendees by the opportunity’s primary contact and license-based use of summaries vs. transcripts) and noted that calendar citations are visible only to attendees.

  https://learn.microsoft.com/en-us/dynamics365/sales/data-enrichment-agent-faqs

- **AI-powered Data Enrichment for opportunities**

  Broadened the enrichment scope to analyze Teams conversations, transcripts, and AI-generated summaries in addition to emails. Updated workflow and capacity guidance to monitor relevant Teams meetings (where the primary contact attended) and to account for transcript-based credit consumption.

  https://learn.microsoft.com/en-us/dynamics365/sales/data-enrichment-agent-overview

- **Responsible AI FAQ about AI-powered Data Enrichment for opportunities**

  Clarified that enrichment targets opportunity records and now leverages Teams transcripts and AI-generated summaries alongside emails. Documented comprehensive auditing of enrichment actions and specified that Teams-based enrichment applies only when the opportunity’s primary contact attended the meeting.

  https://learn.microsoft.com/en-us/dynamics365/sales/FAQs-data-enrichment-agent

- **FAQ about Copilot in Dynamics 365 Sales**

  Expanded Sales agent capabilities to include drafting sales emails grounded in CRM data, capturing meeting takeaways, and updating fields within the workflow. Added guidance on using the Sales agent within Microsoft 365 Copilot experiences in Outlook and Teams so sellers can act without switching apps.

  https://learn.microsoft.com/en-us/dynamics365/sales/sales-copilot-faq

- **FAQs about Sales Qualification Agent**

  Added a new FAQ explaining that the system creates AI agent user accounts required for agentic workflows, even if the feature is not enabled. Included a reference to the “AI agent users” section in security roles for details.

  https://learn.microsoft.com/en-us/dynamics365/sales/sales-qualification-agent-faq

- **Predefined security roles for Sales**

  Introduced an “AI agent users” section describing system-created users for autonomous agent workflows and warning against deleting them to avoid breaking deployments. Included a table of Sales Qualification Agent users with their app IDs and purposes (lead readiness, research, and outreach preparation).

  https://learn.microsoft.com/en-us/dynamics365/sales/security-roles-for-sales

- **Review and approve Data Enrichment suggestions**

  Expanded enrichment to use Teams meetings in addition to emails, with consent covering both sources. Added requirements for meeting-based suggestions (availability of transcripts or Copilot summaries, association to opportunities via attendee matching, and processing latency) and clarified that citations link to the calendar event visible only to participants, with UI and stakeholder detection updated accordingly.

  https://learn.microsoft.com/en-us/dynamics365/sales/use-data-enrichment-agent