# Dynamics 365 Contact Center
**Date created:** 2026-07-22 UTC  
**Tags:** Administration, AI, Agent, Analytics, Automation, Governance, Monitoring, Other, Programming, Security  

## New Articles

- **Manage the enhanced Active Conversation settings**
  Introduces configuration for the enhanced Active Conversation form, including enabling the Customer 360 component, customization settings, and form selector behavior. Adds best practices, limitations, and guidance to switch between enhanced and default customer profile cards.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/active-enh-conv-settings

- **View Agent insights dashboard**
  Introduces a supervisor dashboard to monitor autonomous agents with KPIs, goal setting, and agent-level insights across conversations and cases. Includes performance summaries for multiple AI agents and an FAQ on enablement and limitations.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/agent-insights

- **View and understand the bot report in Omnichannel real-time analytics**
  Describes the real-time Bot report for Copilot agents with access prerequisites, filters, KPIs, drill-downs, and customization options. Highlights permissions and interactive trend monitoring.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/agent-realtime-dashboard

- **Configure sensitive variable masking for voice agents**
  Explains how to mark Copilot Studio variables as sensitive so recording, transcription, and logging pause during capture. Provides a redaction behavior matrix across nodes, Dataverse, connectors, Power Automate, and telemetry with key considerations and limits.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/agent-sensitive-data-masking

- **Security FAQs about AI agents**
  Covers security, privacy, and compliance for AI agents including data handling, access control, incident management, and responsible AI filtering. Clarifies stack, usage, limitations, and feedback channels with links to relevant policies.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/ai-agents-security-faqs

- **Manage all ongoing conversations**
  Introduces a supervisor view to bulk assign, force close, message customers, and notify representatives across ongoing conversations. Details prerequisites, action limits, and progress tracking via Action History.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/all-ongoing-conversations

- **Best practices for application lifecycle management**
  Provides ALM guidance for using unmanaged solutions in source and managed in target environments to avoid active layer issues. Explains update flows, record deletion via solutions, and version parity considerations.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/alm-best-practices

- **Use /conversations endpoint**
  Documents the GET endpoint to retrieve active custom-channel conversations with pagination. Clarifies filters, response schema, and state scope (excludes Wrap-Up/Closed).
  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/api/api-conversation

- **Use /conversation/{conversationId}/contexts endpoint**
  Describes retrieving conversation context variables with eventual consistency and polling notes. Includes response schema and related messaging API links.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/api/api-conversation-context

- **Use /consumer/conversation/create endpoint**
  Explains the POST endpoint to start customer conversations with customer context, start message, and deflection bypass. Details response schema and record matching logic by email/phone.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/api/api-conversation-create

- **Use /conversation/{id} endpoint**
  Documents sending activities to an ongoing conversation using Bot Framework types (message, typing, end, event), including read receipts and custom events. Notes input validation, response codes, and message ID format.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/api/api-conversation-endpoint

- **Use /conversation/{conversationId}/messages endpoint**
  Covers reading conversation messages with filters and pagination aligned to the Bot Framework activity schema. Provides sample responses and empty-array behavior.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/api/api-conversation-messages

- **Use webhook to receive messages and events**
  Guides configuring a webhook to receive real-time activities for custom channels with Entra authentication and retry policy. Lists supported activity/event types and sample payloads; expects HTTP 200 responses.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/api/api-conversation-webhook

- **Autonomous service agents in Dynamics 365**
  Introduces Customer Intent, Case Management, and Customer Knowledge Management agents, their purposes, and related setup links. Highlights AI-driven intent discovery, automation, and knowledge curation.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/autonomous-agents-overview

- **Bot-Intent dashboard**
  Presents a preview dashboard to analyze bot intent performance with filters, KPIs, and drill-down to intent-level metrics. Requires enabling Customer Intent Agent and historical analytics.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/bot-intent-historical

- **Configure a sample voice agent template**
  Provides an importable Copilot Studio voice agent template with end-to-end configuration steps and a sample order status workflow. Explains prerequisites, language behavior, validation, and escalation setup.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/bot-scenario-configure

- **Build Azure AI agent for Dynamics 365 Contact Center**
  Walks through building a .NET Azure AI agent with Dynamics middleware, handling events, and bridging messages. Shows escalation and end flows via a helper client and testing guidance.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/build-your-azure-agent

- **Calculate segment-based queue metrics**
  Defines DAX measures and columns for segment-level analytics using msdyn_queueextension across real-time and historical contexts. Covers service level, abandon logic, transfer analytics, and bot-excluded variants with modeling guidance.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/calculate-segment-metrics

- **Use CCaaS_CancelDeliveryTask API**
  Adds an API to cancel pending and future proactive delivery attempts with required parameters and auth. Includes sample request and links to related APIs and reporting.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/api/ccaas_canceldeliverytask

