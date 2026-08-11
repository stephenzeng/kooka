# Microsoft Foundry
**Date created:** 2026-08-02 UTC  
**Tags:** Agent, AI, Monitoring, Security  

## Moderate Changes

- **Custom Web API skill in an Azure AI Search enrichment pipeline**
  Added security guidance emphasizing that custom skill inputs are untrusted and must be validated and constrained before use. Provides concrete practices such as input validation, destination allowlists, URL/hostname and protocol checks, and least-privilege network access, with references to networking architecture options. This helps reduce injection and exfiltration risks when processing document-derived values.
  https://learn.microsoft.com/en-us/azure/search/cognitive-search-custom-skill-web-api

- **Model leaderboards in Microsoft Foundry portal (preview)**
  Streamlined the introduction and clarified benchmarking scope for LLMs/SLMs and embeddings. Updated methodology details, including aggregation windows and rate-limit descriptions, and refined definitions for throughput and first-token latency while removing redundant summary content. These changes make performance comparisons more precise and actionable.
  https://learn.microsoft.com/en-us/azure/foundry/concepts/model-benchmarks

- **Agent tracing overview**
  Retitled the article and aligned multi-agent span naming by changing the child span to agent_orchestration. Added security and privacy guidance that directs sensitive content to a restricted table. This improves trace consistency and helps teams protect confidential data in observability pipelines.
  https://learn.microsoft.com/en-us/azure/foundry/observability/concepts/trace-agent-concept

- **What is Foundry IQ?**
  Added guidance on connecting a Foundry IQ knowledge base to a Microsoft Copilot Studio agent. Explains how grounded retrieval with source attribution brings enterprise knowledge into Copilot Studio and points to configuration steps. This enables richer, traceable responses in Copilot-powered solutions.
  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/what-is-foundry-iq