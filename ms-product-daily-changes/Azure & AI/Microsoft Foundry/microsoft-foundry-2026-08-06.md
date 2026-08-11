# Microsoft Foundry
**Date created:** 2026-08-06 UTC  
**Tags:** Administration, AI, Agent, Automation, Monitoring, Programming, Security  

## Major Changes

- **How to use the Azure AI Content Safety Content Provenance Detection API**

  Standardized the API to “Content Provenance Detection,” expanded media support to include audio, and renamed the detection path to /contentsafety/provenance:detect. Updated authentication guidance to use the resource Endpoint with Microsoft Entra ID and clarified response fields, including allowed types and semantics. Troubleshooting now focuses on obtaining a valid Entra token for https://cognitiveservices.azure.com and adjusts the required Storage role to Storage Blob Data Reader.

  https://learn.microsoft.com/en-us/azure/ai-services/content-safety/how-to/how-to-provenance-detection

- **Create and Use Memory**

  Added end-to-end C# samples that show inspecting tool calls in agent responses and full CRUD operations for the Memory Store, with package versions pinned to 2.1.0-beta.4 for stability. Guidance notes how to reuse the responseClient and demonstrates practical memory management patterns. These updates make it easier to adopt memory features reliably in .NET solutions.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/memory-usage

- **Azure OpenAI reasoning models**

  Expanded guidance for reasoning models, including token behavior, context management, and cost controls. Introduced reasoning.mode (standard vs. pro) for gpt-5.6, detailed reasoning.context options to persist reasoning across tool calls, and added a Phase parameter to avoid premature finalization in long workflows. Updated feature tables, provided Python/REST examples, and added prompting best practices so teams can tune latency, cost, and quality for real-world scenarios.

  https://learn.microsoft.com/en-us/azure/foundry/openai/how-to/reasoning

- **Foundry Local CLI reference**

  Overhauled commands for local models, replacing legacy subcommands with streamlined “foundry run” and “foundry chat” for interactive use. Introduced clearer list options (for example, --device, --type, --search, --cached, --loaded, --variants) and removed deprecated syntax and examples. Updated integration steps (such as Open WebUI) to use the new commands and cleaned up outdated content for a simpler, more consistent CLI experience.

  https://learn.microsoft.com/en-us/azure/foundry-local/reference/reference-cli

- **How to use the Voice Live API**

  Added Live-Reference AEC configuration so clients can provide a playback reference for improved echo cancellation, available from API version 2026-07-15. Documented required settings for client-side reference (stereo PCM16 with mic on channel 0 and reference on channel 1) and constraints that audio parameters cannot change mid-session. Clarified default server behavior, recommended Live-Reference AEC for nonstandard playback, and included a JSON example and sample reference.

  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/voice-live-how-to

## Moderate Changes

- **Create a Knowledge Base**

  Added links to model lifecycle and retirement documentation and clearly marked several GPT-4 family models as deprecated in the model table. This helps teams plan migrations while keeping supported API versions unchanged.

  https://learn.microsoft.com/en-us/azure/search/agentic-retrieval-how-to-create-knowledge-base

- **Tutorial: Build an Agentic Retrieval Solution**

  Updated the recommended model from gpt-4.1-mini to gpt-5-mini across prerequisites, configuration, code, and performance notes. Added a deprecation notice for GPT-4 family models with a pointer to the retirement schedule to guide safe adoption.

  https://learn.microsoft.com/en-us/azure/search/agentic-retrieval-how-to-create-pipeline

- **azure.yaml reference for hosted agents**

  Clarified that azd deploy now packages and uploads source for remote builds or deploys a prebuilt image before creating a hosted agent version. Updated azd down to explain it removes the resource group only when the current environment created the Foundry project, preserving existing projects and resources otherwise.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/azure-yaml-reference

- **Document Layout skill**

  Removed the “(preview)” label for Microsoft Entra ID authentication in programmatic billing to reflect general availability. No regional or link changes were made.

  https://learn.microsoft.com/en-us/azure/search/cognitive-search-skill-document-intelligence-layout

- **Configure Claude Code for Microsoft Foundry**

  Updated Model Router support to replace claude-opus-4-1 with claude-opus-4-7 and add claude-opus-4-6, alongside haiku-4-5 and sonnet-4-5. Added guidance that some newer Claude models may not be routed and should be deployed directly if needed.

  https://learn.microsoft.com/en-us/azure/foundry/foundry-models/how-to/configure-claude-code

- **How to configure network isolation for Microsoft Foundry**

  Removed “Traces” from the unsupported features list, indicating improved Private Link/network isolation support. This enables more complete private networking scenarios.

  https://learn.microsoft.com/en-us/azure/foundry/how-to/configure-private-link