- **Use CCaaS_CreateOperation API**
  Enables cancel, suspend, or resume operations for Proactive Engagement with input parameters and response codes. Supports operational control at run time with security requirements.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/api/ccaas_createoperation

- **Use CCaaS_CreateProactiveBulkDelivery API**
  Initiates bulk proactive deliveries (v1 and v2) with detailed payload schemas, consent notes, and samples. Designed for scaling outreach to multiple customers.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/api/ccaas_createproactivebulkdelivery

- **Use CCaaS_CreateProactiveDelivery API**
  Starts proactive voice/SMS deliveries with contact windows, priority, and reattempt logic. Details headers, payload structures, consent considerations, and sample requests.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/api/ccaas_createproactivedelivery

- **Use CCaaS_CreateProactiveSMSDelivery API**
  Initiates proactive outbound SMS with simple parameters and Entra auth, noting unsupported features like reattempts. Recommends CreateProactiveDelivery for advanced needs.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/api/ccaas_createproactivesmsdelivery

- **Use CCaaS_CreateProactiveVoiceDelivery API**
  Starts proactive voice calls and schedules callbacks with scope limits and compliance notes. Details headers, Windows object schema, sample payload, and response.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/api/ccaas_createproactivevoicedelivery

- **Use CCaaS_CreateSimpleProactiveDelivery API**
  Adds an action API for a single proactive delivery with simplified attributes and scheduling windows. Includes consent guidance, full sample, and related links.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/api/ccaas_createsimpleproactivedelivery

- **Use CCaaS_GetDeliveryTasks API**
  Retrieves proactive delivery task status and details with sample payloads and response properties. Supports tracking across contact chaining and deliveries.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/api/ccaas_getdeliverytasks

- **CCaaS_GetPresence**
  Returns real-time agent presence with session details and allowed channels. Documents headers, possible status codes, response keys, and sample curl.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/api/ccaas_getpresence

- **CCaaS_ModifyAgentPresence**
  Modifies an agent’s presence at runtime with impersonation support via MSCRMCallerID. Documents request payload, auth, and response behaviors.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/api/ccaas_modifyagentpresence

- **Use CCaaS_GetRepresentativeAvailabilityBeforeConversation**
  Checks queue and representative availability before starting a conversation with support for CustomContextItems. Includes sample requests, constraints, and status codes.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/api/ccaas-get-representative-availability-before-conversation

- **Use CCaaS_GetRepresentativeAvailabilityForConversation**
  Retrieves availability during an active conversation to inform routing decisions. Shows usage with CustomContextItems and links to related APIs.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/api/ccaas-get-representative-availability-conversation

- **Use Copilot Service admin center**
  Introduces a unified admin app with guided setup, searchable settings, overview pages, and role prerequisites. Explains access and automatic installation behavior.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/cc-admin-center

- **Compliance certification of Dynamics 365 Contact Center**
  Summarizes coverage and certifications (HIPAA, FedRAMP, SOC, ISO, PCI DSS, CSA STAR, UK G-Cloud, DORA support). Directs to the Service Trust Portal for official details.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/implement/cc-compliance-certifications

- **Troubleshooting and FAQs**
  Centralizes troubleshooting entry points and links to key FAQs for routing, Copilot, and voice. Helps users quickly find diagnostic guidance.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/implement/cc-troubleshooting-faqs

- **Overview of Copilot Service workspace**
  Introduces the representative-facing app with Copilot, multisession and tab behavior, and navigation rules. Includes limits, access steps, and links to how-to topics.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/ccw-overview

- **Session closure reasons**
  Details closure reasons in msdyn_ocsession with comprehensive values for agent/customer/system outcomes. Supports analytics and diagnostics with a mapping to option sets.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/closure-reasons-descriptions

- **Configure agents for AI-led proactive engagement in Dynamics 365 Contact Center**
  Explains setup for answering machine detection and passing campaign context to IVR agents via APIs or files. Shows how to return data to Dynamics for reporting.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/configure-agents-for-ai-led-proactive-engagement

- **Configure bullseye routing using conversation orchestration playbooks (preview)**
  Guides bullseye routing with progressive levels, wait-time rules, priority, and overflow handling. Includes user group setup and diagnostics via queries.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/configure-bullseye-routing

- **Configure conversation orchestration in Dynamics 365 Contact Center (preview)**
  Introduces natural language playbooks for dynamic prioritization, overflow, and preferred representative assignment. Details creation, validation, conflict handling, and ALM migration.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/configure-conversation-orchestration

- **Enable Copilot features**
  Shows how to enable and manage Copilot capabilities, control availability via experience profiles, and set user privileges. Covers data capture, language support, and next steps for summaries and help pane features.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/configure-copilot-features

- **Configure the connector for any CRM solution**
  Provides patterns to sync Accounts/Contacts from non-Microsoft CRMs to Dataverse using Power Automate, HTTP actions, webhooks, and plugins. Covers prerequisites, mapping, and flow setup.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/configure-custom-connector

