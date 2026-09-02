# Microsoft Foundry
**Date created:** 2026-09-02 UTC  
**Tags:** Analytics, Automation, Best Practices, Configuration, Deprecation, Get Started, Guidance, Identity, Monitoring, Performance, Security, Troubleshooting  

## Major Changes

- **Copy a OneLake lakehouse table to Azure Machine Learning through the UI**
  Shifted from linking OneLake tables to a copy-based workflow into Azure Data Lake Storage, then creating an Azure ML datastore over that copy. Added clear setup, role, and authentication guidance, plus a three-step process using Fabric pipelines and studio UI. Included troubleshooting for permissions, key access, and recurring copies, clarifying that the datastore reflects a point-in-time snapshot rather than a live link.
  https://learn.microsoft.com/en-us/azure/machine-learning/create-datastore-with-user-interface?view=azureml-api-2

- **Deploy a hosted agent**
  Introduced an end-to-end JavaScript/TypeScript path for deploying hosted agents, from prerequisites and version creation to routing and invocation via Responses and Invocations protocols. Added polling for activation, examples for cleanup, and security notes for bearer token usage. This expands language coverage and streamlines deployment automation.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/deploy-hosted-agent

- **Deploy a hosted agent from source code**
  Added comprehensive JavaScript/TypeScript guidance to build, upload, and validate source packages for Python or .NET runtimes, including activation polling and Responses-based invocation. Clarified there’s no Node.js hosted runtime and explained SHA-256 verification and post-deployment validation. This enables JS/TS teams to automate source-driven deployments safely.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/deploy-hosted-agent-code

- **Evaluate your AI agents**
  Added full JavaScript/TypeScript coverage for dataset upload, evaluator configuration, evaluation runs, and result retrieval with polling. Provided concrete examples using built-in evaluators and model deployment configuration. These updates make end-to-end evaluation accessible to JS/TS workflows and improve consistency across languages.
  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/evaluate-agent

- **Use Fabric to access model deployment batch endpoints (preview)**
  Marked the article as preview and strengthened guidance on datastore selection, input/output paths, and integrating OneLake with Azure ML. Added step-by-step execution and verification across Azure ML and Fabric, plus troubleshooting for storage, endpoint authorization, and unique outputs. This reduces setup errors and clarifies the end-to-end run experience.
  https://learn.microsoft.com/en-us/azure/machine-learning/how-to-use-batch-fabric?view=azureml-api-2

- **Manage hosted agents**
  Expanded with extensive JavaScript/TypeScript examples for listing, creating, routing, deleting versions, streaming logs, and retrieving managed identity IDs. Clarified current gaps (e.g., enable/disable not yet in JS/TS) and when to use REST/CLI for role assignments. This broadens automation options and improves operational clarity for JS/TS users.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/manage-hosted-agent

- **Manage hosted agent sessions**
  Added JavaScript/TypeScript coverage for session creation, reuse, direct Invocations protocol calls, and session file operations. Noted REST fallback for features not yet in JS/TS (stop session). This enables robust session lifecycle management and file handling from JS/TS clients.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/manage-hosted-sessions

- **Bring your own registry for hosted agents**
  Reworked the guide to use OIDC token exchange for short-lived access to non-Azure registries (e.g., JFrog, Docker Distribution), avoiding stored secrets. Added provider-specific setup, Entra app configuration, networking with/without VNet isolation, and deployment via azd, Bicep, and Python SDK. This delivers a secure, end-to-end path for private registry integration and verification.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/private-registry-connections

- **Quickstart: Evaluate your hosted agent**
  Added a complete JavaScript/TypeScript flow for confirming a deployed agent, creating datasets/evaluators, running evaluations, and collecting results with polling. Updated guidance to reflect multiple available paths and clarified data mapping usage. This accelerates evaluation onboarding for JS/TS developers.
  https://learn.microsoft.com/en-us/azure/foundry/observability/quickstarts/quickstart-evaluate-hosted-agent

- **Add client-side tracing to Foundry agents (preview)**
  Introduced comprehensive JS/TS examples for enabling GenAI tracing with OpenTelemetry and exporting to Azure Monitor or console. Documented environment variables for experimental tracing and content recording and provided setup and shutdown practices. This improves observability, enabling richer diagnostics from client applications.
  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/trace-agent-client-side

- **Understand how OData collection filters work in Azure AI Search**
  Updated guidance to reflect support for correlated filters on collection complex types, while clarifying that full-text search over those collections remains uncorrelated. This helps teams build more precise filters without misinterpreting text search behavior.
  https://learn.microsoft.com/en-us/azure/search/search-query-understand-collection-filters

