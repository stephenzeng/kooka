# Microsoft 365 Copilot Extensibility
**Date created:** 2026-07-14 UTC  
**Tags:** AI, Agent, Analytics  

## New Articles

- **Evaluators reference for Agent Evaluations CLI (preview)**

  Introduced a comprehensive reference for all evaluators supported by the Microsoft 365 Copilot Agent Evaluations CLI. Covers LLM-based evaluators (such as Relevance, Coherence, Groundedness, and Similarity) with their scoring scales, thresholds, and required fields. Documents retrieval evaluators (RetrievalQuery, RetrievalResult) and string/count-based evaluators (Citations, PartialMatch, ExactMatch) with configuration options and default behaviors. Includes JSON examples, default pass criteria, and links to related configuration guidance and the evaluation dataset schema.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/evaluations-cli-evaluators

## Moderate Changes

- **copilotReportRoot: getMicrosoft365CopilotUsageUserDetail**

  Updated Graph request examples to require the period parameter for both v1.0 and beta endpoints to ensure successful queries. Added a note clarifying that this report is available only in the global cloud, helping admins plan deployments accordingly.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/api/admin-settings/reports/copilotreportroot-getmicrosoft365copilotusageuserdetail

- **copilotReportRoot: getMicrosoft365CopilotUserCountSummary**

  Updated the API examples to include the required period parameter across v1.0 and beta for accurate requests. Added a global-only availability note to set expectations for national cloud tenants.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/api/admin-settings/reports/copilotreportroot-getmicrosoft365copilotusercountsummary

- **copilotReportRoot: getMicrosoft365CopilotUserCountTrend**

  Clarified request syntax by requiring the period query parameter for both v1.0 and beta to align with service behavior. Added a note that this report is available only in the global cloud.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/api/admin-settings/reports/copilotreportroot-getmicrosoft365copilotusercounttrend

- **Declarative agent architecture**

  Clarified how scoped web search grounds responses using Bing-indexed content, noting potential gaps or staleness for dynamically generated or client-rendered pages. Added constraints and guidance for scenarios where reliable recency is required, helping authors choose suitable approaches.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/declarative-agent-architecture

- **Dataset schema and test design**

  Updated references and examples to schema version 1.6.0 and clarified applicability to 1.2.0 or later. Improved guidance on designing multi-turn tests and configuring evaluators to align with the newer schema.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/evaluations-cli-create-tests

- **Agent Evaluations CLI overview (preview)**

  Expanded the metrics with two non-LLM evaluators: RetrievalQuery (pass/fail) and RetrievalResult (proportional scoring). This enables evaluation of retrieval quality without relying on LLMs.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/evaluations-cli-overview

- **Add knowledge sources to your declarative agent**

  Added guidance on “Web search grounding and dynamic content,” explaining that grounding relies on Bing-indexed content and may miss frequently changing or client-rendered pages. Recommends using API plugins with OpenAPI for reliable, up-to-date access to structured data, with links to relevant authoring guidance.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/knowledge-sources