- **Configure a custom messaging channel using messaging APIs**
  Describes end-to-end setup with Entra app registration, webhook implementation, and managed identity linking. Includes JavaScript samples for channel record management and adding to a workstream.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/configure-custom-messaging-channel

- **Configure disposition codes**
  Enables disposition codes globally or per workstream with selection requirements and maximums. Explains management, persistence behavior, and reporting capture.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/configure-disposition-codes

- **Configure fallback actions for the IVR agent**
  Defines fallback behaviors (prompt/hang-up, transfer external, escalate, wait music + escalate) for voice workstreams. Recommends monitoring via “Fallback calls” in analytics.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/configure-fallback-actions-ivr-agent

- **Configure multilingual voice agents**
  Explains multilingual Copilot voice agents, language matching, transcription behavior, and warnings. Covers routing by language and monitoring with Last Language filter.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/configure-multilingual-agents

- **Configure proactive engagement in Dynamics 365 Contact Center**
  Provides comprehensive setup for outbound voice/SMS, dialing modes, display numbers, reattempts, frequency limits, and SMS templates. Details telephony requirements and SBC considerations.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/configure-proactive-engagement

- **Configure quality and coaching skills in Dynamics 365 Contact Center**
  Introduces AI-powered evaluation plans, indicators, and guardrails with nudges and notifications. Includes setup steps, scoring, and best practices.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/configure-quality-coach

- **Configure the connector for Salesforce**
  Guides unidirectional sync from Salesforce to Dataverse with CDC, permissions, and mapping. Details setup, limits, and management actions for updates and diagnostics.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/configure-salesforce-connector

- **Configure screen recording with desktop companion application in Dynamics 365 Contact Center and Dynamics 365 Customer Service**
  Explains enabling screen/audio recording, roles, and capture/upload behavior with retention management. Covers playback permissions, red border, multi-screen, and automated vs. manual recording.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/configure-screen-recording

- **Configure the connector for ServiceNow**
  Describes syncing Accounts/Contacts from ServiceNow to Dataverse using Power Automate flows from GitHub. Includes REST messages, business rules, and predefined mappings.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/configure-servicenow-connector

- **Use AI-generated conversations for agentic simulations in Dynamics 365 Contact Center (preview)**
  Enables AI-driven simulations for voice workstreams with prompts, run history, and transcript review. Documents credit usage, concurrency, duration, and language constraints.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/configure-simulation-agent

- **Configure an SMS channel for Infobip in Dynamics 365 Contact Center**
  Provides end-to-end Infobip SMS setup with API keys, callback URLs, and workstream configuration. Details webhook configuration in Infobip and message flow behavior.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/configure-sms-channel-infobip

- **Configure feedback surveys using Copilot Studio**
  Documents creating multilingual survey agents, publishing, and adding to channels with consent models. Covers runtime, hosting options, analytics, and post-resolution email surveys via Power Automate.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/configure-surveys

- **Configure Teams Phone in voice channel**
  Explains end-to-end integration with Teams Phone including resource accounts, licensing, number assignment, and admin center setup. Covers inbound behavior, known issues, and FAQs.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/configure-teams-phone-in-voice-channel

- **Use Microsoft Azure Virtual Desktop to access voice channel**
  Guides representatives using AVD for voice with multimedia redirection and behavior during disconnects. Offers best practices and links to agent experience.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/configure-voice-avd

- **Configure settings to improve call quality over Citrix virtual desktop**
  Improves voice quality for Citrix users via registry and admin settings, with usage instructions and related links. References reconnection behavior and enhanced call features.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/configure-voice-citrix-virtual-desktop

- **Configure a WhatsApp channel through Azure Communication Services**
  Walks through ACS-based WhatsApp channel setup with Event Grid and authentication. Prepares for Business-Scoped User IDs with routing and integration guidance.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/configure-whatsapp-acs

- **Configure the connector for Zendesk**
  Adds Power Automate-based Zendesk connector setup with flows from GitHub, webhooks, and mappings. Details authentication, incremental sync, and field mapping edits.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/configure-zendesk-connector

- **Trial FAQ—Dynamics 365 Contact Center**
  Answers trial conversion, limitations, supported features, and sample data behaviors. Notes telephony constraints and links to setup resources.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/implement/contact-center-trial-faq

- **Responsible AI FAQ for conversation orchestration**
  Explains ECA playbooks, evaluation metrics, limitations, and responsible-use practices. Offers guidance on monitoring and feedback during preview.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/implement/conversation-orchestration-rai-faq

- **View Copilot analytics report**
  Introduces Copilot usage, productivity, and satisfaction metrics for the standalone experience. Includes access prerequisites, filters, and links to underlying data tables.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/copilot-analytics-report

