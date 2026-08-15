# Microsoft Foundry
**Date created:** 2026-08-15 UTC  
**Tags:** Automation, Configuration, Deprecation, Get Started, Guidance, Troubleshooting  

## Moderate Changes

- **Run evaluations in the cloud by using the Microsoft Foundry SDK**

  Clarified that the model router can only be used as an evaluation target and isn’t supported for synthetic data generation or as a simulator model. Updated parameter descriptions and notes to prevent misconfiguration during evaluations.

  https://learn.microsoft.com/en-us/azure/foundry/how-to/develop/cloud-evaluation

- **Document Intelligence contract model**

  Reworked version applicability using moniker-based sections, adding a v4.0 range, updating v3.1 notes, and marking v3.0 as retiring. This improves clarity on supported versions without changing the model’s behavior.

  https://learn.microsoft.com/en-us/azure/ai-services/document-intelligence/prebuilt/contract?view=doc-intel-4.0.0

- **Document Intelligence general document model**

  Consolidated and broadened version ranges with monikers, removing redundant blocks and expanding feature applicability where appropriate. This streamlines navigation and reduces versioning confusion without altering feature content.

  https://learn.microsoft.com/en-us/azure/ai-services/document-intelligence/prebuilt/general-document?view=doc-intel-4.0.0

- **Use the Foundry Local CLI (preview)**

  Added Homebrew-based installation and upgrade steps for macOS, including guidance to stop the 0.8.x service before upgrading. This simplifies setup and ongoing updates while keeping .pkg/.zip alternatives.

  https://learn.microsoft.com/en-us/azure/foundry-local/how-to/how-to-use-foundry-local-cli

- **Document Intelligence ID document model**

  Scoped the “applies to v4.0” note with a targeted moniker range so it displays only for version 4.0 content. This ensures accurate version-specific guidance.

  https://learn.microsoft.com/en-us/azure/ai-services/document-intelligence/prebuilt/id-document?view=doc-intel-4.0.0

- **Use LangGraph with the Agent Service**

  Expanded prerequisites and environment checks, updated examples (including file search, image generation, and Code Interpreter), and standardized cleanup to avoid orphaned resources. Introduced troubleshooting for common tool execution and deployment issues to accelerate successful runs.

  https://learn.microsoft.com/en-us/azure/foundry/how-to/develop/langchain-agents

- **Foundry Local CLI reference**

  Added Homebrew installation steps and detailed upgrade guidance for macOS (including stopping legacy 0.8.x services), while retaining direct download options. This provides a clearer, faster path to install and maintain the CLI.

  https://learn.microsoft.com/en-us/azure/foundry-local/reference/reference-cli

- **Build a workflow in Microsoft Foundry (Preview)**

  Clarified Logic Apps capabilities by noting deterministic steps can use built-in actions, APIs, and MCP servers, and refined guidance to support incremental enrichment of existing processes. This helps teams adopt workflows without rebuilding from scratch.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/workflow