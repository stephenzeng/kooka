# Microsoft Foundry
**Date created:** 2026-09-03 UTC  
**Tags:** Analytics, Configuration, Deprecation, Guidance, Monitoring, Troubleshooting  

## New Articles

- **Evaluate deployed model and agent conversations with the Microsoft Foundry SDK**
  
  New guidance explains how to evaluate conversations captured in Application Insights using the Microsoft Foundry SDK. It covers two workflows—targeting specific conversation IDs and sampling by agent—along with required/optional parameters, time windows, and lookback limits. The article includes Python and cURL examples, details agent identity formats and filter strategies, and notes ingestion delays and App Insights query constraints. It also links to scripts and follow-on topics for retrieving results, evaluating stored datasets, and simulating conversations.
  
  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/cloud-evaluation-deployed-conversations

- **Simulate conversations with the Microsoft Foundry SDK**
  
  Introduces a preview capability to simulate multi-turn conversations and evaluate agent behavior. The article describes preparing scenario data via JSONL, configuring controls such as num_conversations, max_turns, model, sampling parameters, and data mappings, and defining conversation-level evaluators. Step-by-step Python and cURL examples show how to create evaluations, upload scenarios, run simulations, and configure evaluators. It notes the current absence of JavaScript/TypeScript samples and provides links to related samples and next steps.
  
  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/cloud-evaluation-simulate-conversations

- **Monitor model router in Microsoft Foundry**
  
  Adds a how-to for inspecting per-request routing metadata (preview) for Chat Completions routed through the model router. It shows how to enable the feature with a header, interpret model_selection_details (attempt ordering, latency, HTTP status, and errors), and extract routing and fallback details in code. Guidance explains how to read the serving model, handle cases with no details, and understand variability across attempts and latencies. Links to related model router documentation and samples are included.
  
  https://learn.microsoft.com/en-us/azure/foundry/openai/how-to/monitor-model-router

## Major Changes

- **Evaluate conversation datasets with the Microsoft Foundry SDK**
  
  The article is refocused on evaluating complete conversation datasets rather than production traces. Guidance for evaluating by ID or agent filters in Application Insights was removed and redirected to a new page for deployed conversations. Prerequisites now highlight evaluator examples and updated environment variables (AZURE_AI_PROJECT_ENDPOINT and AZURE_AI_MODEL_DEPLOYMENT_NAME). Testing examples were streamlined to core evaluators such as conversation coherence and groundedness.
  
  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/cloud-evaluation-conversations

- **Evaluate existing datasets with Microsoft Foundry SDK**
  
  The content now emphasizes using the Microsoft Foundry SDK and tightens guidance for small, precomputed datasets. Inline source examples were improved with explicit response fields, and the source support section now clearly maps JSONL/CSV to file_id and file_content options. Examples using the Azure AI builtin.f1_score evaluator were removed, aligning guidance to other evaluators and a dataset-centric framing.
  
  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/cloud-evaluation-datasets

- **Generate synthetic data with the Microsoft Foundry SDK**
  
  The article significantly trims scope by removing the “Simulate conversations (preview)” section and its related examples. It now focuses on generating individual test queries and evaluating model/agent targets. This streamlines guidance and reduces overlap with the new dedicated simulation article.
  
  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/cloud-evaluation-synthetic-data

- **Create and manage prompt flow compute sessions in Microsoft Foundry portal (classic)**
  
  An important notice clarifies that prompt flow container images (including promptflow-runtime) no longer receive updates, and recommends planning a migration to Microsoft Agent Framework. The page’s wording was clarified in the base image section, and “Related resources” was renamed to “Related content.” A migration link was added to help customers move off deprecated images.
  
  https://learn.microsoft.com/en-us/azure/foundry-classic/how-to/create-manage-compute-session

- **Fireworks models on Microsoft Foundry**
  
  The model catalog was expanded with new entries, and availability was updated for some existing models that move to PTU-only. The pay-per-token option is now deprecated for several Fireworks models, with PTU remaining available. These changes help customers plan migrations and choose supported deployment options across a broader set of models.
  
  https://learn.microsoft.com/en-us/azure/foundry/how-to/fireworks/enable-fireworks-models

## Moderate Changes

- **Create a Blob Knowledge Source for Agentic Retrieval**
  
  Added preview guidance for enabling automatic per-language analyzers through a shared include. Azure AI Search can now detect document language and apply the matching analyzer automatically, simplifying configuration and improving multilingual relevance.
  
  https://learn.microsoft.com/en-us/azure/search/agentic-knowledge-source-how-to-blob

- **Create an indexed OneLake knowledge source**
  
  Introduced a preview option to enable automatic per-language analyzers via an include. This reduces manual analyzer selection and helps ensure language-appropriate analysis for OneLake-based knowledge sources.
  
  https://learn.microsoft.com/en-us/azure/search/agentic-knowledge-source-how-to-onelake

- **Create a SharePoint (Indexed) Knowledge Source**
  
  Added guidance to enable automatic per-language analyzers, making it easier to configure language-aware processing for SharePoint (Indexed) content. This streamlines setup and can improve retrieval quality across multilingual datasets.
  
  https://learn.microsoft.com/en-us/azure/search/agentic-knowledge-source-how-to-sharepoint-indexed

- **What is a Knowledge Source?**
  
  The overview now documents preview support for automatic per-language analyzers across Blob, indexed OneLake, and indexed SharePoint sources. With automatic language detection and analyzer selection, authors no longer need to specify analyzers in definitions or queries, reducing setup effort.
  
  https://learn.microsoft.com/en-us/azure/search/agentic-knowledge-source-overview

- **Introduction to cloud evaluation with Microsoft Foundry SDK**
  
  The article was retitled and the “Choose your starting point” section reworked to a three-column format that introduces evaluation units (individual turn vs. complete conversation). Workflows were clarified and expanded, with updated names and links for evaluating datasets, deployed conversations, generating synthetic queries, and simulating conversations.
  
  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/cloud-evaluation

- **Evaluate individual interactions from deployed models and agents with Microsoft Foundry SDK**
  
  Retitled to highlight evaluating individual interactions, and removed a partial-trace safety evaluator example (builtin.violence). This aligns examples with current evaluation patterns.
  
  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/cloud-evaluation-deployed-interactions

- **Evaluate model and agent targets with Microsoft Foundry SDK**
  
  Retitled to emphasize target evaluation and removed the Azure AI task adherence evaluator example. The guidance now reflects the current recommended approach to configuring testing criteria.
  
  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/cloud-evaluation-targets

- **Use model router for Microsoft Foundry**
  
  Clarified that Chat Completions responses include a model field identifying the serving model and documented how to opt in to preview per-request routing metadata, with a pointer to monitoring guidance. Also corrected wording to reference the model router model version and updated the supported regions to include Canada Central, North Europe, Norway East, and UAE North for Global Standard deployments.
  
  https://learn.microsoft.com/en-us/azure/foundry/openai/how-to/model-router

- **Auto and direct model routing with the Responses API**
  
  Replaced the observability bullet with guidance on using response.model to identify the serving model and linked to monitoring for preview routing attempts, status, and latency. This helps teams trace routing decisions and understand fallback behavior.
  
  https://learn.microsoft.com/en-us/azure/foundry/openai/how-to/responses-model-routing