- **Chat with case data in Customer Service (preview)**
  Shows how to use the Customer Service plugin in Microsoft 365 Copilot to query case data with example prompts. Notes prerequisites, supported data, and review guidance.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/copilot-chat-customer-service-data

- **Enable Copilot to draft emails**
  Explains enabling email drafting in the editor and help pane, knowledge sources, and template recommendations. Details default and configurable case fields used by Copilot.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/copilot-email-enable

- **Enable features in Copilot pane**
  Centralizes configuration for help pane features, translation, filters, and prompt management. Adds Customer Support and Admin Management agents with access controls and extensibility.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/copilot-enable-help-pane

- **Enable summarization of cases and conversations**
  Enables Copilot summaries for cases and conversations with field mapping and exclusions. Describes automatic and on-demand generation and UI placement.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/copilot-enable-summary

- **Copilot feature availability across products**
  Compares Copilot capabilities across Customer Service, Contact Center, and Microsoft 365 Copilot for Service. Highlights supported scenarios, customization, and cross-product behaviors.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/copilot-feature-availability

- **Understand how Copilot supports different languages**
  Explains response language behavior based on UI language and knowledge article tagging. Covers mixed-language handling and standalone vs. embedded constraints.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/copilot-language-support

- **Use Copilot to summarize conversations**
  Guides representatives to generate conversation summaries during or after interactions, with optional case creation. Explains display formats and where to view completed summaries.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/copilot-summarize-conversations

- **Summarize cases in non-Microsoft CRM systems**
  Enables Copilot-generated case and conversation summaries for Salesforce and ServiceNow data. Details source coverage, actions, and preview notes.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/copilot-use-summary

- **Create rollout plans to manage AI agents**
  Introduces Rollout Manager for phased AI agent deployment with plan lifecycle controls. Explains agent-specific considerations when deactivating or deleting plans.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/create-rollout-plans

- **Customize the bot dashboard**
  Shows how to tailor Power BI visuals and add variables to analyze bot fallout and performance. Provides best practices and table references for custom reporting.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/customize-agent-dashboard

- **Customize Copilot conversation summaries**
  Lets admins choose paragraph or structured formats and configure fields like Root Cause and Outcome. Supports reordering and removing unverifiable details.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/customize-copilot-conv-summary

- **Deprecations in Dynamics 365 Contact Center**
  Lists deprecations with dates and guidance, including Apple Messages onboarding, post-call survey toggle, chat draft feature, and legacy voice local hosting. Links to broader deprecation info.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/implement/deprecations-contact-center

- **Diagnose contact center health with the Application Insights dashboard**
  Introduces a Diagnose dashboard to debug routing using Application Insights with live trends and timelines. Details filters, metrics, non-assignment reasons, and event analysis.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/diagnose-dashboard

- **Download call recordings in bulk**
  Provides a Power Automate flow pattern to list recordings, generate SAS URLs, and save to storage. Notes permissions, date filters, expiration, and error handling recommendations.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/download-call-recordings-bulk

- **Use Copilot to draft an email in non-Microsoft CRMs**
  Shows how to draft emails in embedded experiences with prompts, knowledge sources, and refinement options. Covers reviewing suggested replies and starting over.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/draft-email-embedded-experience

- **Use ask a question in non-Microsoft CRM systems**
  Explains Ask a question in embedded Copilot with auto prompts, plugin triggers, translation, and summarization tools. Includes steps and shared includes for consistent behavior.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/embed-ask-question

- **Use Copilot to summarize conversations in non-Microsoft CRM systems**
  Enables conversation summaries in embedded experiences with prerequisites and steps to view results. Reuses common availability and action guidance.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/embed-summarize-conversation

- **Enable Agent insights dashboard and KPI goals**
  Details enabling the Agent insights dashboard and configuring KPI goals for conversations and cases. Supports goal tracking against AI agent performance.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/enable-agent-insights

- **Enable plugins for generative AI (preview)**
  Describes enabling prompt and connector plugins with access controls, auth modes, inputs, and response handling. Notes constraints like single action and re-enable needs after updates.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/enable-copilot-plugins-for-generative-ai

- **Enable Diagnose dashboard**
  Walks through enabling conversation diagnostics and connecting to Application Insights with federated credentials. Includes troubleshooting steps and cost notes.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/enable-diagnose-dashboard

- **Enable fields for account and contact for identifying customers**
  Shows how to map custom fields and update record identification rules for voice channels via OData/PATCH. Includes FetchXML examples and mapping tables.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/enable-fields-identify-customers

- **Enable intent-based suggestions for service representatives**
  Enables intent-based suggestions and next best actions during live or persistent chats. Explains behaviors for unknown intents and case-driven recommendations.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/enable-intent-for-service-reps

- **Error handling in messaging APIs**
  Defines HTTP and RFC 7807 error patterns with specific app error codes and correlation IDs. Helps developers diagnose issues consistently across messaging APIs.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/error-handling

