# Microsoft Foundry
**Date created:** 2026-07-15 UTC  
**Tags:** AI, Agent, Automation, Programming  

## Major Changes

- **What is the agent optimizer? (preview)**

  Expanded the optimizer to automatically improve instructions, skills, tool descriptions, and model selection in a single run, guided by baseline config and eval.yaml. Introduced a clear, step-by-step workflow with links, plus a concise target/activation matrix to show what’s optimized and when. Updated process guidance to highlight cloud execution, typical run times, and that no code changes are needed between runs when using load_config(). Simplified model configuration by requiring explicit eval and optimization models and replacing inline YAML with pointers to dedicated how-to content.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/agent-optimizer-overview

- **Create an evaluation dataset and evaluators (preview)**

  Overhauled guidance for creating evaluation assets by clarifying the roles of datasets and evaluators and detailing the azd workflow that generates seed data, rubric evaluators, and eval.yaml. Added instructions for customizing evaluators, editing rubric dimensions, and versioning via azd ai agent eval update. Simplified dataset design with a clearer schema, options for Foundry-registered or local JSONL sources, and task-level criteria, plus validation steps for local files. Expanded best practices and troubleshooting to improve dataset quality, manage versioning, and resolve reference path issues.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/create-optimizer-dataset

- **Optimize agent instructions, skills, tools, and models (preview)**

  Rewrote and reorganized the optimization guide to clarify targets and streamline execution paths. Added detailed run options (default command, config-driven), agent targeting and priority resolution, and a comprehensive “Configure the optimization run” section with eval.yaml schema and parameters. Introduced guidance for selecting eval/optimization models, evaluating multiple deployments using model_search_space, and monitoring jobs in CLI and portal. Consolidated target-specific content into a concise reference that explains what each target changes and retained practical examples.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/optimize-agent-targets

## Moderate Changes

- **Configure Claude Code for Microsoft Foundry**

  Updated prerequisites and deployment guidance to reference supported regions by deployment type, note broad support for global standard deployments, and remove the “preview” label for Claude models. Revised the VS Code configuration to use an array of name/value objects for environment variables (CLAUDE_CODE_USE_FOUNDRY, ANTHROPIC_FOUNDRY_RESOURCE, ANTHROPIC_FOUNDRY_API_KEY), improving clarity and consistency.

  https://learn.microsoft.com/en-us/azure/foundry/foundry-models/how-to/configure-claude-code

- **Fireworks models on Microsoft Foundry**

  Updated the catalog to remove Pay-per-token availability for DeepSeek V3.2, Moonshot AI Kimi K2.5, OpenAI gpt-oss-120b, and Z.ai GLM-5, making them PTU-only. Added an explicit deprecation notice for the Pay-per-token offering on these models to guide cost and deployment planning.

  https://learn.microsoft.com/en-us/azure/foundry/how-to/fireworks/enable-fireworks-models

- **Make your agent optimizer-ready (preview)**

  Repositioned this article as the starting point for optimization with a clear three-step flow: install the package, configure the baseline, and load the config. Clarified required baseline assets (metadata.yaml, instructions.md) and optional items (tools.json, skills/) that drive which targets are optimized, and streamlined usage by consolidating sections. Redirected apply/deploy steps to a dedicated article and emphasized that external tool calls execute during evaluation for more realistic results.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/make-agent-optimizer-ready

- **Quickstart: Asynchronous document translation**

  Renamed the batch API request option from translateWithinImage to translateTextWithinImage in the example payload to more clearly indicate translating text within images.

  https://learn.microsoft.com/en-us/azure/ai-services/translator/document-translation/latest/quickstarts/asynchronous

- **Start an asynchronous batch translation**

  Updated the API reference parameter name from translateWithinImage to translateTextWithinImage to precisely describe translation of text within images in .docx and .pptx files.

  https://learn.microsoft.com/en-us/azure/ai-services/translator/document-translation/latest/rest-api/translate-asynchronous