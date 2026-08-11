# Microsoft Foundry
**Date created:** 2026-08-11 UTC  
**Tags:** Best Practices, Billing, Compliance, Configuration, Consumption, Deprecation, Get Started, Governance, Guidance, Performance, Security, Troubleshooting  

## New Articles

- **Use Content Understanding with the Microsoft Agent Framework**

  Introduced a how-to for using Content Understanding as a context provider in the Microsoft Agent Framework to process user file attachments. Covers prerequisites, Python package install, and async usage to add Markdown and extracted fields into model context. Explains configuration (endpoint, credentials, analyzer selection, output sections, max wait) and optional file search for RAG, with supported file types and next steps.

  https://learn.microsoft.com/en-us/azure/ai-services/content-understanding/integrations/agent-framework

- **Quickstart: Analyze a document with agentic mode**

  Added a quickstart for enabling agentic mode with API version 2026-06-01-preview. Provides a sample analyzer schema, model deployment setup, and cURL steps to create, run, and retrieve results, including workflow resolution details and cleanup. Highlights advanced contextualization rates and links to preview limitations.

  https://learn.microsoft.com/en-us/azure/ai-services/content-understanding/quickstart/agentic-mode

- **Agentic mode overview for document analysis (preview)**

  Introduced a concept article describing agentic mode for complex documents with multistep reasoning, calculations, validation, visual analysis, and structured outputs. Documents enabling config.workflow="agentic", workflow resolution behavior, and preview limits (single-file requests). Provides cost/latency considerations, migration guidance from retired pro mode, and links to reference and quickstart materials.

  https://learn.microsoft.com/en-us/azure/ai-services/content-understanding/concepts/agentic-mode

- **Use Content Understanding with LangChain**

  Added a how-to for the AzureAIContentUnderstandingLoader to bring documents, images, audio, and video into LangChain. Details installation, automatic analyzer selection, async usage, extracting fields with confidence, and controlling outputs (markdown, page, segment) and content ranges. Includes model deployment mapping examples and supported file types.

  https://learn.microsoft.com/en-us/azure/ai-services/content-understanding/integrations/langchain

- **Use Content Understanding with MarkItDown**

  Published guidance to use Content Understanding as a backend for MarkItDown across modalities. Covers install and CLI/Python usage with automatic analyzer selection, structured field extraction serialized as YAML front matter, and routing behavior for incompatible file types. Provides tips to manage cost by limiting routed file types and links to related resources.

  https://learn.microsoft.com/en-us/azure/ai-services/content-understanding/integrations/markitdown

- **Quickstart: Use synchronous Content Understanding operations**

  Added a quickstart for synchronous REST operations that return immediate results without polling. Targets prebuilt-read and prebuilt-layout analyzers with step-by-step instructions and pointers to document format and size limits.

  https://learn.microsoft.com/en-us/azure/ai-services/content-understanding/quickstart/use-synchronous-rest-api

## Major Changes

- **Validate document analyzer quality with confidence, grounding, and labeled samples**

  Expanded and reorganized training guidance to use labeled sample documents with evaluation best practices and clarified scope (document analyzers only). Explained that confidence and grounding apply across extract, classify, and generate methods in GA and preview APIs. Added preview training improvements that distill patterns to reduce runtime tokens and avoid retaining labeled documents, with privacy/storage notes and clearer grounding rationale and OCR limitations.

  https://learn.microsoft.com/en-us/azure/ai-services/content-understanding/document/analyzer-improvement

- **What is a Content Understanding analyzer?**

  Introduced agentic workflow selection with request/response behavior, performance impact, and preview support, plus a resolution table for standard, advanced, and agentic. Expanded estimateSourceAndConfidence support and clarified extract requirements, added automatic normalization for typed fields, and standardized method naming from generative to generate. Removed disableFaceBlurring options and updated cross-references.

  https://learn.microsoft.com/en-us/azure/ai-services/content-understanding/concepts/analyzer-reference

- **Classify and route your data using Content Understanding**

  Extended the how-to with SDK workflows alongside Studio and REST, with multilingual samples for Python, C#, JavaScript/TypeScript, and Java. Added preview sub-page segmentation with configuration, response shape, and routing to sub-analyzers, plus model updates and improved organization of Studio and programmatic paths.

  https://learn.microsoft.com/en-us/azure/ai-services/content-understanding/how-to/classification-content-understanding-studio

- **Content Understanding classification/segmentation**

  Documented preview classification enhancements including layout-based features (no config) and in-page segmentation with a new allowInPageSegments setting for custom analyzers. Added segment output details (page ranges, category, confidence, source polygon) and API fields reference, and clarified hierarchical routing via analyzerId. Noted default page-boundary segmentation and preview availability of in-page segments.

  https://learn.microsoft.com/en-us/azure/ai-services/content-understanding/concepts/classifier