- **Use evaluation criteria**
  Introduces creating and managing quality evaluation criteria with AI-enabled responses and weighted scoring. Covers versioning, inheritance, simulations, and detailed limits.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/evaluation-criteria

- **Use evaluation plan**
  Explains creating and running evaluation plans for cases, conversations, and emails with AI-assisted or manual methods. Covers frequency, sampling, run history, and limits.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/evaluation-plan

- **Responsible AI FAQ for AI agents**
  Details capabilities, evaluation metrics, limitations, data processing, and governance controls for multiple AI agents. Provides responsible-use guidance and feedback channels.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/implement/faq-rai-ai-agents

- **How proactive engagement works in Dynamics 365 Contact Center**
  Explains representative-led and AI-led outbound engagement flows, notifications, and escalation. Advises on honoring do-not-contact requests via disposition codes.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/how-proactive-engagement-works

- **Install and manage desktop companion application for voice channel**
  Provides installation steps, browser extension enablement, and diagnostics collection management. Includes registry settings to control user updates.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/install-manage-desktop-app

- **International availability of Dynamics 365 Contact Center**
  Lists geographic and language availability for digital and voice channels, including GCC considerations. Links to supported languages and system requirements.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/implement/international-availability

- **Overview of messaging APIs**
  Introduces service-to-service messaging APIs with auth headers, base URL format, and supported endpoints. Recommends SDKs for client scenarios and links to references.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/intro-messaging-apis

- **Enable knowledge sources from Microsoft Copilot Studio (preview)**
  Shows how to enable Copilot Studio knowledge sources for use with Copilot, including publishing steps. Notes preview limitations and supported scenarios.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/knowledge-copilot

- **Configure knowledge articles for verbatim responses in Copilot**
  Enables verbatim responses by tagging entire articles or sections, with highlighted source citations. Improves fidelity for authoritative answers in Ask a question.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/knowledge-verbatim

- **Manage Customer Intent Agent**
  Covers enabling, managing LOBs, intent discovery and promotion, instruction authoring, and connectors/tools mapping. Explains propagation timing and rules management.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/manage-customer-intent-agent

- **Manage ongoing record conversations**
  Provides supervisor actions to assign, transfer, release, and remove record conversations, including enhanced intent-based transfers. Details access and related views.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/manage-ongoing-record-conversations

- **Manage quality evaluation**
  Explains enabling and configuring quality evaluation across records, with connection references and flows. Adds regeneration of summaries after evaluator edits and bulk options.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/manage-quality-evaluation-agent

- **Migrate Copilot Studio survey agents configurations**
  Describes migrating survey agent configurations using solutions, with options to include workstreams. Covers connection reference fixes and publishing steps.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/migrate-survey-agents

- **Use msdyn_queueextension to calculate segement-based queue metrics**
  Documents the msdyn_queueextension table structure for segment analytics, durations, and reasons. Supports building queue-level performance insights.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/msdyn-queueextension

- **Responsible AI FAQs for NLUs in AI agents**
  Clarifies NLU options, performance trade-offs, processing locations, and transparency best practices. Guides on responsible evaluation and orchestration choices.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/implement/natural-language-ai-faq

- **View customer information on Active Conversation form**
  Describes the form sections, actions, and summary tabs including self-service and visitor details. Explains linked records and timeline usage.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/oc-active-conv

- **Use on-demand evaluation**
  Enables supervisors to request evaluations for cases, conversations, and emails with AI or manual methods. Details assignment, due dates, and viewing evaluation records.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/on-demand-evaluation

- **Overview of agent hub for administrators**
  Introduces Agent hub with learn, rollout manager, insights, security, and architecture sections. Helps admins adopt and manage autonomous AI agents.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/overview-agent-hub

- **Overview of AI agents and Copilot features**
  Summarizes autonomous agent capabilities and Copilot assistance for representatives across channels. Links to responsible AI FAQs and related guidance.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/overview-ai-agents-copilot-features

- **Dynamics 365 Contact Center overview**
  Provides an overview of AI-first capabilities including autonomous agents, proactive engagement, routing, dashboards, and Teams integration. Includes architecture visuals and next steps.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/implement/overview-contact-center

- **Overview of contact center agents in Dynamics 365 Contact Center**
  Describes Customer Assist, Quality Assurance, and Service Operations agents and their roles. Includes navigation and links to deeper topics.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/overview-contact-center-agents

- **Overview of Customer Intent Agent**
  Explains intent discovery and library management for self-service and assisted service. Shows benefits for representatives and links to setup and rollout.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/overview-customer-intent-agent

- **Overview of proactive engagement**
  Defines proactive engagement, single vs multi-step journeys, and AI-led scheduling. Links to configuration and reporting resources.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/overview-proactive-engagement

