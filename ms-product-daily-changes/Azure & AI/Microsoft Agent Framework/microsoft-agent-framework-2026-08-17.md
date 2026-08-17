# Microsoft Agent Framework
**Date created:** 2026-08-17 UTC  
**Tags:** Best Practices, Configuration, Get Started, Governance, Guidance, Identity, Security  

## New Articles

- **Agent hooks**

  Introduced Agent Hooks, a governance capability that intercepts agent inputs, model/tool calls, and outputs using a framework-neutral AGENT-HOOKS-0.1 contract. The article outlines enforcement guarantees such as fail-closed behavior, buffered streaming, transform write-back, and verdict-gated persistence, and explains verdict types (allow, deny, escalate, transform). It covers Python availability (experimental), installation via the agent-hooks extra, and how to configure interceptors, composition, identity, and timeouts. Guidance includes evaluate-only rollout, placement alongside middleware, interactions with tool approval, session/audit recording, and current limitations.

  https://learn.microsoft.com/en-us/agent-framework/agents/agent-hooks

## Major Changes

- **Backend Tool Rendering with AG-UI**

  Simplified and refocused guidance to clarify that AG-UI uses the standard Agent Framework tool pipeline and emits transport events for client observation—removing any separate tool abstraction. Added a minimal C# sample, guidance to share JsonSerializerOptions for complex types, and an AG-UI event mapping that connects FunctionCallContent and FunctionResultContent to TOOL_CALL_* and TOOL_CALL_RESULT. Included a streamlined .NET client snippet for observing calls/results and links to backend tools samples and general function tool guidance. These changes reduce setup overhead and make tool observability and integration clearer.

  https://learn.microsoft.com/en-us/agent-framework/integrations/by-component/ui/ag-ui/backend-tool-rendering

- **Frontend Tool Rendering with AG-UI**

  Rewrote the tutorial around a concise, end-to-end C# flow for declaring, registering, and executing frontend tools with AGUIChatClient. Added a step-by-step view of client continuation and highlighted security guidance for handling untrusted client input with proper authorization and validation. Linked to shared function tool guidance and next steps for human approval. The result is a practical, code-first guide that accelerates implementation while improving safety.

  https://learn.microsoft.com/en-us/agent-framework/integrations/by-component/ui/ag-ui/frontend-tools

- **Getting Started with AG-UI**

  Reworked the getting-started flow to focus on hosting a preconfigured agent and exposing it via MapAGUIServer, removing extensive Azure setup steps. Added a streamlined .NET client example using AGUIChatClient with streaming, and clarified server-sent events behavior and how to run the server. Introduced conversation continuity, explaining threadId/parentRunId semantics with sample continuation code, and linked to session persistence and security considerations. The new guidance shortens setup time and clarifies how to build reliable, resumable chat experiences.

  https://learn.microsoft.com/en-us/agent-framework/integrations/by-component/ui/ag-ui/getting-started

- **Human-in-the-Loop with AG-UI**

  Streamlined the approval tutorial to show how MAF controls approval decisions while AG-UI transports requests and responses. Added concise C# server and .NET client examples for requesting approval (via ApprovalRequiredAIFunction), handling ToolApprovalRequestContent, and resuming sessions after a decision. Removed lengthy setup content and linked to centralized tool-approval guidance and state management for next steps. This improves clarity on implementing safe tool execution with human oversight.

  https://learn.microsoft.com/en-us/agent-framework/integrations/by-component/ui/ag-ui/human-in-the-loop

- **Self-host Agent Framework applications**

  Replaced a placeholder with a full .NET self-hosting guide covering prerelease packages, hosting helpers (AddAIAgent, AddWorkflow, IHostedAgentBuilder, AgentSessionStore), and their scope relative to protocol servers. Documented hosted session persistence, durability tradeoffs, and how this differs from history providers, along with ASP.NET Core integration responsibilities. Added protocol integrations (OpenAI-compatible endpoints, A2A, AG-UI), continuation ID considerations, and secure session continuation using claims-based isolation. This provides a complete blueprint for building secure, durable, self-hosted agent services.

  https://learn.microsoft.com/en-us/agent-framework/hosting/self-hosting/