- **Configure language identification and diarization for speech transcription**

  Clarified differences across real-time, fast, and batch transcription and provided a comparison for language identification and speaker labeling. Updated locale guidance, added robust recommendations for candidate lists and fallbacks, and introduced a detailed C# example for auto-detection. Expanded diarization guidance, added cautions and constraints, and improved a preflight checklist to avoid common configuration issues.

  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/configure-language-identification-diarization

- **Data, privacy, and security for Content Understanding**

  Added a section comparing how labeled training data is handled across GA and preview APIs, noting preview distills information without retaining documents for analysis. Clarified authentication options, expanded TLS 1.2/1.3 requirements, and refined result retrieval and Face data handling descriptions. Core privacy principles remain unchanged aside from these clarifications.

  https://learn.microsoft.com/en-us/azure/foundry/responsible-ai/content-understanding/data-privacy

- **Document analysis: Extract structured content**

  Extended the document elements model with a new Signatures element and Document metadata object, updating the top-level JSON and navigation accordingly. Added detailed sections with examples for signatures (including id, source, span, and elements) and extracted metadata (preview), plus a table of metadata keys by file type. This enables downstream workflows to detect signatures and leverage embedded metadata.

  https://learn.microsoft.com/en-us/azure/ai-services/content-understanding/document/elements

- **Connect a Foundry IQ knowledge base to Foundry Agent Service**

  Clarified that hub-based projects aren't supported and added a conditional role assignment for Azure AI Search’s managed identity when an LLM is used. Updated project resource IDs to Microsoft.CognitiveServices/accounts and aligned code samples. Consolidated role assignment guidance for Search roles to simplify setup.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/foundry-iq-connect

- **Content Understanding Studio and Microsoft Foundry**

  Rewrote the comparison to focus on key feature differences, including added coverage for the latest preview API. Introduced a “Choose an experience” section with workflow guidance and clarified analyzer availability by API version. Added a deprecation notice for Foundry (classic) and removed outdated content and notices.

  https://learn.microsoft.com/en-us/azure/ai-services/content-understanding/foundry-vs-content-understanding-studio

- **Azure Content Understanding in Foundry Tools region and language support**

  Removed the entire 2025-05-01-preview section, including managed capacity details, region table, and Pro mode processing location notes. This streamlines the page to reflect current GA and newer preview guidance.

  https://learn.microsoft.com/en-us/azure/ai-services/content-understanding/language-region-support

- **Document analysis: Markdown representation**

  Clarified alt text behavior for figures with no detected text to ensure proper rendering. Added a Signatures section describing how signatures are represented as Markdown images, availability in preview, and accuracy considerations, including examples for recognized and unrecognized text and handling of region-linked signatures.

  https://learn.microsoft.com/en-us/azure/ai-services/content-understanding/document/markdown

- **Azure Content Understanding in Foundry Tools document solutions**

  Added signature detection and document metadata extraction capabilities for supported file types, and replaced a use case with an insurance policy analysis scenario. Clarified that confidence and grounding apply across all field types and methods and reiterated opt-in flags. Noted automatic normalization of typed fields and introduced agentic mode (preview) with one-file-per-request constraints.

  https://learn.microsoft.com/en-us/azure/ai-services/content-understanding/document/overview

- **What is Azure Content Understanding in Foundry Tools?**

  Added a capabilities-by-API-version section with a comparison table and guidance on when to use GA vs. preview, plus a link to What's new. Updated portals content to reflect the Microsoft Foundry portal. Removed Face-related capabilities and associated biometric guidance to align with current scope.

  https://learn.microsoft.com/en-us/azure/ai-services/content-understanding/overview

- **Azure Content Understanding in Foundry Tools video solutions**

  Removed all face description and identification references, including configuration details and biometric guidance. This reflects the deprecation/removal of face-related features from the video solution docs.

  https://learn.microsoft.com/en-us/azure/ai-services/content-understanding/video/overview

- **Prebuilt analyzers in Azure Content Understanding in Foundry Tools**

  Overhauled content with versioned metadata behavior, enhanced prebuilt-layout (signatures, preview), and expanded RAG analyzer outputs with semantic chunking options. Restructured domain categories, added new analyzers (e.g., procurement, Schedule K‑1 forms, MN M1, call center), and clarified composed routing and pricing links to aid selection and integration.

  https://learn.microsoft.com/en-us/azure/ai-services/content-understanding/concepts/prebuilt-analyzers

- **Pricing for Azure Content Understanding in Foundry Tools**

  Substantially revised pricing guidance for GA and preview, including workflow resolution, contextualization tiers, and detailed usage fields. Added rules for custom analyzer billing, model family impacts, and comprehensive tables for prebuilt analyzers. Updated estimation approach to rely on current pricing pages and expanded FAQs with modern model references.

  https://learn.microsoft.com/en-us/azure/ai-services/content-understanding/pricing-explainer

