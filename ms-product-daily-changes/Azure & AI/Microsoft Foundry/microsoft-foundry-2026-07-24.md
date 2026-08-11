# Microsoft Foundry
**Date created:** 2026-07-24 UTC  
**Tags:** Administration, AI, Agent, Programming, Security  

## New Articles

- **Configure language identification and diarization for speech transcription**

  Introduced a unified guide for configuring language identification and speaker diarization across real-time, translation, fast, and batch transcription scenarios. Provides best practices for constraining candidate locales and handling short or noisy audio. Includes SDK and REST examples for real-time and offline workflows with clear parameters for enabling diarization and specifying maximum speakers. Adds a preflight checklist to validate settings before running jobs.

  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/configure-language-identification-diarization

- **What is the Foundry Agent Canvas?**

  Introduces the Foundry Agent Canvas, a GitHub Copilot App extension that lets you design, configure, test, and deploy hosted agents from a side panel. Explains how the canvas scaffolds and edits agent code while staying in sync with your project resources (models, toolboxes, skills, guardrails). Details end-to-end workflows, sign-in and project selection, local testing via Agent Inspector, and deployment to the Foundry Agent Service. Provides installation options and notes underlying azd command usage with links to related articles.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/foundry-agent-canvas

- **Fast transcription containers - Speech service**

  Adds a how-to for running the Fast Transcription Speech container on-premises with Docker, including image locations, versioning, and broad locale/model support. Covers prerequisites and GPU-only requirements, pull/run commands, and parameters for connected and disconnected modes. Documents the REST API for synchronous file transcription with examples for dual-channel audio, diarization, and profanity filtering. Explains response schemas and environment variables for tuning performance and licensing.

  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/speech-container-ft

- **Use tool search with the Azure OpenAI Responses API**

  Introduces tool search for the Responses API and shows how to defer tool definitions to reduce context size and preserve prompt caching. Explains when to centralize tool definitions and how this improves performance and cost. Provides core guidance via shared content for consistent implementation.

  https://learn.microsoft.com/en-us/azure/foundry/openai/how-to/tool-search

## Major Changes

- **What is MAI-Voice (preview)?**

  Overhauled the documentation to focus on MAI-Voice-2 and the new MAI-Voice-2-Flash, removing MAI-Voice-1 content. Highlights low-latency, real-time synthesis with MAI-Voice-2-Flash and high-fidelity, long-form strengths with MAI-Voice-2, along with expanded multilingual support and SSML emotion/style control. Adds gated instant voice cloning guidance, new SSML examples, and a Python sample using the Azure Speech SDK to synthesize SSML to MP3. Expands custom voice guidance and provides a comprehensive prebuilt voices table for MAI-Voice-2-Flash.

  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/mai-voices

- **Quickstart: Deploy your first hosted agent**

  Added a new canvas-based path that walks you through building and deploying a hosted agent using the Foundry Agent Canvas in the GitHub Copilot App. The update covers connecting a Foundry project, scaffolding the agent, configuring models/toolboxes/skills/guardrails, and testing locally with integrated azd run and Agent Inspector. It then guides you through deployment to the Foundry Agent Service and cleanup steps, with cross-references to related concepts.

  https://learn.microsoft.com/en-us/azure/foundry/agents/quickstarts/quickstart-hosted-agent

## Moderate Changes

- **Create a File Knowledge Source for Agentic Retrieval**

  Clarified private networking prerequisites: when public access is disabled, create and approve an openai_account shared private link from Azure AI Search and keep trusted services bypass enabled. Expanded troubleshooting for model access and upload failures, including the 403 Public access is disabled error and common causes like unsupported file types and quotas, to reduce setup friction and speed resolution.

  https://learn.microsoft.com/en-us/azure/search/agentic-knowledge-source-how-to-file

- **Work with chat completion models**

  Strengthened setup and usage guidance for Azure OpenAI chat completions in Python and .NET, including resource prerequisites, model deployment, Azure Identity usage, role assignments, and az login steps. Clarified how to replace resource and deployment placeholders in samples and added related links to the Responses API, available models, and embeddings for deeper exploration.

  https://learn.microsoft.com/en-us/azure/foundry/openai/how-to/chatgpt

- **Configure environment variables for a hosted agent**

  Added new environment variables—FOUNDRY_HOSTING_ENVIRONMENT and FOUNDRY_AGENT_ID—to help agents detect hosting context and identify the running agent. Updated azd service configuration examples to use the environmentVariables key for more accurate deployment configuration.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/configure-hosted-agent-env-variables

- **Foundry Agent Service limits, quotas, and regional support**

  Updated the regional availability matrix: removed File Search support in Brazil South and Italy North, and enabled Code Interpreter in South Central US and Spain Central. Adjusted the guidance to reflect these changes so teams can plan deployments and capabilities by region with confidence.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/limits-quotas-regions