- **State Management with AG-UI**

  Reworked content into clear concepts for exposing client-visible JSON state and .NET options to manage it. Added patterns for reading client state from RunAgentInput, emitting snapshots and deltas via AGUIStreamOptions (MapResultAsStateSnapshot/MapResultAsStateDelta), mapping tool calls to state events, and consuming StateSnapshotEvent/StateDeltaEvent in a client. Clarified JsonElement requirements and that state mapping is opt-in. This helps teams design predictable, observable state flows without heavy boilerplate.

  https://learn.microsoft.com/en-us/agent-framework/integrations/by-component/ui/ag-ui/state-management

## Moderate Changes

- **Executors**

  Added C# guidance for declaring protocol message and output types using [SendsMessage] and [YieldsOutput], including examples and the requirement for partial classes when using the workflows source generator. Documented handler-scoped declarations via [MessageHandler] and clarified default behaviors that auto-send or auto-yield handler results, plus the need to register outputs with WorkflowBuilder.WithOutputFrom. This makes executor protocols explicit and reduces boilerplate.

  https://learn.microsoft.com/en-us/agent-framework/concepts/workflows/executors

- **AG-UI Integration with Agent Framework**

  Reorganized the AG-UI integration overview to emphasize scenarios, .NET capabilities (SSE streaming, tool events, approvals, state exchange, session resume, workflows), and simplified architecture and setup. Also updated the broader capabilities catalog by adding an Agent Hooks entry that describes fail-closed governance via a shared interception contract. Together, these updates clarify how to integrate AG-UI and highlight new governance options.

  https://learn.microsoft.com/en-us/agent-framework/integrations/by-component/ui/ag-ui/

- **MCP Apps Compatibility with AG-UI**

  Replaced placeholders with direct guidance noting that MCP Apps-specific behavior is not provided by MAF and is supplied by external middleware. Directed readers to their chosen AG-UI client or middleware documentation for setup and compatibility. This sets accurate expectations and accelerates correct configuration.

  https://learn.microsoft.com/en-us/agent-framework/integrations/by-component/ui/ag-ui/mcp-apps

- **Security Considerations for AG-UI**

  Expanded authentication and authorization guidance for AG-UI endpoints and clarified that authorization must be implemented by the host. Advised treating client-supplied threadId as untrusted, requiring authorization before resuming sessions, and scoping persisted data by user, tenant, or workspace. Renamed “Session ID management” to “Thread ID management” to align with current practices.

  https://learn.microsoft.com/en-us/agent-framework/integrations/by-component/ui/ag-ui/security-considerations

- **Session**

  Added guidance on hosted session persistence using AgentSessionStore to load/save sessions by continuation ID during request processing. Clarified differences from manual persistence and history providers and updated the capability matrix accordingly. This helps teams choose the right durability model for their workloads.

  https://learn.microsoft.com/en-us/agent-framework/concepts/agents/conversations/session

- **Testing with AG-UI Dojo**

  Added concrete C# guidance explaining that Dojo is an interoperability tool and requires no MAF-specific .NET configuration. Instructed readers to expose their scenario via MapAGUIServer, then connect from Dojo, with links to backend tools, frontend tools, human approval, and state management. This makes scenario testing straightforward.

  https://learn.microsoft.com/en-us/agent-framework/integrations/by-component/ui/ag-ui/testing-with-dojo

- **Workflows with AG-UI**

  Simplified the .NET path to expose a workflow by wrapping it as an AIAgent and mapping it with AG-UI, removing lengthy setup steps. Clarified that .NET streams text and tool-call outputs with AuthorName but currently lacks lifecycle events and interrupt/resume over AG-UI (unlike Python), with a link to the tracking issue. This sets clear expectations and points to security next steps.

  https://learn.microsoft.com/en-us/agent-framework/integrations/by-component/ui/ag-ui/workflows