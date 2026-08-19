# Microsoft Foundry
**Date created:** 2026-08-19 UTC  
**Tags:** Automation, Best Practices, Compliance, Configuration, Get Started, Governance, Guidance, Identity, Licensing, Monitoring, Performance, Security, Troubleshooting  

## Major Changes

- **Manage hosted agent sessions**

  Expanded session management guidance to make idle timeouts configurable per agent version (5–60 minutes, default 15) and to clarify behavior when the timeout is reached. Added a dedicated “Manage session idleness” section with step-by-step instructions to configure idle_timeout_seconds via Python SDK, REST, and Azure Developer CLI, including example snippets. This enables teams to align session lifetime with workload needs and control resource usage.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/manage-hosted-sessions

- **Indexer execution on Serverless and Standard 3 High Density (S3 HD)**

  Increased the daily cumulative indexer runtime quota from 6 hours to 24 hours and clarified that all running indexers draw from a single shared service budget. Added operational guidance on monitoring (Get Indexer Status), handling failures, and the inability to pause/stop active runs, plus a split-and-embed throughput example with caveats. These updates help plan schedules, stagger workloads, and manage skillset costs for more predictable execution.

  https://learn.microsoft.com/en-us/azure/search/search-indexer-high-density-serverless-overview

## Moderate Changes

- **Build a voice agent with hosted agents**

  Updated platform limits to make session idle timeout configurable from 5 to 60 minutes (default 15), with compute deprovisioned at timeout while session state persists. This provides flexibility to right-size resource usage without losing session context.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/build-voice-agent

- **Configure content filters (classic)**

  Added options to switch to annotate-only mode or disable prompt filtering, with approvals required for partial or full filter changes. Control remains limited to managed customers, and new managed enrollment isn’t currently available, helping set expectations for governance and escalation paths.

  https://learn.microsoft.com/en-us/azure/foundry-classic/openai/how-to/content-filters

- **How to create a custom photo avatar**

  Clarified consent requirements: the consent video must include about one minute of audio used to help match voice and avatar. Updated steps cover identity confirmation, script-based verification, face-to-photo checks, and voice-avatar matching, strengthening compliance and authenticity.

  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/text-to-speech-avatar/custom-photo-avatar-create

- **Rate limits, region support, and enterprise features for evaluation**

  Added a “Supported regions for AI red teaming” section, including regions for current and classic experiences, and referenced classic red teaming regions. This helps teams locate appropriate regions and plan evaluations consistently across environments.

  https://learn.microsoft.com/en-us/azure/foundry/concepts/evaluation-regions-limits-virtual-network

- **Hosted agents in Foundry Agent Service**

  Introduced configurable idle timeout per agent version (5–60 minutes), updated references across sections, and clarified scaling behavior (timer resets on requests; compute deprovisioned at timeout; state persists). Reiterated that sessions are permanently deleted after 30 days of inactivity, improving capacity planning and lifecycle clarity.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/hosted-agents

- **Deploy Azure Machine Learning extension on Azure Kubernetes Service (AKS) or Azure Arc-enabled Kubernetes cluster**

  Added a limitation that the Azure ML extension isn’t supported on ARM64 and requires x86_64 (amd64) node pools; provided guidance to use nodeSelector in mixed-architecture clusters. Clarified real-time inference by identifying the router as the “azureml-fe-v2” deployment and where it appears among components, improving deployment reliability.

  https://learn.microsoft.com/en-us/azure/machine-learning/how-to-deploy-kubernetes-extension?view=azureml-api-2

- **Get started with LangChain and LangGraph with Foundry**

  Updated code samples to current APIs, including corrected imports and namespaces, and refined credential guidance (added AzureCliCredential; direct API key usage; AzureCliCredential replacing placeholders). These changes align examples with the latest SDK behavior and reduce setup friction.

  https://learn.microsoft.com/en-us/azure/foundry/how-to/develop/langchain

- **Use Foundry Memory with LangChain and LangGraph**

  Refreshed examples to use current langchain-azure-ai modules, corrected model identifiers (azure_ai:gpt-4.1), and removed deprecated imports. This improves compatibility and helps avoid runtime errors.

  https://learn.microsoft.com/en-us/azure/foundry/how-to/develop/langchain-memory

