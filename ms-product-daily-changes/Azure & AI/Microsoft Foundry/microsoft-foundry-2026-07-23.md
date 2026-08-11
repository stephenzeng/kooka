# Microsoft Foundry
**Date created:** 2026-07-23 UTC  
**Tags:** Administration, Agent, AI, Automation, Governance, Monitoring, Programming, Security  

## New Articles

- **Reminder tool for self-scheduling hosted agents**

  Introduced a new how-to for the reminder_preview tool that lets hosted agents reschedule themselves after a specified delay to continue work without manual intervention. It explains prerequisites, tool arguments (minutes and input), and behavior that re-invokes the same hosted agent within the same conversation using a scheduled routine. Step-by-step setup is provided for portal, SDKs (Python, C#, JavaScript), REST, and Azure Developer CLI, along with YAML examples and an end-to-end pattern for polling long-running tasks. It also clarifies limitations such as hosted agents only and supported delay ranges, and links to related toolbox and routine guidance.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/reminder-tool

- **Restrict access to sensitive content in Microsoft Foundry traces**

  Added guidance to protect sensitive generative AI trace data by routing message content and tool call details to the AppGenAIContent table and restricting access via Azure RBAC. The article covers enabling the dedicated table with preview feature flags, marking it as Protected, and granting access through the Privileged Monitoring Data Reader role with PIM considerations. It includes verification steps and a migration timeline detailing default behavior changes on September 30, 2026 and opt-out deprecation on September 30, 2027. Related links help teams configure protected tables and set up tracing consistently.

  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/traces-sensitive-content

## Major Changes

- **Query Knowledge Base via API or MCP**

  Expanded troubleshooting for the retrieve action in 2026-05-01-preview, mapping key HTTP status codes to causes and concrete remediation steps. Clarified partial content handling, where activity entries can include errors for 206 responses, and noted that some 502 failures surface only at the top-level error. Updated guidance on requiring a knowledge source to succeed, specifying failOnError behavior and pointing to the new troubleshooting section. This improves diagnosis of configuration issues, invalid requests, and transient failures with clearer next actions.

  https://learn.microsoft.com/en-us/azure/search/agentic-retrieval-how-to-retrieve

- **Debug Sessions in Azure AI Search**

  Clarified that debug sessions aren’t supported with shared private links and removed earlier guidance implying private environment support. Added a recommended workaround using a separate test search service with synthetic content when private connectivity is required. For managed identity, it details required permissions and trusted services settings to ensure write access for session state in Storage. These changes set accurate expectations and reduce time spent on unsupported configurations.

  https://learn.microsoft.com/en-us/azure/search/cognitive-search-debug-session

- **Microsoft Entra authentication with the Speech SDK**

  Reworked authentication examples across C#, C++, Java, and Python to use TokenCredential-based Microsoft Entra auth with custom domain endpoints. Samples for common recognizer and synthesizer scenarios now create configs from endpoints plus TokenCredential rather than constructing aad# tokens. The VoiceProfileClient Entra guidance was removed, and Python examples were corrected for variable use. This modernizes authentication patterns and reduces token handling complexity.

  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/how-to-configure-azure-ad-auth

- **Routines in Foundry Agent Service (preview)**

  Extended routines to support event-based triggers alongside timer and recurring schedules, starting with a GitHub issue trigger. Added guidance on authenticating event triggers via project connections and documented the end-to-end flow for externally driven runs. Introduced agent-scheduled reminders via a new tool for hosted agents, enabling agents to defer and resume work autonomously. Preview limitations were updated to reflect supported trigger types.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/routines

- **Automate agents with routines (preview)**

  Added an event trigger for GitHub issue opened/closed events with comprehensive setup via portal, REST, SDKs, and Azure Developer CLI. Expanded action definitions to accept an optional input field and clarified that GitHub payloads overwrite action input on delivery, with updated examples across languages and YAML. Included extensive C# samples and documented constraints such as agents that require end-user identity. A new section explains self-scheduling using the reminder tool to simplify long-running or deferred workflows.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/use-routines

## Moderate Changes

- **Model-based echo cancellation with the Microsoft Audio Stack**

  Added instructions to override the echo cancellation model path via AudioProcessing_EchoCancellationModelPath on AudioProcessingOptions, requiring Speech SDK v1.51.0 or later. Clarified configuration scope and provided C# and C++ examples to ensure predictable setup.

  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/audio-processing-model-based-echo-cancellation

- **Run evaluations in the cloud by using the Microsoft Foundry SDK**

  Refactored Python samples to use the TestingCriterionAzureAIEvaluator class for test criteria across multiple evaluation scenarios. Added practical dataset bootstrapping tips and links to runnable GitHub samples for end-to-end workflows, improving learnability and reuse.

  https://learn.microsoft.com/en-us/azure/foundry/how-to/develop/cloud-evaluation

- **Document-based PII overview**

  Introduced a new playground experience in the Microsoft Foundry portal for document-based PII detection with curated samples. It shows side-by-side redacted output with entity categories, confidence scores, and file-fidelity metrics, with a link to step-by-step usage guidance.

  https://learn.microsoft.com/en-us/azure/ai-services/language-service/personally-identifiable-information/document-based-pii-overview

- **Use the document PII playground in Microsoft Foundry**

  Expanded coverage of playground capabilities, including curated sample documents with expected outputs and a side-by-side results view aligned with production API behavior. Guidance encourages starting with samples or uploading your own files and adds notes on assessing layout fidelity alongside redaction accuracy.

  https://learn.microsoft.com/en-us/azure/ai-services/language-service/personally-identifiable-information/document-based-pii-playground

- **Enable incoming A2A on a Foundry agent (preview)**

  Simplified A2A setup by removing the need to set a custom agent card path; Foundry now resolves the default path and negotiates protocol versions automatically. Updated REST and PowerShell examples to omit AgentCardPath and removed outdated portal limitations.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/enable-agent-to-agent-endpoint

- **Generate a synthetic evaluation dataset (preview)**

  Replaced the inline region list with a centralized reference for supported regions and added links to runnable Python samples. This streamlines maintenance and helps users quickly stand up end-to-end generation and evaluation flows.

  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/evaluation-dataset-synthetic

- **Microsoft Foundry portal general availability overview**

  Updated feature readiness to reflect current GA and preview statuses, including Playgrounds and publishing agents to Microsoft 365 Copilot and Teams. Added Routines (Preview), Agent optimizer (Limited preview), and clarified Workflow deprecation with retirement date and migration guidance to Microsoft Agent Framework. Also refined tracing status and added Convert traces to evaluation datasets (Preview), with warnings to avoid new dependencies on deprecated features.

  https://learn.microsoft.com/en-us/azure/foundry/concepts/general-availability

- **Connect agents to Model Context Protocol servers**

  Added a turnkey private networking setup option via the 11-private-network-basic-vnet template for users who prefer not to bring their own resources. Clarified private networking requirements and pointed to the dedicated setup page for end-to-end configuration.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/model-context-protocol

- **What is PII detection in Azure Language?**

  Announced the general availability of the Document PII playground, offering curated samples and a single view to compare detection results across entity types. Clarified parity with production API behavior and called out supported native document formats such as .pdf, .docx, and .txt.

  https://learn.microsoft.com/en-us/azure/ai-services/language-service/personally-identifiable-information/overview

- **Detect and redact PII in native documents**

  Promoted the Microsoft Foundry portal playground with a tip linking to step-by-step instructions and updated redaction configuration to use policyKind options. Added notes that the UI surfaces entity categories, confidence scores, and file-fidelity outputs aligned with API artifacts, and removed outdated preview notices.

  https://learn.microsoft.com/en-us/azure/ai-services/language-service/personally-identifiable-information/how-to/redact-document-pii

- **Make outbound connections through a shared private link**

  Clarified that debug sessions aren’t supported with shared private links and removed references to storing debug session state for indexer skillset operations. Added a link to a workaround path so teams can test without private endpoint constraints.

  https://learn.microsoft.com/en-us/azure/search/search-indexer-howto-access-private

- **Azure OpenAI SDK language support**

  Updated the heading and introduction to clarify SDK usage with the Azure OpenAI v1 endpoint and highlight supported languages. Recommends using the Responses API for new apps while noting Chat Completions for existing message-based solutions.

  https://learn.microsoft.com/en-us/azure/foundry/openai/supported-languages

- **Create, test, and deploy a toolbox in Foundry**

  Added a new Reminder section introducing the reminder_preview tool that lets hosted agents schedule themselves to run later. Included availability notes, an illustrative image, and a link to detailed setup and usage guidance.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/toolbox

- **What's new in Azure Language in Foundry Tools?**

  Announced GA for the Document PII playground and detailed its refreshed capabilities, including curated sample inputs, single-view results across entity types, and alignment with production API and policies. Updated references to reflect GA status and guidance on moving from samples to live documents.

  https://learn.microsoft.com/en-us/azure/ai-services/language-service/whats-new