- **Overview of Quality Management Agent**
  Introduces quality evaluation, governance, and recording setup within WEM. Links to evaluation plan, criteria, and usage pages.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/overview-quality-management

- **Overview of Service Operations Agent in Dynamics 365 Contact Center**
  Presents an AI assistant for configuring channels, routing, and diagnostics via conversation. Emphasizes unified, guided admin workflows.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/overview-service-operations-agent

- **Synchronize service representative presence status across multiple systems**
  Provides webhook and API patterns to sync presence, with mappings and payload examples. Details OAuth setup and impersonation for updates.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/presence-status-sync

- **Best practices for proactive engagement campaigns in Dynamics 365 Contact Center**
  Outlines global compliance, consent, preference management, and caller ID reputation practices. Helps reduce risk and improve contact outcomes.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/proactive-engagement-best-practices

- **Use proactive engagement dashboard in Dynamics 365 Contact Center**
  Introduces real-time KPIs and visualizations for proactive engagement performance. Defines metrics and provides drill options with related links.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/proactive-engagement-dashboard

- **Dial modes for proactive engagement in Dynamics 365 Contact Center**
  Details Copilot, progressive, predictive, and preview dial modes with algorithms and constraints. Includes compliance notices and links to configuration.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/proactive-engagement-dial-modes

- **Manage consent for proactive engagement in Dynamics 365 Contact Center**
  Shows how to track and enforce opt-outs and consent across delivery methods. Supports bulk uploads, SMS keyword handling, and disposition-based do-not-contact.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/proactive-engagement-manage-consent

- **Outcomes for proactive engagement in Dynamics 365 Contact Center**
  Defines SIP-based voice outcomes, SMS delivery results, AI agent outcomes, and disposition codes. Explains SMS timeout behaviors and reporting storage.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/proactive-engagement-outcomes

- **Use proactive engagement tables for reporting**
  Documents msdyn_proactive_delivery and attribute tables for reporting identifiers, status, timings, and results. Links to related API usage.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/proactive-engagement-tables

- **Proactive Outbound dashboard**
  Introduces historical analytics for outbound engagements with segmentation and filters. Complements real-time dashboards with status and result trends.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/proactive-outbound-dashboard

- **Provision channels in Dynamics 365 Contact Center**
  Explains provisioning steps, trial defaults, failure handling, and turning channels on/off. Helps admins manage supported channels across the org.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/implement/provision-channels

- **View and understand real-time analytics in the User group report**
  Presents a preview real-time report by agent group with filters and metric definitions. Supports drill-down to agent-level presence and session metrics.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/realtime-agent-group-report

- **View and understand real-time analytics in the Intent group report**
  Adds a preview report to monitor performance by intent group with customizable dimensions. Defines group and per-intent metrics and drill behavior.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/realtime-intent-group-report

- **Overview of real-time streaming analytics (preview)**
  Introduces a supervisor portal for live and aggregated metrics with thresholds and trendlines. Details access URLs, filters, and dashboard tabs.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/realtime-streaming

- **Use real-time assisted service in real-time streaming analytics (preview)**
  Describes the Assisted service view with funnels, trends, and overflow metrics. Helps diagnose self-serve containment and assisted service performance.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/realtime-streaming-assisted-service

- **Monitor conversations in real time (preview)**
  Enables conversation monitoring with filters and bulk actions across ongoing and closed items. Includes preview compliance guidance.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/realtime-streaming-conversations

- **Use the Queues view to monitor queue metrics and performance (preview)**
  Monitors queue health with backlog, wait time, ASA, abandon, transfers, callbacks, and service level. Includes formulas, definitions, and preview notes.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/realtime-streaming-queues

- **Monitor representatives in real time (preview)**
  Tracks representative presence, availability, and workload with actions to update queues and reset presence. Visualizes performance and status distribution.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/realtime-streaming-representatives

- **Monitor real-time metrics in the Wallboard view (preview)**
  Provides a wallboard for live operational metrics with five-minute trend updates and thresholds. Supports multi-queue/channel filtering and definitions.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/realtime-streaming-wallboard

- **Use APIs to pause or resume transcription and recording**
  Documents voice module methods to control recording/transcription and completion callbacks. Supports compliance workflows for sensitive data handling.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/api/record-transcription-api

- **Use service representative availability APIs**
  Introduces availability APIs with Entra auth setup and tokens. Links to before/during-conversation endpoints and usage.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/representative-availability-overview

- **Manage omnichannel environments**
  Explains resetting, restoring, recovering, and tenant migration with required re-provisioning steps. Ensures omnichannel capabilities are re-enabled after environment changes.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/implement/restore-environment

- **Responsible AI FAQ for Service Operations Agent**
  Covers purpose, evaluation metrics, limitations, and responsible-use guidance for the Service Operations Agent. Provides feedback and preview channel notes.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/implement/service-operations-agent-rai-faq