- **Use LangChain with models in Microsoft Foundry**

  Updated the embeddings example to import and pass DefaultAzureCredential to init_embeddings, noting it doesn’t automatically fall back like init_chat_model. This clarifies authentication patterns and prevents credential-related failures.

  https://learn.microsoft.com/en-us/azure/foundry/how-to/develop/langchain-models

- **Trace LangChain and LangGraph apps with Microsoft Foundry and Azure Monitor**

  Revised configuration to use FOUNDRY_PROJECT_ENDPOINT and set the model to “gpt-4.1,” updated invocation to workflow.invoke, and moved thread_id into the configurable section. These changes align tracing setup with current Foundry configuration practices.

  https://learn.microsoft.com/en-us/azure/foundry/how-to/develop/langchain-traces

- **Manage hosted agents**

  Documented that container idle timeout is configurable from 5 to 60 minutes (default 15) at agent version creation and clarified that compute scaling is separate from endpoint state. This helps tailor cost and performance to workload patterns.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/manage-hosted-agent

- **Built-in policies for model deployment in Microsoft Foundry portal**

  Moved the “Foundry model deployments should meet eligibility requirements” policy from Preview to Generally available. Updated headings, tables, and CLI/portal instructions to match the GA display name, ensuring consistent policy enforcement and discovery.

  https://learn.microsoft.com/en-us/azure/foundry/how-to/model-deployment-policy

- **Azure Content Understanding in Foundry Tools document solutions**

  Added an “Extraction mode” section explaining layout-aware versus text-only extraction and how to choose per scenario (for example, RAG or ingestion). Included guidance on using confidence scores and source grounding to route low-confidence results to human review, improving accuracy and automation.

  https://learn.microsoft.com/en-us/azure/ai-services/content-understanding/document/overview

- **Run or Reset Indexers**

  Expanded quota guidance to cover Serverless and clarified limits: two-hour maximum per indexer run and 24 hours of cumulative runtime per service per 24-hour UTC window. Added details on tracking cumulative runtime via servicestats and refined response property descriptions to aid monitoring and planning.

  https://learn.microsoft.com/en-us/azure/search/search-howto-run-reset-indexers

- **Service limits in Azure AI Search**

  Clarified indexer runtime limits by setting a two-hour maximum per run and adding a new 24-hour cumulative runtime per service per 24-hour window for S3 HD and Serverless. Updated tables and footnotes to consolidate guidance, helping teams plan schedules and monitor usage.

  https://learn.microsoft.com/en-us/azure/search/search-limits-quotas-capacity

- **Customize voice and sound with SSML**

  Added guidance on style marker behavior for HD voices: styles persist across sentences until reset, [Neutral] restores the default, and paragraph/sentence boundaries reset styles (but <break> does not). This clarifies how to control prosody consistently in generated speech.

  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/speech-synthesis-markup-voice

- **Create and manage a toolbox in Foundry**

  Introduced MCP Server–based toolbox management with a catalog of MCP tools (get, version_get, version_create, update, delete) and versioning behaviors. Included example prompts and a link to the Foundry MCP Server reference to streamline automation and governance of tools.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/toolbox

- **How to use the Voice Live API**

  Added photo avatar guidance: standard avatars expect a 512x512 source image; custom photo avatars require a subject photo and about one minute of consent audio. Linked to custom avatar creation docs to clarify prerequisites and workflow.

  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/voice-live-how-to

- **What is custom text to speech avatar?**

  Updated that custom photo avatars can be created directly in the Foundry portal from a single image and used for batch or real-time synthesis. Simplified notes by removing preview licensing language while retaining access and request details.

  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/text-to-speech-avatar/what-is-custom-text-to-speech-avatar

- **What is Text to speech avatar?**

  Replaced VASA-1 references with Microsoft VASA and clarified photo avatar variants: standard (talking head from a single photo) and custom (fine-tuned look). Added a requirement for about one minute of consent audio to improve voice-avatar matching and linked to the custom avatar article.

  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/text-to-speech-avatar/what-is-text-to-speech-avatar

- **What's new in Azure Content Understanding in Foundry Tools?**

  Broadened generative model support to the GPT-5 series (including 5.0, 5.1, 5.2, 5.4, 5.5 and mini/nano where supported). Introduced the extractionMode capability (2025-11-01 GA API) to choose layout-aware or faster text-only extraction, and clarified its separation from confidence/source grounding settings for more precise analyzer control.

  https://learn.microsoft.com/en-us/azure/ai-services/content-understanding/whats-new