- **Microsoft Foundry docs: What's new for August 2026**
  Overhauled the monthly update to highlight significant additions across agents, models/APIs, observability, platform capabilities, and responsible AI. Summaries cover long-running agents, private registries, router evaluation, multi-agent orchestration, synthetic data, Entra-authenticated trace ingestion, and more. Provides a consolidated view of broad platform enhancements for the month.
  https://learn.microsoft.com/en-us/azure/foundry/whats-new-foundry

## Moderate Changes

- **Add guardrails to a hosted agent**
  Added JavaScript/TypeScript examples to configure guardrails via the SDK, including package setup and creating a hosted agent version with RAI settings. This simplifies adding policy-based protections in code.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/add-hosted-agent-guardrails

- **Connect to an A2A agent endpoint from Foundry Agent Service (preview)**
  Documented how to attach the A2A tool directly to an agent or through a toolbox, with TypeScript samples and expected output. This enables reuse and direct invocation patterns for agent-to-agent integrations.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/agent-to-agent

- **Connect an Azure AI Search index to Foundry agents**
  Clarified that SDKs can resolve connection IDs by name and added a TypeScript example for retrieving the connection ID. This reduces configuration friction when wiring up search.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/ai-search

- **Reference a path to enriched nodes by using context and source properties in an Azure AI Search skillset**
  Corrected an example annotation from “last” to “lastname,” aligned path references, and clarified zero-based array indexing. Also refined the page title for clarity, improving accuracy for skillset authors.
  https://learn.microsoft.com/en-us/azure/search/cognitive-search-concept-annotations-syntax

- **Tips for AI enrichment in Azure AI Search**
  Clarified how Debug session scopes to a single source document and updated portal-based troubleshooting steps. Added guidance for scheduling frequent indexer runs to resume long image processing. These changes enhance diagnostic effectiveness.
  https://learn.microsoft.com/en-us/azure/search/cognitive-search-concept-troubleshooting

- **Configure and share your agent**
  Added JS/TS examples for setting up endpoints, enabling protocols and auth schemes, and creating an agent card with skills/examples. This streamlines end-to-end configuration from code.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/configure-agent

- **Enable incoming A2A on a Foundry agent (preview)**
  Added JS/TS setup and a TypeScript sample to enable the A2A protocol and define an agent card. This makes it easier to programmatically open A2A endpoints.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/enable-agent-to-agent-endpoint

- **Generate a synthetic evaluation dataset (preview)**
  Introduced JS/TS examples for creating and managing generation jobs with the SDK, plus notes on current limitations. This expands dataset generation options for JS/TS users.
  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/evaluation-dataset-synthetic

- **Customize a model with fine-tuning**
  Added a JavaScript pivot with Foundry SDK usage for fine-tuning. This broadens language coverage for customizing models.
  https://learn.microsoft.com/en-us/azure/foundry/openai/how-to/fine-tuning

- **Create and run component-based ML pipelines (CLI)**
  Updated CLI instructions, added a command to check job status, and corrected a YAML expression reference. These changes reduce errors and improve pipeline operations clarity.
  https://learn.microsoft.com/en-us/azure/machine-learning/how-to-create-component-pipelines-cli?view=azureml-api-2

- **Custom tool package creation and usage**
  Added prerequisites, clarified compute session setup and package installation, and improved VS Code extension guidance. This helps teams set up Prompt flow custom tools more reliably.
  https://learn.microsoft.com/en-us/azure/machine-learning/prompt-flow/how-to-custom-tool-package-creation-and-usage?view=azureml-api-2

- **Use Azure Machine Learning studio to debug pipeline failures**
  Added a prerequisites section outlining workspace access and failed jobs needed for debugging. This sets expectations for successful troubleshooting.
  https://learn.microsoft.com/en-us/azure/machine-learning/how-to-debug-pipeline-failure?view=azureml-api-2

- **Monitor agents with the Agent Monitoring Dashboard**
  Added JS/TS instructions for setup, creating versions, and creating continuous evaluation rules, plus listing runs and retrieving reports. This enables monitoring workflows in JS/TS environments.
  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/how-to-monitor-agents-dashboard

- **Hybrid search using vectors and full-text search in Azure AI Search**
  Updated request parameters to use vectorQueries and corrected filter property naming. This aligns examples with current API conventions and avoids misconfiguration.
  https://learn.microsoft.com/en-us/azure/search/hybrid-search-overview

- **Isolate hosted agent sessions per user**
  Added JS/TS examples for session scoping using caller Entra identity or the x-ms-user-identity header. This clarifies how to ensure per-user isolation and auditability.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/isolate-sessions-per-user

- **Create a Knowledge Store Using REST**
  Clarified table projection requirements and refined status verification using indexer status and expected 200 responses. This improves correctness and reduces confusion during setup.
  https://learn.microsoft.com/en-us/azure/search/knowledge-store-create-rest

- **Connect agents to Model Context Protocol servers**
  Removed “preview” references for Azure DevOps MCP, explained hosted endpoint behavior, and clarified Entra ID authentication requirements. This sets clear expectations for setup and support boundaries.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/model-context-protocol

