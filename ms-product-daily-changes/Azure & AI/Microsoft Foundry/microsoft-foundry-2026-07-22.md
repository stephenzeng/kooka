# Microsoft Foundry
**Date created:** 2026-07-22 UTC  
**Tags:** Administration, Agent, AI, Governance, Monitoring, Programming, Security  

## New Articles

- **Microsoft Foundry Notification Center overview**

  Introduced a new overview of the Notification Center, explaining its purpose, in-app delivery, and how it centralizes alerts. Describes key capabilities like an unread indicator, Dismiss All, and a View All page with filtering and sorting for historical messages. Highlights supported notification types—including security alerts, policy/compliance events, and run completions or failures—and how to access and manage them. Links to related observability and RBAC guidance to help teams operationalize notifications effectively.

  https://learn.microsoft.com/en-us/azure/foundry/concepts/concept-notification-center

- **Export hosted agent telemetry by using OpenTelemetry**

  Added a how-to guide for exporting hosted agent traces, logs, and metrics with OpenTelemetry alongside the default Application Insights export. Explains enabling OTLP export via environment variables, storing sensitive headers in a project connection, and running dual export to both destinations. Provides YAML examples, notes on service naming and version immutability, and tuning via standard OpenTelemetry variables. Includes troubleshooting for missing telemetry, auth failures, and ensuring Application Insights continues to receive data.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/configure-hosted-agent-telemetry

- **Secure your Azure Language data and deployment**

  Published a best-practices guide covering security for Azure Language in Foundry Tools across data protection, IAM, and network controls. Details service-specific guidance (for PII detection, NER, custom models, language detection, health) plus legacy features, with recommendations for logging, RBAC, Key Vault, private networking, and CMK. Explains deployment considerations (native vs container), retention and residency, monitoring and alerting, and governance with Azure Policy and security assessments. Helps teams design compliant, least-privilege, and resilient Language deployments.

  https://learn.microsoft.com/en-us/azure/ai-services/language-service/secure-deployment

## Major Changes

- **Hosted agents in Foundry Agent Service**

  Clarified versioning by stating that each agent endpoint serves a single immutable version at a time and routes 100% of traffic to it. Removed prior guidance on canary or blue/green patterns, noting that traffic splitting isn’t supported. Eliminated the suggestion to skip creating versions when parameters are unchanged to reinforce explicit versioning practices.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/hosted-agents

- **Manage hosted agents**

  Updated management guidance to require routing all traffic to one agent version and removed traffic-splitting examples. Added an important directive to configure a single FixedRatio rule set to 100% and raised the Python SDK requirement to azure-ai-projects>=2.3.0. Removed preview headers from examples and clarified how to select versions via REST/SDK and how azd behaves.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/manage-hosted-agent

- **Lucene query syntax in Azure AI Search**

  Substantially expanded explanations of query behavior, ranking, and precedence. Clarified OR handling under searchMode, refined examples and terminology, and deeply elaborated on boosting—including scope rules, field interactions, and analyzer effects. Added guidance and examples to help authors design more precise, better-ranked queries and understand exceptions for wildcard, regex, and fuzzy queries.

  https://learn.microsoft.com/en-us/azure/search/query-lucene-syntax

- **Create, test, and deploy a toolbox in Foundry**

  Enhanced File Search guidance to support dynamic vector stores alongside pinned configurations. Added examples across REST, Python, .NET, JavaScript, and azd showing how to supply vector_store_ids at runtime and clarified argument patterns. Updated user isolation notes to state that any referenced vector stores are shared among users, and noted the preview header requirement for the toolbox MCP surface.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/toolbox

- **How to use the Voice Live API**

  Expanded the list of supported azure-realtime-native voices into a comprehensive catalog with Locale and Voice Detail. Added many new voices across multiple locales and described ideal use cases to guide selection. Retained the default behavior note while improving discoverability of voice options.

  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/voice-live-how-to

## Moderate Changes

- **Deploy a hosted agent**

  Raised the Azure AI Projects SDK requirement to version 2.3.0 and updated installation steps. Removed preview-only headers and flags in Python, REST, and curl examples to reflect GA usage.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/deploy-hosted-agent

- **Deploy a hosted agent from source code**

  Removed the outbound access requirements for bundled dependency resolution and the related provisioning note. Guidance now points to the virtual network deployment article for network configuration.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/deploy-hosted-agent-code

- **Fireworks models on Microsoft Foundry**

  Clarified that deprecations apply only to the Pay-per-token offering, not the models themselves, and listed affected models. Added a deprecation date for FW-GLM-5.1 and FW-MiniMax-M2.5 Pay-per-token and confirmed PTU remains available for all six models.

  https://learn.microsoft.com/en-us/azure/foundry/how-to/fireworks/enable-fireworks-models

- **Isolate hosted agent sessions per user**

  Removed preview notices and headers to reflect GA. Examples now use x-ms-user-identity without preview opt-in and omit the previous troubleshooting for missing preview headers.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/isolate-sessions-per-user

- **MAI-Transcribe in Azure Speech (preview)**

  Marked the mai-transcribe-1 model as deprecated effective Aug 20, 2026. No other changes were made.

  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/mai-transcribe

- **Manage hosted agent sessions**

  Updated guidance from preview to GA by requiring azure-ai-projects>=2.3.0 and removing preview-only flags and beta surfaces. Python examples now use project.agents, and REST examples remove preview headers while preserving the x-ms-user-isolation-key where needed.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/manage-hosted-sessions

- **Migrate from agent applications to the new agent endpoint and publishing experience**

  Adjusted the FAQ to remove traffic splitting from capabilities exclusive to the new agent model. Clarified the remaining advantages like multiple protocols, enable/disable, and A2A.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/migrate-agent-applications

- **Migrate hosted agents to the latest version**

  Increased the minimum Azure AI Projects SDK to 2.3.0 and moved examples from beta to stable SDK surfaces. Refined endpoint version routing guidance and removed preview headers and allow_preview requirements in REST and agent_name scenarios to align with GA.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/migrate-hosted-agent-preview

- **OData `search.score` function in Azure AI Search**

  Added a Limitations section explaining that search.score() can’t be used in $orderby for pure vector or hybrid queries and will return HTTP 400. Clarified syntax applicability to full-text queries and updated examples to reference relevance scores.

  https://learn.microsoft.com/en-us/azure/search/search-query-odata-search-score-function