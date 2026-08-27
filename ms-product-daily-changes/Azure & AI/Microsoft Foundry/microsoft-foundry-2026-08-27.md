# Microsoft Foundry
**Date created:** 2026-08-27 UTC  
**Tags:** Analytics, Best Practices, Billing, Compliance, Configuration, Deprecation, Get Started, Governance, Guidance, Identity, Licensing, Monitoring, Security, Troubleshooting  

## New Articles

- **Autopilot lifecycle in Microsoft Foundry**

  Introduced a comprehensive concept that maps the full autopilot lifecycle across blueprint, instance, and fleet layers. Defined stages from provision and publish through approve/consent, hire, onboard, operate, and retire/delete, with clear role responsibilities across admins, developers, and tenant approvers. Clarified approval vs. consent, access vs. consent gates, and audience/listening/messaging scopes, plus irreversible actions. Included lifecycle tables, role comparisons, deployment patterns, and related links.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/autopilot-lifecycle

- **What is an autopilot in Microsoft Foundry?**

  Introduced autopilots as agents with both an agent identity and an agent user account, enabling them to act independently across Microsoft 365 surfaces. Clarified how identity—not capabilities—defines autopilots and distinguished them from other agent types. Explained the blueprint model that creates per-team instances for scoped access and governance, and outlined group, company-wide, and personal autopilot types with links to lifecycle and integration content.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/autopilot-overview

- **Run cloud evaluations with the Microsoft Foundry SDK**

  Added a how-to for running cloud evaluations using the Foundry SDK, including prerequisites, regional considerations, and client setup. Explained the evaluation workflow—defining data shape and evaluators, creating evaluations, and monitoring runs—with results stored in the Foundry project and optionally routed to Application Insights. Mapped common starting scenarios (datasets, models/agents, deployed interactions, conversations, synthetic data) to concrete workflows and linked to related docs and APIs.

  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/cloud-evaluation

- **Evaluate conversations with the Microsoft Foundry SDK**

  Provided guidance on conversation-level and turn-level evaluation using the evaluation_level parameter and compatible evaluators. Covered preparing JSONL conversations and running evaluations from datasets, inline data, Application Insights traces, or sampled production traffic with random or smart filtering. Documented parameters for trace lookups and agent filtering, common errors, ingestion delays, 7‑day limits, and paths to retrieve results.

  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/cloud-evaluation-conversations

- **Evaluate datasets with the Microsoft Foundry SDK**

  Explained how to evaluate JSONL and CSV datasets stored in the project or provided inline, including schema mapping to evaluator parameters. Included Python and cURL examples for configuring built-in evaluators (such as coherence, violence, f1_score) and creating evaluations and runs. Linked to runnable samples and guidance for retrieving results.

  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/cloud-evaluation-datasets

- **Evaluate deployed interactions with the Microsoft Foundry SDK**

  Detailed how to evaluate deployed agent and model interactions by stored response IDs or Application Insights traces. Introduced intelligent sampling based on MinHash farthest‑first selection to improve trace diversity and explained when to use it. Specified OpenTelemetry GenAI requirements, necessary roles and data access, and workflows for targeting agents or specific traces, with evaluator setup and data mappings.

  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/cloud-evaluation-deployed-interactions

- **Get cloud evaluation results with the Microsoft Foundry SDK**

  Added guidance for polling evaluation runs, retrieving item-level and aggregate outputs, and canceling jobs. Documented the result schema (label, score, threshold, reason, details) with sample payloads. Included troubleshooting for capacity delays, authentication and schema errors, HTTP 400/429 conditions, and evaluator/tool support considerations.

  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/cloud-evaluation-results

- **Generate synthetic data with the Microsoft Foundry SDK**

  Introduced workflows for generating synthetic evaluation data and simulated conversations to accelerate testing. Described required parameters, evaluator setup, and data mappings, with end‑to‑end examples for models and agents in Python and cURL. Added a preview conversation simulation flow and links to fetch results and runnable samples.

  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/cloud-evaluation-synthetic-data

- **Evaluate models and agents with the Microsoft Foundry SDK**

  Explained how to run cloud evaluations against deployed models, prompt agents, and hosted agents using the azure_ai_target_completions data source. Showed how to define input_templates, configure evaluators (coherence, violence, task adherence), and target models or agents, including the model router as an evaluation-only option. Provided examples for invocations‑protocol agents and linked to related topics and samples.

  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/cloud-evaluation-targets

- **Microsoft Foundry reasoning models**

  Added a how-to for using reasoning models via the OpenAI Chat Completions API with Foundry project endpoints. Covered Entra ID authentication and multi-language examples for basic chat, reading reasoning_content, and streaming. Provided parameter guidance for reasoning models, safety handling, and best practices with links to related Azure OpenAI resources.

  https://learn.microsoft.com/en-us/azure/foundry/foundry-models/how-to/use-chat-reasoning

- **Deploy and use Grok models in Microsoft Foundry**

  Introduced deployment and usage of Grok models (including Grok 4.6) for advanced reasoning, coding, and agentic workflows. Outlined interactions via Chat Completions and Responses APIs and highlighted long‑context support. Most detailed usage content is delivered through shared includes for consistency.

  https://learn.microsoft.com/en-us/azure/foundry/foundry-models/how-to/use-foundry-models-grok

## Major Changes