- **Azure Content Understanding in Foundry Tools service quotas and limits**

  Expanded supported Chat Completion models (GPT‑5.x and additional GPT‑4o variants) and overhauled input limits, separating async vs. sync constraints. Greatly broadened supported file types and clarified sync behavior (first five pages by default) and page-equivalence rules. Removed Pro mode notes and corrected audio section markers.

  https://learn.microsoft.com/en-us/azure/ai-services/content-understanding/service-limits

- **What's new in Azure Content Understanding in Foundry Tools?**

  Added July 2026 updates covering agentic mode (preview), synchronous Read/Layout (preview), improved training with labeled samples, confidence/grounding across fields, automatic normalization, and new integrations (Agent Framework, LangChain, Logic Apps, MarkItDown). Introduced signature detection, document metadata extraction, classification enhancements, Azure AI Search skill updates, and expanded GPT‑5.x support. Removed legacy Pro mode and Face-related content and marked Foundry classic as retired.

  https://learn.microsoft.com/en-us/azure/ai-services/content-understanding/whats-new

- **AudioVisual analysis: extracting structured content**

  Consolidated updates removing a Face configuration requirement note while also reflecting expanded document model coverage for signatures and document metadata. Together, these changes simplify setup where Face prerequisites previously applied and improve downstream analysis by adding signatures and embedded metadata outputs.

  https://learn.microsoft.com/en-us/azure/ai-services/content-understanding/video/elements

## Moderate Changes

- **Best practices for Azure Content Understanding in Foundry Tools**

  Added guidance on improving Azure AI Search retrieval by extracting hierarchical sections, tables (including cross-page), figures with AI-generated descriptions, and Markdown content. Expanded training recommendations to cover varied layouts and before/after evaluation, with links to analyzer training improvements.

  https://learn.microsoft.com/en-us/azure/ai-services/content-understanding/concepts/best-practices

- **Azure Content Understanding skill**

  Noted that AI-based descriptions are generated for images, charts, diagrams, and embedded figures and embedded into Markdown for retrieval. These descriptions are searchable and can improve RAG grounding and multimodal retrieval quality.

  https://learn.microsoft.com/en-us/azure/search/cognitive-search-skill-content-understanding

- **Quickstart: Try Content Understanding Studio or Microsoft Foundry**

  Reworked to cover both Studio and Foundry, with tabbed prerequisites and updated flows for prebuilt analyzers and a Foundry playground. Clarified analyzer availability differences and refreshed the custom analyzer creation section with new screenshots.

  https://learn.microsoft.com/en-us/azure/ai-services/content-understanding/quickstart/content-understanding-studio

- **Use the Foundry Local CLI (preview)**

  Updated macOS install to use Apple Silicon installers instead of Homebrew and renamed the tab to “macOS Apple Silicon.” Adjusted instructions and wording across the article for clarity.

  https://learn.microsoft.com/en-us/azure/foundry-local/how-to/how-to-use-foundry-local-cli

- **Migrate from Azure Content Understanding Preview to GA**

  Generalized references to retired preview APIs and removed outdated notes about unchanged confidence/grounding behavior. Simplified deprecations to focus on TrainingData being replaced by knowledgeSources and removed obsolete Pro mode and Face bullets.

  https://learn.microsoft.com/en-us/azure/ai-services/content-understanding/how-to/migration-preview-to-ga

- **Built-in policies for model deployment in Microsoft Foundry portal**

  Updated governance guidance by renaming the eligibility policy to “should meet eligibility requirements (preview)” and detailing how to discover preview policies in CLI and Portal. Clarified catalog behavior and how block reasons are shown when multiple policies apply.

  https://learn.microsoft.com/en-us/azure/foundry/how-to/model-deployment-policy

- **Model deployment options for Content Understanding analyzers**

  Clarified API versioning in examples, refined supportedModels guidance, and updated default model mappings to gpt-5.2. Explained omitting modelDeployments when resource defaults exist and corrected usage property naming.

  https://learn.microsoft.com/en-us/azure/ai-services/content-understanding/concepts/models-deployments

- **Foundry Local CLI reference**

  Revised install/upgrade steps (Apple Silicon installers; clarified Windows commands), standardized server/daemon terminology, and enhanced model listing options with device/task filters, limits, and verbosity. Added server log options, expanded cache controls, and updated troubleshooting for status and restart flows.

  https://learn.microsoft.com/en-us/azure/foundry-local/reference/reference-cli

- **Azure Content Understanding in Foundry Tools image solutions**

  Removed the Face description fields section and associated guidance and links to align with current GA scope. No other content changes were made.

  https://learn.microsoft.com/en-us/azure/ai-services/content-understanding/image/overview

- **AudioVisual analysis: extracting structured content**

  Removed a note requiring enableFace in analyzer configuration and limited access registration, indicating updated prerequisites for using Face features.

  https://learn.microsoft.com/en-us/azure/ai-services/content-understanding/video/elements