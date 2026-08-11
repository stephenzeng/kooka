# Microsoft Foundry
**Date created:** 2026-07-31 UTC  
**Tags:** Administration, Agent, AI, Automation, Governance, Monitoring, Programming, Security  

## Major Changes

- **Add guardrails to a hosted agent**

  Expanded guidance from content safety-only controls to comprehensive guardrails, introducing preview network egress controls for outbound traffic governance. Clarified rule evaluation order, default allow/deny behavior, and enforcement modes (Audit vs Enforce), plus documented account-wide limits. Added REST API instructions (2026-05-15-preview) for configuring egressPolicy with Allow/Deny/Transform/Rewrite actions and header transformations, alongside portal-based setup. Included HTTPS certificate handling details and Application Insights queries to review egress decisions, with notes on blocked-request behavior and preview limitations.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/add-hosted-agent-guardrails

- **GenAI Prompt skill**

  Added in-depth security guidance for managed identity authentication, explaining token acquisition for the Foundry Tools audience and supported endpoint domains (Azure OpenAI and Foundry), including APIM/custom domains with live validation. Highlighted token exposure risks and recommended least-privilege roles, network restrictions (NSP/private endpoints/VNet), validation of gateways, and preferring managed identity over API keys. Advised restricting access to skillset configuration due to control over uri and authentication parameters and encouraged ongoing monitoring and reviews.

  https://learn.microsoft.com/en-us/azure/search/cognitive-search-skill-genai-prompt

- **Quickstart: Custom categories (standard mode) (preview)**

  Announced retirement of Custom categories (standard) on September 1, 2026, and directed users to migrate to the Foundry Custom text classification API. This ensures continuity on a supported path and aligns solutions with the long-term platform roadmap.

  https://learn.microsoft.com/en-us/azure/ai-services/content-safety/quickstart-custom-categories

- **Quickstart: Optimize a hosted agent (preview)**

  Expanded the quickstart to cover optimization via Azure Developer CLI, Python SDK, Visual Studio Code (Foundry Toolkit with GitHub Copilot agent mode), and the Microsoft Foundry Skill. Added detailed end-to-end workflows to select workspaces, start optimization runs, compare candidates, and deploy the best option, with new prerequisites and updated Python SDK usage. Clarified template import outputs and interactive initialization, and added troubleshooting for VS Code visibility, Copilot setup, workspace/service alignment, and gated review/apply steps.

  https://learn.microsoft.com/en-us/azure/foundry/agents/quickstarts/quickstart-optimize-hosted-agent

- **Foundry Local CLI reference**

  Reworked terminology and commands from “service” to “server/daemon,” adding an overview of command groups and a top-level command summary. Introduced new Server commands (start/stop/restart/status/logs) and options like --port and --idle-timeout, with examples for fixed-port operation and endpoint verification. Updated quick verification, Open WebUI connection, and troubleshooting to align with the new “foundry server” workflow, reducing setup friction and improving discoverability.

  https://learn.microsoft.com/en-us/azure/foundry-local/reference/reference-cli

- **Azure OpenAI vectorizer**

  Added comprehensive security considerations for managed identity authentication, detailing token use for the Foundry Tools audience and supported endpoints (openai.azure.com, cognitiveservices.azure.com, services.ai.azure.com) with APIM support and live validation. Emphasized the risks of sending tokens to untrusted endpoints and recommended least-privilege roles, network restrictions, and regular reviews and monitoring. Advised limiting who can create or modify index/vectorizer configurations to reduce attack surface.

  https://learn.microsoft.com/en-us/azure/search/vector-search-vectorizer-azure-open-ai

## Moderate Changes

- **Add a custom skill to an Azure AI Search enrichment pipeline**

  Clarified managed identity authentication requirements so that uri must target the same application endpoint identified by authResourceId. Explained how mismatches can cause authentication failures or unintended routing, and added verification steps and security considerations to prevent misconfiguration.

  https://learn.microsoft.com/en-us/azure/search/cognitive-search-custom-skill-interface

- **Custom Web API skill in an Azure AI Search enrichment pipeline**

  Expanded managed identity documentation with a new section on selecting the correct authResourceId (audience/Application ID URI), accepted formats, and examples. Allowed newer API versions (2023-10-01-preview or later) and added security best practices, plus clearer parameter descriptions to reduce common configuration errors.

  https://learn.microsoft.com/en-us/azure/search/cognitive-search-custom-skill-web-api

- **Configure environment variables for a hosted agent**

  Added FOUNDRY_HOSTING_ENVIRONMENT to the injected variables, set to 1 when running in Foundry. This enables code paths to detect Foundry-hosted execution versus local runs and adjust behavior accordingly.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/configure-hosted-agent-env-variables

- **Custom categories (preview)**

  Added an important retirement notice for Custom categories (standard) effective September 1, 2026, and advised migration to the Foundry Custom text classification API. This helps teams plan transitions and avoid service disruptions.

  https://learn.microsoft.com/en-us/azure/ai-services/content-safety/concepts/custom-categories

- **Agent development lifecycle**

  Introduced a stable get-or-create pattern for agents, recommending caching the agent ID, treating 404 as terminal, and performing get-or-create on startup. Clarified that deleted agent IDs are invalid, guiding developers to recreate agents instead of retrying the same ID.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/development-lifecycle

- **GPT Realtime Transcribe overview**

  Updated terminology from “Whisper” to “Transcribe,” aligning the heading and labels with the current feature name. This reflects a product rebrand without changing underlying functionality.

  https://learn.microsoft.com/en-us/azure/foundry/openai/concepts/gpt-realtime-whisper

- **Guardrails and controls overview in Microsoft Foundry**

  Introduced preview network egress controls for hosted agents, enabling teams to restrict outbound connections to approved destinations. Linked to authoring guidance so administrators can define and enforce egress policies within the same guardrail.

  https://learn.microsoft.com/en-us/azure/foundry/guardrails/guardrails-overview

- **Foundry Agent Service limits, quotas, and regional support**

  Clarified agent version limits and updated the error description to “Too many valid agent versions,” noting it is terminal. Advised deleting older versions before creating new ones and avoiding retries until capacity is available, with a new best practice for version lifecycle management.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/limits-quotas-regions

- **Use skills in Foundry (preview)**

  Streamlined risk guidance by replacing a lengthy caution with a concise statement emphasizing customer responsibility to understand external skill behavior and data handling. This keeps the focus on due diligence when integrating third-party endpoints.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/skills

- **Transparency note for Azure OpenAI**

  Updated terminology to replace “Whisper” with the “transcription model” across capabilities, key terms, use cases, API notes, and quality-of-service guidance. Aligned language to consistently describe speech recognition and translation features and availability through Azure Speech services.

  https://learn.microsoft.com/en-us/azure/foundry/responsible-ai/openai/transparency-note

- **Add declarative agent workflows in Visual Studio Code**

  Updated portal navigation to open a workflow by first selecting Agents and then the Workflows tab on the Agents page. This reflects the current UI flow and reduces confusion when launching workflows in VS Code for the Web.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/vs-code-agents-workflow-low-code