- **Use model router with Foundry agents**
  Added JS/TS samples alongside Python for creating agents and configuring router usage, with API references. This helps teams adopt router patterns in multiple languages.
  https://learn.microsoft.com/en-us/azure/foundry/openai/how-to/model-router-agents

- **Auto and direct model routing with the Responses API**
  Added JS/TS examples and setup steps to call multiple deployments via the Responses API, with language-specific installation guidance. This makes model routing patterns easier to adopt across stacks.
  https://learn.microsoft.com/en-us/azure/foundry/openai/how-to/responses-model-routing

- **Run AI Red Teaming Agent in the cloud**
  Added JS/TS and cURL tabs covering environment setup, creating and running red teams with evaluators and attack strategies, polling, and exporting results. This expands access to security testing workflows beyond Python.
  https://learn.microsoft.com/en-us/azure/foundry/how-to/develop/run-ai-red-teaming-cloud

- **Upgrade to Azure AI Search .NET SDK version 11**
  Corrected API/client mappings and clarified responsibilities across versions, with guidance to prefer the current stable SDK. This reduces migration errors and aligns implementations with modern patterns.
  https://learn.microsoft.com/en-us/azure/search/search-dotnet-sdk-migration-version-11

- **Azure Table Indexer**
  Updated managed identity guidance to use the Storage Table Data Reader role instead of Reader and Data Access. This ensures correct permissions for Entra-based connections.
  https://learn.microsoft.com/en-us/azure/search/search-how-to-index-azure-tables

- **Azure Cosmos DB Gremlin Indexer**
  Corrected configuration examples, JSON syntax, and connection strings (ApiKind=Gremlin), and aligned schema samples. These fixes prevent misconfigurations and improve reliability.
  https://learn.microsoft.com/en-us/azure/search/search-how-to-index-cosmosdb-gremlin

- **Indexing with Azure Cosmos DB for MongoDB**
  Fixed JSON examples, removed unused properties, standardized ApiKind casing, and corrected configuration keys. This improves example validity and reduces setup issues.
  https://learn.microsoft.com/en-us/azure/search/search-how-to-index-cosmosdb-mongodb

- **Azure SQL Indexer**
  Updated T-SQL defaults, removed unsupported container.query, and clarified indexer parameter payloads and soft-delete configuration with precise JSON. This improves performance tuning and correctness.
  https://learn.microsoft.com/en-us/azure/search/search-how-to-index-sql-database

- **Query Types**
  Clarified hybrid search behavior, corrected geospatial field type guidance, and fixed Lucene wildcard/prefix operators. These changes enhance query accuracy and developer understanding.
  https://learn.microsoft.com/en-us/azure/search/search-query-overview

- **Customize agent behavior at runtime with structured inputs**
  Added TS examples showing MCP configuration, passing structured inputs via Responses, and using advanced Handlebars templates. This enables more dynamic and maintainable agent instruction patterns.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/structured-inputs

- **How toolbox authentication works in Microsoft Foundry**
  Added JS/TS examples and version requirements for SDKs, plus configuration examples using OAuth identity passthrough. This helps standardize secure tool authentication in multi-language environments.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/tool-authentication

- **Enable tool search in a toolbox**
  Expanded JS guidance with concrete code for discovering, pinning, and validating tools, including wildcard pinning and additional search text. This improves toolbox governance and discoverability.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/tool-search

- **Convert agent traces into evaluation datasets (preview)**
  Added JS/TS guidance for job management (list, cancel, delete) and SDK setup, with notes on current limitations. This streamlines dataset creation from traces in JS/TS workflows.
  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/traces-to-dataset

- **Tutorial: Create a custom analyzer for phone numbers**
  Updated analyzer configuration and corrected names and index references, including tokenizer adjustments and field naming consistency. This ensures the tutorial aligns with working configurations.
  https://learn.microsoft.com/en-us/azure/search/tutorial-create-custom-analyzer

- **Tutorial: Index from multiple data sources using the .NET SDK**
  Modernized the C# sample to use IndexerClient.RunIndexerAsync and RequestFailedException handling. This aligns with current SDK best practices and error handling patterns.
  https://learn.microsoft.com/en-us/azure/search/tutorial-multiple-data-sources

- **Tutorial: Optimize indexing using the push API**
  Modernized C# examples for payload sizing, async usage, and response handling, and fixed minor code issues. This improves performance guidance and sample correctness.
  https://learn.microsoft.com/en-us/azure/search/tutorial-optimize-indexing-push-api

- **Web search tool**
  Added domain-restricted Bing Custom Search setup with streaming and citation extraction, plus deep research using o3-deep-research with direct web_search tool. Clarified costs, terms, and compliance boundaries outside code samples. These additions offer practical patterns for targeted and exploratory retrieval.
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/web-search