- **Quickstart: Build your first autopilot**

  Reworked the content from a publish-focused how‑to into an end‑to‑end quickstart that takes users from setup to a working autopilot in Teams. Added prerequisite details (Frontier enrollment, licensing seats, roles), tooling requirements, and regional guidance. Consolidated provision/build/publish flows with Azure CLI/Azure Developer CLI, expanded hosted agent blueprint steps, and introduced comprehensive Microsoft 365 publishing with API examples and versioning notes. Included admin approval walkthroughs, outcomes, licensing propagation, cleanup steps, and significantly expanded troubleshooting to accelerate successful deployments.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/agent-365

- **Microsoft Agent 365 integration with Foundry**

  Clarified registry synchronization and substantially updated concepts for autopilots, including identity model, blueprints, and cross‑Microsoft 365 usage. Updated the supported agent types matrix to indicate Prompt agents are no longer publishable as autopilots and aligned telemetry naming for hosted agents. These changes help teams select the right agent type and understand integration boundaries.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/agent-365-integration

- **Endpoints for Microsoft Foundry Models (classic)**

  Streamlined the page by removing extensive in‑page explanations and examples for the Azure AI inference endpoint, routing behavior, and limitations. The content now relies on shared includes for authoritative guidance, reducing duplication and easing maintenance. This improves consistency and keeps details aligned across related docs.

  https://learn.microsoft.com/en-us/azure/foundry-classic/foundry-models/concepts/endpoints

- **Optimize agent instructions, skills, tools, and models in Foundry Agent Service.**

  Overhauled targeting guidance by replacing a priority list with a context‑based matrix covering azd and non‑azd scenarios and configuration precedence. Added a new path to optimize an existing hosted agent without azd project files, including endpoint discovery, authentication, eval.yaml changes, and standalone limitations. Clarified when apply or direct deploy requires an azd environment and expanded troubleshooting for missing endpoint, agent name, operation ID, and standalone instruction requirements to reduce setup friction.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/optimize-agent-targets

- **Supported regions for Azure Speech**

  Revamped the Voice Live regions table with new columns for gpt‑realtime‑datazone and gpt‑realtime‑1.5‑datazone and updated availability across major models. Clarified that datazone variants use Data Zone Standard deployments with processing contained within the resource’s data zone. These changes help customers plan compliant, region‑appropriate deployments.

  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/regions

- **Azure AI Search regions list**

  Overhauled regional capability tables globally and introduced a dedicated Serverless column with reordered feature columns. Updated capability indicators across regions and revised confidential computing support to list specific regions. Follow‑up refinements adjusted footnotes for high‑demand constraints, added Serverless and Query rewrite for Italy North, and updated Norway East and UAE North for Agentic retrieval/Serverless and related notes. Together, these updates give a more accurate, feature‑complete view of regional availability.

  https://learn.microsoft.com/en-us/azure/search/search-region-support

## Moderate Changes

- **Set the Foundry project context for azd commands**

  Clarified which azd ai agent commands require a local azd project versus those that can run standalone. Documented how optimize can target a deployed agent by name when the project endpoint is resolved via global config, flags, or environment variables, and reiterated using --agent-endpoint with invoke for calls without local project files.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/cli-project-context

- **Data and privacy for Face**

  Inserted a Biometric data privacy note beneath the existing disclosure note to strengthen guidance on handling biometric data for Foundry Tools Face scenarios. This addition consolidates privacy messaging and improves compliance clarity.

  https://learn.microsoft.com/en-us/azure/foundry/responsible-ai/face/data-privacy-security

- **Disclosure for voice and avatar talent**

  Replaced inlined biometric data responsibility text with a reusable Biometric data privacy note include. Centralizing this guidance improves consistency and maintainability without changing policy intent.

  https://learn.microsoft.com/en-us/azure/foundry/responsible-ai/speech-service/text-to-speech/disclosure-voice-talent

- **Guidance for integration and responsible use of Face**

  Added a Biometric data privacy note include to enhance privacy guidance for biometric scenarios. This aligns Face documentation with centralized compliance messaging.

  https://learn.microsoft.com/en-us/azure/foundry/responsible-ai/face/guidance-integration-responsible-use

- **Limited Access**

  Inserted a Biometric data privacy note include for Text to Speech limited access, highlighting privacy considerations for voice talent verification and custom voice usage. This strengthens compliance guidance for sensitive biometric workflows.

  https://learn.microsoft.com/en-us/azure/foundry/responsible-ai/speech-service/text-to-speech/limited-access

- **Migrate from the Foundry (classic) portal**

  Updated the retirement date for the azure-ai-inference package from May 30, 2026 to August 26, 2026 in key callouts and the SDK mapping table. The change provides a more accurate migration timeline and wording.

  https://learn.microsoft.com/en-us/azure/foundry/how-to/navigate-from-classic

- **Role-based access control for Microsoft Foundry**

  Added an IMPORTANT note that the Azure portal currently supports assigning Foundry Agent Consumer only at the account scope and recommends Azure CLI for least‑privilege assignments at project or agent scope. Provided new CLI examples using scope variables and explicit principal parameters to reduce misconfiguration and improve governance.

  https://learn.microsoft.com/en-us/azure/foundry/concepts/rbac-foundry

- **Use cases for Speech to text**

  Added a Biometric data privacy note include to the Speech to text transparency guidance. This reinforces consistent, centralized privacy/compliance information for biometric data handling.

  https://learn.microsoft.com/en-us/azure/foundry/responsible-ai/speech-service/speech-to-text/transparency-note

- **Voice Live API for real-time voice agents**

  Added new Data Zone variants (gpt‑realtime‑datazone and gpt‑realtime‑1.5‑datazone) to the supported models list with data residency notes and Azure TTS support. Removed gpt‑5.2‑chat and gpt‑5.1‑chat entries and updated Voice Live pro pricing to include the new variants.

  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/voice-live

## Minor Changes