- **Set up the embedded experience in Salesforce for Dynamics 365 Contact Center**
  Guides embedding the conversation widget in Salesforce via Call Center XML and utility setup. Includes Copilot connection options and version guidance.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/set-up-embedded-experience

- **Set up the embedded experience in ServiceNow for Dynamics 365 Contact Center**
  Explains embedding the conversation widget using ServiceNow OpenFrame configuration. Lists prerequisites and references panel docs.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/set-up-embedded-experience-servicenow

- **Configure intent-based suggestions for Copilot agents**
  Configures intent-based suggestions in Copilot Studio, connection references, and enrichment context. Details escalation logic, variables, and publishing updates.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/set-up-intent-agent

- **Set up microphone connection on representative sign-in**
  Adds a toggle to pre-connect microphones at sign-in to reduce call setup latency. Explains runtime behavior and where to configure.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/set-up-microphone-connection

- **Set up voice agents to use intents**
  Connects voice-enabled Copilot agents with Customer Intent Agent for intent-driven flows and escalation. Details configuration, instructions, IVR integration, and service principal setup.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/set-up-voice-agents-to-use-intents

- **System requirements for Dynamics 365 Contact Center**
  Lists prerequisites, supported browsers, network allowlists, ACS dependency, and hardware/bandwidth recommendations. Covers embedded experiences and customer widget compatibility.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/implement/system-requirements-contact-center

- **Transfer conversations from customer service representatives to AI agents**
  Explains representative-to-AI transfer scenarios across queues with capacity considerations. Documents event sequences and greeting triggers for the receiving AI agent.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/transfer-to-agents

- **Transparency note for constrained speech recognition**
  Provides responsible AI guidance, grammar design best practices, performance metrics, and fairness considerations for constrained speech use. Clarifies intended vs. unsupported uses.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/implement/transparency-note

- **Transparency note for real-time agents in Dynamics 365 Contact Center**
  Details architecture, capabilities, limitations, performance metrics, and evaluation framework for real-time voice agents. Recommends safeguards, monitoring, and fallback strategies.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/implement/transparency-note-real-time-voice-agents

- **Trust center for Dynamics 365**
  Summarizes security, privacy, and compliance practices including role-based controls, data governance, and prompt shielding. Provides transparency into operations and complaint handling.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/trust-center

- **Sign up for a free trial—Dynamics 365 Contact Center**
  Walks through trial signup steps, availability, and included features with links to try core scenarios. Notes personal email limitations and provides training resources.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/implement/try-dynamics365-contact-center

- **Ask a question**
  Describes Copilot’s Ask a question with case summarization, auto/prompts, plugin triggers, translations, and verbatim source checking. Includes examples and related links.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/use-ask-a-question

- **Write an email with Copilot**
  Shows agents drafting emails via editor and help pane, using templates and knowledge sources with refinement options. Explains actions, tone adjustments, and iterative prompts.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/use-copilot-email

- **Use evaluations**
  Guides viewing and managing evaluations, scoring, states, and editing submitted results. Adds regeneration behavior for summaries and links to related management pages.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/use-evaluations

- **Use intent-based suggestions**
  Teaches representatives to leverage identified intents and next best actions, send suggested questions, and request solutions. Covers handling changes, history, and feedback.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/use-intent-suggestions

- **Use Quality Assurance Agent**
  Introduces real-time monitoring, alerts, and coaching for supervisors with compliance guidance. Details prerequisites and configuration steps for the “Quality and coaching” skill.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/use-quality-assurance-agent

- **Use quality and coaching skills**
  Shows supervisors monitoring QAA conversations, trends, and AI summaries, and representatives receiving coaching nudges. Explains navigation and transcript-embedded guidance.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/use-quality-coach

- **Use representative availability APIs from Copilot Studio**
  Explains invoking availability APIs in the Escalate system topic with OAuth connections and branching logic. Provides examples for before/during-conversation checks.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/use-representative-availability-api

- **Use Service Operations Agent in Dynamics 365 Contact Center**
  Details conversational configuration for channels, queues, routing rules, and diagnostics. Includes connection setup, troubleshooting, and prompt examples.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/use-service-operations-agent

- **Use agent dashboard and call controls in the voice channel**
  Covers making/receiving calls, consult and transfer workflows, recording/transcription controls, and spam reporting. Provides quality tips for Citrix/AVD and troubleshooting guidance.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/voice-channel-agent-experience

- **Use the desktop companion application with the voice channel**
  Explains using the desktop app during web issues to control calls and view status. Includes device settings, test calls, and support file generation.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/voice-dca-application

- **What's new in Dynamics 365 Contact Center**
  Introduces the AI-first contact center and highlights generative AI capabilities with a link to try and to requirements. Sets expectations for ongoing feature additions.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/implement/whats-new

- **Use the real-time adherence tracker**
  Enables supervisors to monitor adherence vs. schedule with list, Gantt, and summary views. Details prerequisites and filtering by time zone and shift plan.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/workforce-management-adherence-tracker

