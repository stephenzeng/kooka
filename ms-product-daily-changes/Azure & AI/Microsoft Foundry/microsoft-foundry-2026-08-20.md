# Microsoft Foundry
**Date created:** 2026-08-20 UTC  
**Tags:** Analytics, Automation, Best Practices, Billing, Configuration, Consumption, Deprecation, Get Started, Governance, Guidance, Identity, Monitoring, Security  

## New Articles

- **Add a human-in-the-loop approval step (preview)**

  Introduces a how-to for pausing long-running hosted agents to await human approval and then resuming work without losing progress. Explains the suspend/resume pattern using task IDs and entry modes, with Python examples to initiate approvals and apply decisions. Covers persisting small state in metadata versus storing large artifacts externally, and shows how to clean up suspended chains. Links to resilience, steering, state management, and recovery guidance to help teams design safe review workflows.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/add-human-in-the-loop

- **Agent optimizer cost and token usage overview**

  Explains how the optimizer estimates costs before a run and how to interpret measured token usage afterward. Breaks down the optimization loop into cost layers (agent, judge, reflection), inputs that affect estimates, and pricing assumptions with an example. Clarifies limitations (averages, exclusions, and non-spending-limit estimates) and how to approximate model costs from measured tokens, including cache effects. Helps teams plan budgets up front and reconcile consumption after runs.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/agent-optimizer-costs

- **Deploy a crash-resilient long-running agent (preview)**

  Provides step-by-step guidance to deploy a hosted agent that survives process crashes using resilient background responses. Details prerequisites, enabling resilience and steering options, and running a Python sample locally or in Foundry. Walks through intentionally crashing and observing automatic recovery, stream reconnection, and checkpointed progress. Includes clean-up steps and links to deeper conceptual topics.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/deploy-resilient-agent

- **Deploy a steerable agent (preview)**

  Shows how to deploy a long-running hosted agent that accepts a queued follow-up turn and cooperatively cancels the in‑flight turn. Demonstrates enabling steerable conversations in server options, provisioning with CLI, and exercising the behavior with a sample client. Explains ordering guarantees, avoiding conflicts, and handling full steering queues. Helps teams create responsive agents without breaking sequential conversation history.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/deploy-steerable-agent

- **Long-running agent API reference (preview)**

  Documents resilient task primitives and APIs for Python and C# to build crash‑resilient, long‑running hosted agents. Covers one-shot and multi-turn tasks, retry policies, task status and exceptions, and recovery enablement. Details host options for resilient background work and steerable conversations, plus streaming backends with live and replay capabilities. Includes cross-language code samples and links to related concepts and how‑tos.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/long-running-agent-reference

- **Resilience for long-running Microsoft Foundry hosted agents (preview)**

  Defines the resilience model for hosted agents, distinguishing simple background work from durable, recoverable execution. Describes durable identities, input persistence, lease-based recovery, and strategies for preserving progress with metadata and external storage. Explains streaming replay with cursors, cooperative cancellation, graceful shutdown, and composition with external checkpointers or workflow engines. Provides design boundaries and best practices to reduce rework and side effects after failures.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/long-running-agent-resilience

- **Manage state for long-running agents (preview)**

  Introduces a two-layer state approach: small task metadata for checkpoints and FoundryStateStore for durable bulk data. Explains scopes, flushing, concurrency with ETags, TTL, size limits, tagging, and user isolation. Shows how to back framework checkpointers (LangGraph, MAF) and when to externalize large payloads to blob storage. Helps teams build reliable recovery with minimal duplication or data loss.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/manage-task-state

- **Model migration: upgrade or switch models in Microsoft Foundry**

  Outlines a six‑phase process to move workloads between models: Discover, Assess, Adapt, Validate, Roll out, and Retire. Explains when to migrate, how retirement varies by deployment type, and why to prepare a frozen test set. Provides guidance on replaying workloads, adjusting prompts, tools, schemas, and code, and selecting rollout strategies like canary or side‑by‑side. Highlights Foundry capabilities for optimization, simulation, evaluation, and post‑rollout observability.

  https://learn.microsoft.com/en-us/azure/foundry/foundry-models/concepts/model-migration

- **Recover long-running work after a crash (preview)**

  Explains how to enable crash recovery with resilient background processing and task recovery flags. Details reinvocation behavior, stream replay, and conversation locking, and how to detect recovery on responses and tasks. Provides strategies to resume safely, fence side effects with watermarks, and handle graceful shutdown to keep in‑progress responses recoverable. Includes code samples and links to deeper guidance.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/recover-long-running-work