- **Quickstart: Agentic retrieval in the Azure portal**

  Clarified API availability: programmatic access is generally available via 2026-04-01, while the Azure portal continues to use 2026-05-01-preview for full features. Retained migration caveats for earlier portal objects to prepare for potential breaking changes.

  https://learn.microsoft.com/en-us/azure/search/get-started-portal-agentic-retrieval

- **Use the Foundry Local CLI (preview)**

  Updated commands and options to align with the current CLI: switched service to server terminology, adjusted list filters to --device and --type, and replaced “foundry model run” with “foundry chat” for interactive sessions. These changes reduce confusion and match the latest tooling behavior.

  https://learn.microsoft.com/en-us/azure/foundry-local/how-to/how-to-use-foundry-local-cli

- **Provenance detection overview**

  Standardized on the “Content Provenance Detection API” name and corrected supported audio details (removing M4A, specifying MP4-audio). Clarified supported media types for consistency with the API.

  https://learn.microsoft.com/en-us/azure/ai-services/content-safety/concepts/provenance-detection

- **Quickstart: Deploy your own code as a hosted agent**

  Raised the minimum azd version to 1.27.1, added azd auth login, and updated troubleshooting to verify the azure.ai.agents extension (1.0.0-beta.4+). Clarified cleanup to differentiate behavior when the environment created the project versus using an existing project.

  https://learn.microsoft.com/en-us/azure/foundry/agents/quickstarts/quickstart-deploy-own-code

- **Quickstart: Add a Foundry IQ knowledge base to a hosted agent with a tool**

  Clarified that azd deploy uploads source as a ZIP for remote dependency resolution and build in Foundry. Updated azd down behavior to preserve existing projects unless the current environment created the project, reducing accidental deletions.

  https://learn.microsoft.com/en-us/azure/foundry/agents/quickstarts/quickstart-foundry-iq-hosted-agent

- **Quickstart: Deploy your first hosted agent**

  Increased the minimum azd requirement to 1.27.1, added azd auth login, and clarified that deployment now packages source for remote build in Foundry. Cleanup and troubleshooting steps were updated to reflect conditional deletion behavior and extension version checks.

  https://learn.microsoft.com/en-us/azure/foundry/agents/quickstarts/quickstart-hosted-agent

- **Quickstart: Give a hosted agent persistent memory**

  Updated deployment to use azd packaging with remote dependency resolution and build in Foundry, replacing container build steps. Clarified azd down behavior so teams understand when project resources are preserved versus deleted.

  https://learn.microsoft.com/en-us/azure/foundry/agents/quickstarts/quickstart-memory-hosted-agent

- **Quickstart: Build a toolbox and use it with a hosted agent**

  Clarified the impact of azd down: it deletes the project only if the current environment created it, otherwise it leaves the project and resources intact. This helps prevent unintended resource removal.

  https://learn.microsoft.com/en-us/azure/foundry/agents/quickstarts/quickstart-toolbox-agent

- **Quickstart: Trace your hosted agent**

  Raised the azd requirement to 1.27.1 for the microsoft.foundry extension and clarified cleanup behavior depending on project creation. Minor wording updates note that this quickstart doesn’t create extra resources.

  https://learn.microsoft.com/en-us/azure/foundry/observability/quickstarts/quickstart-tracing-hosted-agent

- **Upgrade to the latest REST API in Azure AI Search**

  Updated vector search examples to require "search": "*" for vector-only queries, clarifying that the parameter is mandatory but ignored for ranking. This removes ambiguity and aligns samples with actual API behavior.

  https://learn.microsoft.com/en-us/azure/search/search-api-migration

- **Create an Azure AI Search service in the Azure portal**

  Removed the “(preview)” designation from keyless connections when attaching a Microsoft Foundry resource, reflecting general availability. This signals readiness for production scenarios without key-based auth.

  https://learn.microsoft.com/en-us/azure/search/search-create-service-portal

- **Quickstart: Vector search**

  Added a note on supported Azure OpenAI embedding models for vector search and guidance to review GPT-4 family deprecations via the retirement schedules. This helps teams select supported embeddings and plan migrations.

  https://learn.microsoft.com/en-us/azure/search/search-get-started-vector

- **Transcription models from OpenAI**

  Renamed and broadened content from Whisper-only to cover OpenAI transcription models, updating titles, workflows, and comparisons. Clarified offline versus realtime options, capabilities (like diarization), file size limits, and regional availability to guide model and platform choice.

  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/transcribe-overview

- **Best practices and troubleshooting guide for Foundry Local CLI (preview)**

  Updated licensing guidance to emphasize reviewing publisher terms and internal policy compliance, removing CLI-based license retrieval steps. Troubleshooting now references “foundry server” commands, checking server logs, and using “foundry report” for diagnostics to streamline support.

  https://learn.microsoft.com/en-us/azure/foundry-local/reference/reference-best-practice