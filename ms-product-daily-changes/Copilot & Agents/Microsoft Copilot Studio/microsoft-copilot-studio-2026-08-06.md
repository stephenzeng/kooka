# Microsoft Copilot Studio
**Date created:** 2026-08-06 UTC  
**Tags:** Agent, AI, Analytics, Monitoring  

## Moderate Changes

- **Environment-level telemetry with Application Insights (preview)**

  Clarified that during rollout, root agent invocations (invoke_agent) are emitted as dependencies rather than requests, improving trace interpretation in Application Insights. Recommended evaluating this preview in a non-production environment with the Early release cycle enabled. Removed outdated guidance about reconstructing multi-agent traces using sub-agent details.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/advanced-environment-level-agent-telemetry

- **Use code interpreter in a prompt to generate and execute Python code**

  Expanded guidance by adding Excel semantic search examples to the code interpreter, enabling prompts to retrieve and work with spreadsheet data more effectively. This helps authors build richer, data-aware workflows directly within prompts.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/code-interpreter-for-prompts

- **Use code interpreter to analyze structured data (preview)**

  Added Excel semantic search guidance to structured data scenarios, showing how the code interpreter can semantically locate and analyze spreadsheet content. This streamlines data analysis tasks and improves accuracy when working with Excel data.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/knowledge-code-interpreter-structured-data

- **Knowledge sources summary**

  Introduced Excel semantic search guidance within the Tenant graph grounding with semantic search section, expanding options for finding and grounding knowledge from spreadsheets. This helps improve relevance and coverage for knowledge retrieval scenarios.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/knowledge-copilot-studio

- **Change the model version and settings**

  Added a new section clarifying that model context windows apply per call and that a single interaction may involve multiple calls (planner, retrieval, generation, and tool summarization). Explained that total tokens per turn are the sum across calls and can exceed an individual model’s context window without errors, since no cross-call token cap is enforced. Clarified that context window settings govern how history is trimmed or compacted.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/prompt-model-settings