- **Create and manage capacity plans**
  Adds capacity planning for staffing with short/long-term horizons and auto-extension. Explains configuration inputs, views, filters, and drill navigation.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/workforce-management-capacity-planning

- **Enable capacity planning**
  Shows how to turn on capacity planning in the admin center and where to access it. Links to user setup prerequisites.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/workforce-management-configure-capacity-planning

- **Enable forecasting**
  Enables long/short-term forecasting with scenario modeling and connections to capacity plans. Describes prerequisites and admin center steps.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/workforce-management-configure-forecast-scenarios

- **Enable the representative calendar**
  Enables the representative calendar to visualize scheduled activities. Provides steps to turn on scheduling in admin settings.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/workforce-management-configure-representative-calendar

- **Create a time-off request**
  Guides representatives to submit time-off with required fields and manager notifications. Clarifies workflow and where to access the form.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/workforce-management-create-time-off-request

- **Estimate AI agent credits from forecasts**
  Adds AI credit estimation from forecasting scenarios for supported agents with totals and monthly views. Helps refine planning with adoption assumptions and comparisons.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/workforce-management-credit-estimation

- **Enable adherence historical analytics**
  Enables historical adherence analysis to understand trends and workforce insights. Details admin steps to activate analytics.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/workforce-management-enable-adherence-historical-analytics

- **Enable schedule management**
  Turns on schedule management, including agent acceptance windows and auto-reject behavior. Improves staffing coordination and schedule governance.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/workforce-management-enable-schedule-management

- **Enable shift-based routing**
  Enables routing based on representatives’ shifts and time-off to avoid off-duty assignments. Provides simple steps to activate in admin settings.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/workforce-management-enable-shift-based-routing

- **Enable shift bids**
  Enables shift bidding so agents can request preferred shifts and supervisors can manage bids. Describes prerequisites and admin steps.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/workforce-management-enable-shift-bids

- **Enable shift swapping**
  Allows representatives to swap shifts with expiry controls set by admins. Provides steps to enable and configure basic parameters.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/workforce-management-enable-shift-swapping

- **Create and manage forecast scenarios**
  Guides creating short/long-term forecast scenarios with channels/queues, schedules, and data sources. Details viewing, running on demand, and capacity planning refresh.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/workforce-management-forecast-scenarios

- **Import historical data**
  Defines CSV schemas for daily and intraday forecasting inputs and how to upload. Supports external data sources for scenario creation.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/workforce-management-import-historical-data

- **Install the Workforce Management for Customer Service package**
  Provides steps to install the WFM package via Power Platform admin center. Includes prerequisites and related setup links.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/workforce-management-package-installation

- **Use shift bidding to select shifts**
  Explains how agents submit bids against released plans from Request Management. Outlines steps to review details and save requests.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/workforce-management-representative-shift-bidding

- **Manage schedules in Workforce Management**
  Teaches supervisors to view, adjust, publish, and manage schedules with filters, activities, and rep calendars. Covers editing behaviors and publishing constraints.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/workforce-management-schedule-workforce

- **Configure shift activity types**
  Sets up activity types with productivity, duration, colors, and adherence tolerances. Notes break distribution eligibility and adherence behavior.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/workforce-management-shift-activity-types

- **Create and schedule a shift plan**
  Walks supervisors through building shift plans with activities, skills, and queues. Explains required fields and managing the activity itinerary.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/workforce-management-shift-plan

- **Create and manage shift rotation policies**
  Introduces rotation policies with cadence, slots, activation date, and constraints. Details lifecycle actions and effects on scheduling.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/workforce-management-shift-rotation-policies

- **Configure time-off requests**
  Sets up time-off request types with colors and owner; enables supervisor notifications and scheduling visibility. Lists prerequisites for user management and manager assignment.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/workforce-management-time-off-request-types

- **Use the adherence history report**
  Explains adherence calculations, statuses, and a worked example with intervals and tolerance. Shows filters, summaries, and activity grid usage.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/workforce-management-use-adherence-history-report

- **Schedule representatives with auto-schedule**
  Automates schedule generation with criteria, availability order, and break distribution rules. Supports acceptance workflows and requires eligible activity types.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/workforce-management-use-auto-schedule

- **Set up your workforce with roles and skills**
  Guides admins through creating users, roles, skills, bookable resources, and work hours. Centralizes WFM user setup in the admin center.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/workforce-management-user-management

- **Use shift swapping**
  Lets agents create shift swap requests with availability preferences and public posts to eligible peers. Explains selection of bookings and notification behavior.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/workforce-management-use-shift-swapping

- **View and take action on time-off requests**
  Enables supervisors to review, approve, or reject time-off with visibility into details and totals. Supports notifications when enabled.
  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/workforce-management-view-time-off-requests