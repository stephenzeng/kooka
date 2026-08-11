# Microsoft Foundry
**Date created:** 2026-07-25 UTC  
**Tags:** Agent, AI, Monitoring, Programming, Security  

## Major Changes

- **Query a knowledge base using the retrieve action or MCP endpoint**

  Updated guidance on integrating Azure AI Search knowledge bases with MCP-compatible clients through the Azure OpenAI Responses API. Clarified authentication by introducing a dedicated “Authenticate to the MCP endpoint” section with recommended bearer token flow and admin key alternative, including required roles and headers. Added complete C# and Python samples to configure MCP tools, inject Authorization/api-key headers, and invoke the knowledge_base_retrieve tool, reducing setup errors and accelerating implementation.

  https://learn.microsoft.com/en-us/azure/search/agentic-retrieval-how-to-retrieve

- **Evaluate your AI agents**

  Made rubric evaluators the primary evaluation method, with end-to-end examples for generating rubrics from agent context and combining them with built-in quality and safety evaluators. Updated setup to newer SDKs and environment variables, refined evaluator configuration, and added options to bootstrap datasets from synthetic data or traces. Clarified scoring and sample outputs to make results more interpretable and actionable, helping teams standardize and scale agent evaluation.

  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/evaluate-agent

## Moderate Changes

- **Index content from SharePoint in Microsoft 365 (preview)**

  Streamlined Entra ID setup by clarifying app registration, selecting Application vs. Delegated Microsoft Graph permissions, and granting tenant-wide admin consent. Updated authentication steps to use a Redirect URI for desktop apps and enable public client flows, and clarified ACL ingestion requirements to avoid permission-related indexing failures.

  https://learn.microsoft.com/en-us/azure/search/search-how-to-index-sharepoint-online

- **Convert agent traces into evaluation datasets (preview)**

  Clarified prerequisites by requiring the project’s managed identity to have Log Analytics Reader on the linked Application Insights workspace, and Privileged Monitoring Data Reader for protected trace tables. This ensures trace queries succeed when converting telemetry into evaluation datasets.

  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/traces-to-dataset