- **Steer an in-flight agent turn (preview)**

  Introduces steering controls that queue a follow‑up turn and cooperatively cancel the current turn for long‑running hosted agents. Covers enabling steering, queuing follow‑ups with prior response and session IDs, and handler patterns to wind down work. Describes observability fields, ordering guarantees, and error handling for full queues, helping developers deliver responsive agent experiences without race conditions.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/steer-hosted-agent

- **Stream long-running agent output with reconnect (preview)**

  Details reliable streaming for long-running hosted agents with live and replay backends, including file‑backed persistence for restarts. Explains cursor‑based reconnect, producer/subscriber patterns, and lifecycle from active to closed streams. Clarifies snapshot reset semantics and how clients resume after in‑progress events. Provides Python examples to implement robust, resumable streaming.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/stream-with-reconnect

## Major Changes

- **Available tools and example prompts for Foundry MCP Server (preview)**

  Substantially expands and reorganizes the tools reference, growing coverage from 50 tools across 12 categories to 79 across 17 categories. Introduces hosted agent sessions and files, generation and evaluation job orchestration, dataset download via SAS, and unified model deployment retrieval. Updates example workflows, including managed compute quota planning and continuous evaluation, and deprecates older aliases for a cleaner deployment workflow. This upgrade improves discoverability, standardizes operations, and streamlines end‑to‑end scenarios.

  https://learn.microsoft.com/en-us/azure/foundry/mcp/available-tools

- **Manage and optimize Azure Machine Learning costs**

  Adds an important notice that low‑priority VMs were retired on March 31, 2026; affected clusters now use Spot VMs via Azure Batch. Clarifies Spot pricing behavior, eviction model, and the absence of a price cap for Batch Spot nodes, and recommends using the Azure pricing calculator to check current rates. This helps teams re‑evaluate cost assumptions and adjust capacity and reliability planning for training and inference workloads.

  https://learn.microsoft.com/en-us/azure/machine-learning/how-to-manage-optimize-cost?view=azureml-api-2

- **Agents in Microsoft Foundry**

  Rewrites and restructures the overview to clarify how to build with prompt agents, hosted agents, or the Responses API. Introduces new concepts such as Toolboxes, Optimizer, observability enhancements, and ephemeral agents, and links directly to key concepts. Refines positioning of agent types, expands tool guidance including MCP connections and authentication, and updates lifecycle, enterprise capabilities, and navigation links. This makes it easier to choose an approach, assemble the right tools, and get started quickly.

  https://learn.microsoft.com/en-us/azure/foundry/agents/overview

## Moderate Changes

- **Agent optimizer in Foundry Agent Service overview (preview)**

  Adds cost‑awareness guidance for prompt agents with pre‑run estimate review and post‑run token usage analysis. Clarifies evaluation execution semantics and sharpens descriptions of optimization targets. Includes a new reference link to detailed cost estimates and token usage to help teams plan and validate optimization runs.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/agent-optimizer-overview

- **Hosted agent runtime contract**

  Explains long‑running and resilient execution integrations, including durable checkpoints, background processing, and replay behavior. Clarifies that the Invocations adapter lacks a status/polling contract and recommends resilient tasks with defined endpoints for client progress. Provides a pointer to deeper resilience and replay guidance to design reliable client experiences.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/hosted-agent-contract

- **What are hosted agents?**

  Expands guidance on preserving work across interruptions and replaying streamed results. Clarifies when to opt in to background mode, differentiates it from optional resilient recovery, and updates protocol comparisons. Adds a note linking to the resilience article to guide architecture choices for long‑running scenarios.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/hosted-agents

- **Connect agents to Model Context Protocol servers**

  Adds best practices to treat remote MCP tool metadata and results as untrusted input and to review allowed tools and approvals when servers change. Reinforces governance and review processes to reduce indirect prompt injection risk and ensure safe tool usage.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/model-context-protocol

- **Quickstart: Optimize a prompt agent (preview)**

  Clarifies that cost estimates are modeled ranges with explicit pricing assumptions and exclusions. Adds detailed cost breakdowns by phase and explains the Token usage view for post‑run analysis. Helps users plan costs and interpret token metrics accurately.

  https://learn.microsoft.com/en-us/azure/foundry/agents/quickstarts/quickstart-optimize-prompt-agent

- **Supported regions for Azure Speech**

  Updates the feature matrix to reflect new availability in centralus, eastasia, and westcentralus. Ensures readers rely on current regional support when planning deployments.

  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/regions