# Microsoft Agent 365
**Date created:** 2026-08-14 UTC  
**Tags:** Automation, Best Practices, Configuration, Get Started, Governance, Guidance, Identity, Licensing, Monitoring, Security, Troubleshooting  

## New Articles

- **Agent 365 Skills for Guided Agent Setup**

  Introduced Agent 365 Skills, a guided setup that connects existing agents to Agent 365 from coding assistants like GitHub Copilot CLI, Claude Code, and VS Code agent mode. The article explains how Skills run, when to use them, and details seven skills covering setup, provisioning, observability, validation, Work IQ tooling, and local testing. It emphasizes safe, repeatable, and state-aware workflows that replace the prior instructions-based approach, with guidance on when to choose Skills versus manual setup. Links to related quickstart, SDK overview, and validation resources are provided.

  https://learn.microsoft.com/en-us/microsoft-agent-365/developer/agent-365-skills

- **Choose an Agent 365 Integration Option**

  Added a comparison guide for three integration mechanisms: built-in integration, registry sync (preview), and the Agent 365 SDK. It directs readers to prefer built-in or registry sync when sufficient, and to use the SDK for code-level capabilities such as identity, observability, tooling, and notifications. The guide clarifies identity execution modes (S2S, OBO, Agentic-User), notes platform-specific nuances, and includes related links for deeper implementation.

  https://learn.microsoft.com/en-us/microsoft-agent-365/developer/choose-integration-option

- **Agent 365 SDK Validation Checklist**

  Published a comprehensive checklist to validate SDK integrations across identity, observability, tooling, notifications, configuration, and deployment readiness. It covers Entra setup (agent identity, sponsors, user account prerequisites, permissions), telemetry requirements and visibility across Microsoft services, and end-to-end tool and notification flows. The guide provides remediation paths and references to troubleshooting, FAQs, and Skills-based setup to streamline issue resolution.

  https://learn.microsoft.com/en-us/microsoft-agent-365/developer/validation-checklist

## Major Changes

- **Microsoft Agent 365 SDK overview**

  Significantly expanded and reorganized the SDK overview to clarify where the SDK fits, when to use it, and how it complements platform integrations. Added a capability breakdown (Identity, Observability, governed Work IQ tooling, Notifications), selective adoption guidance, and a comparison with the Microsoft 365 Agents SDK. Introduced an onboarding flow (Register, Extend, Validate, Operate), an example request flow, and refined package guidance for Python, JavaScript, and .NET, with curated related links to accelerate adoption.

  https://learn.microsoft.com/en-us/microsoft-agent-365/developer/agent-365-sdk

- **Quickstart: Connect an existing agent to Agent 365**

  Rewrote the content into a procedural quickstart focused on connecting an existing agent using Agent 365 Skills. Added clear prerequisites, skill-based installation, provisioning paths for standard agents and AI teammates, and detailed steps for registration, messaging/notifications, and observability across S2S, OBO, and Agentic-User modes. Expanded setup with Work IQ tools for Microsoft 365 data, local testing via Agents Playground, validation guidance, and a troubleshooting table, while removing prior broad conceptual sections.

  https://learn.microsoft.com/en-us/microsoft-agent-365/developer/get-started

- **Agent 365 identity**

  Overhauled to center on Microsoft Entra Agent ID with a three-object model: blueprint, agent identity, and optional user account. Added credential guidance on configuring secrets, certificates/keys, and federated credentials at the blueprint level, including managed identity federation and governance via Conditional Access. Clarified execution modes (S2S, OBO, Agentic-User) with selection steps, sponsor requirements, audit/sign-in log mapping, pre-onboarding decisions, and updated related links.

  https://learn.microsoft.com/en-us/microsoft-agent-365/developer/identity

## Moderate Changes

- **Agent 365 CLI**

  Updated guidance to reflect that Agent 365 Skills now automate CLI installation, updates, and workflow, replacing prior AI-guided setup references. Adjusted prerequisites to point to the Quickstart and made minor wording edits without changing any CLI commands or behaviors.

  https://learn.microsoft.com/en-us/microsoft-agent-365/developer/agent-365-cli

- **Microsoft Agent 365 SDK and CLI**

  Refreshed the developer landing page quick-start table by replacing “AI-guided setup” with “Agent 365 Skills” and updating references to modern coding assistants (GitHub Copilot CLI, Claude Code, VS Code agent mode). Updated navigation links, including changing “Types of agents” to “Agent identity.”

  https://learn.microsoft.com/en-us/microsoft-agent-365/developer/

- **Why does an enterprise need Agent 365?**

  Enhanced the article with a complex image and extended caption describing Agent 365 as a centralized control plane for enterprise AI agents. The updates emphasize visibility, security, governance, oversight, and lifecycle monitoring to reinforce the case for centralized management at scale.

  https://learn.microsoft.com/en-us/microsoft-agent-365/leadership/why-agent-365-for-enterprise