# Microsoft Foundry
**Date created:** 2026-07-29 UTC  
**Tags:** AI, Agent, Governance, Programming, Security  

## Major Changes

- **Configure Blob Storage for Azure OpenAI Batch (classic)**

  Rewrote the article into an end-to-end workflow with clearer prerequisites and a new workflow overview. Added parallel setup paths using Azure CLI and Azure portal to enable system-assigned managed identity and assign required Storage Blob Data Contributor roles. Provided Python-based steps to create containers, prepare and upload JSONL, submit and monitor a batch with Entra ID auth, and download results. Clarified key limitations (no user-assigned identity, no metadata support, modifying input during execution fails jobs) and removed the older REST curl example.

  https://learn.microsoft.com/en-us/azure/foundry-classic/openai/how-to/batch-blob-storage

- **Microsoft Foundry Playgrounds (classic)**

  Updated the Images playground model lineup by adding gpt-image-2 and expanding Black Forest Labs options to include FLUX.2-pro and FLUX.2-flex, while removing Stability AI models. Refreshed highlights and examples to compare gpt-image models with FLUX variants for clearer selection. These changes guide users toward currently supported models and more relevant comparisons for image generation workflows.

  https://learn.microsoft.com/en-us/azure/foundry-classic/concepts/concept-playgrounds

- **Microsoft Foundry Models overview**

  Replaced the full article body with a shared include to centralize guidance on model categories, deployment, billing, safety, networking, and lifecycle. This consolidation simplifies maintenance and keeps guidance consistent across pages. No new features were introduced; the content is reorganized for easier reuse.

  https://learn.microsoft.com/en-us/azure/foundry/concepts/foundry-models-overview

- **Connect Using Azure Roles**

  Significantly expanded RBAC guidance for Azure AI Search with step-by-step role assignment instructions across Portal, CLI, PowerShell, and REST. Added per-index and service-level scoping procedures, tips on identifying the correct assignee, and comprehensive testing examples across SDKs using token-based auth. Included end-to-end custom role creation with JSON definitions, assignable scopes, and required actions, plus clarified limitations such as indexer behavior.

  https://learn.microsoft.com/en-us/azure/search/search-security-rbac

- **Fast transcription containers with Docker (preview)**

  Marked the feature as preview and recommended mono PCM WAV 16-bit at 48 kHz for best performance. Added practical ffmpeg examples to convert MP3, M4A/AAC, and OPUS to the preferred format, with flag guidance. Introduced a robust troubleshooting section covering end-of-speech delays, fragmented results, and unsupported media errors, along with corrective steps.

  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/speech-container-ft

- **Enable tool search in a toolbox**

  Announced general availability by renaming the directive and type from toolbox_search_preview to toolbox_search across docs, APIs, and SDKs. Documented how search ranks tools (BM25), what metadata is indexed, and clarified defaults and limits (for example, limit defaults to 5, max 10). Explained why tools are hidden from initial listings and how discovery works, updated all SDK samples to the new type, and aligned troubleshooting and headers with current behavior.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/tool-search

## Moderate Changes

- **How to configure network isolation for Microsoft Foundry**

  Updated firewall allowlisting guidance: revised column naming to “FQDNs / ServiceTags,” refreshed entries for evaluations and traces (including blob storage and Application Insights), and removed outdated endpoints and service tags. Added a new row for Hosted Agents to Agent365 observability/tracing via AzureFrontDoor.Frontend on TCP 443.

  https://learn.microsoft.com/en-us/azure/foundry/how-to/configure-private-link

- **Data, privacy, and security for Document Intelligence**

  Clarified that input data and analyze results are retained for 24 hours and then automatically deleted. Documented that the Delete Analyze Result API can permanently remove both submitted input and results earlier across all models.

  https://learn.microsoft.com/en-us/azure/foundry/responsible-ai/document-intelligence/data-privacy-security

- **Tutorial: Get started with a DeepSeek reasoning model in Foundry Models**

  Generalized the tutorial from DeepSeek-R1 to DeepSeek reasoning models, with concrete guidance centered on DeepSeek-V4-Pro for selection and deployment. Updated examples, deployment options, and rate limits references to reflect the broader model family and current availability.

  https://learn.microsoft.com/en-us/azure/foundry/foundry-models/tutorials/get-started-deepseek-r1

- **Language and voice support for Azure Speech**

  Expanded Speech to text coverage to include post-stream refinement alongside real-time, fast, and batch transcription. Clarified table entries for monolingual (GA) versus multilingual (public preview) post-stream refinement support.

  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/language-support

- **Supported regions for Azure Speech**

  Split the single post-stream refinement column into separate monolingual and multilingual (preview) columns. Updated region checkmarks to reflect current availability per refinement type while leaving other feature listings intact.

  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/regions

- **API Versions**

  Updated SDK references to newer major versions across .NET, Java, JavaScript, and Python and standardized changelog labeling. Improved migration guidance in deprecated and discontinued sections to steer users to current APIs and SDKs.

  https://learn.microsoft.com/en-us/azure/search/search-api-versions

- **What is speech translation?**

  Reorganized the overview into a unified real-time speech translation model supporting text, audio, or both. Elevated and expanded Live Interpreter capabilities such as unspecified input language, dynamic language switching, bring-your-own voice, and target-language-only transcription to clarify scenarios like travel and meetings.

  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/speech-translation

- **Create, test, and deploy a toolbox in Foundry**

  Updated examples to reflect GA naming for Tool Search by replacing toolbox_search_preview with toolbox_search across REST, SDKs, YAML, and CLI. Clarified naming in SDK classes and notes, and explained that toolbox_search is a configuration directive not listed by tools/list.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/toolbox

- **Manage compliance and security in Microsoft Foundry**

  Removed the preview label and updated Microsoft Purview integration to general availability. Clarified that, when enabled by an admin, AI interaction data from all applications and agents in the subscription flows to Purview for centralized compliance, governance, and data security policy enforcement.

  https://learn.microsoft.com/en-us/azure/foundry/control-plane/how-to-manage-compliance-security