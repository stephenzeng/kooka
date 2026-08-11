# Microsoft Foundry
**Date created:** 2026-08-07 UTC  
**Tags:** Administration, Agent, AI, Automation, Governance, Monitoring, Programming, Security  

## New Articles

- **How to transcribe multichannel audio in real time - Speech service**

  Introduced a step-by-step guide for real-time transcription of up to two audio channels with per-channel results, tailored for scenarios like stereo call recordings. Outlines supported and unsupported features, latency considerations during overlapping speech, and nuances when combining diarization with multichannel recognition. Provides SDK-specific implementation guidance across multiple languages and highlights that results from different channels may arrive out of order. Includes links to related recognition, audio concepts, and batch transcription topics.

  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/how-to-recognize-speech-multichannel

- **Quickstart: Optimize a prompt agent (preview)**

  Added a quickstart that walks through optimizing a prompt agent using the portal’s optimization wizard. It covers prerequisites, selecting optimization targets and evaluation datasets, choosing evaluators, submitting and monitoring runs, and comparing baseline versus candidates. Shows how to promote the best candidate to a new agent version and calls out limitations for tool-description optimization. Includes related links to the overview, hosted agent optimization, and trace-to-dataset conversion.

  https://learn.microsoft.com/en-us/azure/foundry/agents/quickstarts/quickstart-optimize-prompt-agent

- **Configure Microsoft Entra authentication for Foundry Agent trace ingestion (preview)**

  Introduced guidance to secure agent trace ingestion into Application Insights using project managed identity and role-based access control. Details prerequisites, disabling local auth, and configuring the connection with Auth type set to Project Managed Identity, including automatic and manual role assignments. Provides additional steps for hosted agents, notes OpenTelemetry semantic conventions, and includes troubleshooting for common configuration and permission issues.

  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/trace-ingestion-entra-authentication

## Major Changes

- **Agent optimizer in Foundry Agent Service overview (preview)**

  Expanded the scope to cover both prompt agents and hosted agents, with dedicated guidance and workflows for each. Clarified optimization steps, including baseline selection, dataset and evaluator choice, and application of candidate improvements. Improved explanations of candidate generation, model configuration differences, and result presentation across portal and CLI. Added a matrix for optimization targets and updated limitations, with links to related prompt-agent content.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/agent-optimizer-overview

- **Deployment overview for Microsoft Foundry Models**

  Repositioned “Serverless API” as the primary deployment path and added an “instant access (preview)” option for eligible models. Clarified decision flow across instant access, Serverless API variants, and managed compute, and noted that Foundry selects deployment type per chosen model. Substantially updated managed compute details (supported model families, runtimes, accelerators, and billing) and refreshed getting-started guidance. Revised the comparison to focus on Serverless API versus managed compute and excluded instant access from the comparison.

  https://learn.microsoft.com/en-us/azure/foundry/concepts/deployments-overview

- **Configure a vectorizer in a search index**

  Added a warning that GET responses redact httpHeaders and explained how to resubmit values during updates, including rules tied to URI changes. Updated examples to use explicit placeholders, renamed parameters to align with current API (customWebApiParameters), changed the sample URI, and specified the HTTP method. These changes improve security clarity and help avoid configuration errors.

  https://learn.microsoft.com/en-us/azure/search/vector-search-how-to-configure-vectorizer

## Moderate Changes

- **Audio concepts in Azure Speech in Foundry Tools**

  Clarified that real-time speech to text can transcribe up to two channels independently and label results by source channel, with a pointer to multichannel guidance. Confirmed that text to speech remains mono only.

  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/concepts/audio-concepts

- **Work with chat completion models**

  Added a note on reasoning models (GPT-5 series): they use max_completion_tokens, ignore temperature/top_p/penalties, and require reasoning_effort=none for tool calls via Chat Completions on gpt-5.6+. Directed users to the Responses API for tool calling with reasoning models and linked to reasoning model guidance.

  https://learn.microsoft.com/en-us/azure/foundry/openai/how-to/chatgpt

- **Deploy Microsoft Foundry Models to managed compute with pay-as-you-go billing (classic) **

  Expanded the supported models list, adding EngineeringGroup’s EngGPT2-16B-A3B, Inception Labs’ Mercury-2, and Voyage models for multimodal embeddings and reranking. This broadens deployment options for chat, embeddings, and ranking workloads.

  https://learn.microsoft.com/en-us/azure/foundry-classic/how-to/deploy-models-managed-pay-go

- **Configure AI Gateway in your Foundry resources**

  Enhanced monitoring guidance with steps to route API Management diagnostics to Log Analytics and a sample Kusto query to validate traffic. Clarified rate-limit responses, distinguishing 429 for TPM exceedance and 403 for overall token quota limits.

  https://learn.microsoft.com/en-us/azure/foundry/configuration/enable-ai-api-management-gateway-portal

- **Features of Azure AI Search**

  Removed “preview” labels from Knowledge bases, Knowledge sources, and Agentic retrieval to indicate GA status. Also made wording and capitalization refinements for clarity and consistency.

  https://learn.microsoft.com/en-us/azure/search/search-features-list

- **What is speech to text?**

  Added a new section on real-time multichannel transcription supporting up to two independent channels with per-channel tagging. Included example use cases and a link to the detailed how-to for setup.

  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/speech-to-text

- **Set up tracing in Microsoft Foundry**

  Streamlined setup by replacing detailed steps with shared include snippets for connecting Application Insights from Traces and Project details. Added a reference for configuring Microsoft Entra authentication for agent trace ingestion, while retaining readiness checks.

  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/trace-agent-setup

- **Custom Web API vectorizer**

  Clarified httpHeaders handling, including a new section on updating header values when GET returns <redacted> and rules when the URI changes. Explained prohibited headers, the purpose of the <redacted> sentinel, and updated sample configurations to use neutral placeholders.

  https://learn.microsoft.com/en-us/azure/search/vector-search-vectorizer-custom-web-api