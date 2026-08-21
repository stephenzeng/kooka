# Microsoft Agent 365
**Date created:** 2026-08-21 UTC  
**Tags:** Automation, Best Practices, Compliance, Governance, Guidance, Identity, Monitoring, Security  

## New Articles

- **How do enterprises know which agents are risky?**

  Added guidance on how Agent 365 identifies and prioritizes risky AI agents using signals from Microsoft Entra (identity), Microsoft Purview (data access), and Microsoft Defender (runtime behavior). Clarifies the consolidated exposure view in the Microsoft 365 admin center and the actions admins can take, including limiting access, blocking agents, or escalating to security investigation in Microsoft Defender. Highlights a roadmap to incorporate additional security signals and explicitly defines what is out of scope to set correct expectations.

  https://learn.microsoft.com/en-us/microsoft-agent-365/guidance/detect-risky-agents

- **Why do local agents need their own governance?**

  Introduced conceptual guidance explaining why device-run (local) agents require distinct governance from cloud agents. Details how Agent 365 represents local agents with user- and device-bound identities for visibility in the Microsoft 365 admin center and how risk varies with device posture. Emphasizes maintaining inventory and visibility across devices and recommends safer defaults such as containment or isolated runtimes, with references to Defender for Endpoint discovery and protection.

  https://learn.microsoft.com/en-us/microsoft-agent-365/guidance/govern-local-agents

- **Why does Shadow AI governance matter for the enterprise?**

  Published guidance defining Shadow AI and the risks of unsanctioned tools and unmanaged agents, including lack of visibility, audit, and centralized control. Explains how Agent 365 enables discovery at scale and moves from detection to enforcement to block unauthorized agents. Encourages steering users to sanctioned, easier-to-use alternatives to meet business needs while maintaining control.

  https://learn.microsoft.com/en-us/microsoft-agent-365/guidance/govern-shadow-ai

- **How do enterprises control what agents can do?**

  Added guidance on tool-level governance for enterprise AI agents, defining tools such as connectors, MCP servers, skills, and plugins. Describes centralized visibility and approval of tools in the Microsoft 365 admin center, support for custom/BYOD MCP servers, and the ability to block risky tools organization-wide with Defender-integrated signals. Outlines future finer-grained controls at the function level and discovery for unmanaged tools to tighten governance over agent actions.

  https://learn.microsoft.com/en-us/microsoft-agent-365/guidance/govern-tools

- **How can we enforce agent policies at scale?**

  Introduced policy templates that bundle controls across Microsoft Entra, Microsoft Purview, Microsoft Defender, and SharePoint Online to reduce configuration drift and enforce consistent governance. Provides baseline templates and support for custom templates aligned to organizational risk and regulatory needs. Explains evolution from manual application at activation to automated, rule-based assignment across agent classes to sustain compliance as agents are created and operated.

  https://learn.microsoft.com/en-us/microsoft-agent-365/guidance/scale-governance

- **Why is securing AI agents a new kind of problem?**

  Published conceptual guidance on why agent security differs from traditional user or app security, emphasizing treating each agent as a first-class identity in Microsoft Entra. Highlights AI-specific attack surfaces and the need to enforce controls at action time between input processing and tool invocation, especially given machine-speed operations. Reinforces governance, monitoring, and policy enforcement anchored to agent identity to close gaps where legacy controls fall short.

  https://learn.microsoft.com/en-us/microsoft-agent-365/guidance/secure-agents