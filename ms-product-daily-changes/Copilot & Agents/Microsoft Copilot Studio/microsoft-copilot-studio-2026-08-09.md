# Microsoft Copilot Studio
**Date created:** 2026-08-09 UTC  
**Tags:** Agent, Security  

## Major Changes

- **Control image rendering and embedded URLs**
  
  Expanded and reorganized security guidance to let admins choose whether to block all images/URLs, block only contextually untrusted content, or allow all. Added step-by-step configuration for environments and environment groups via Security > Threat detection and Manage > Environment groups > Rules, plus a comparison table to aid selection. Clarified how “Block untrusted” evaluates context (citations, user input, Microsoft-managed redirectors) and how unsafe content is handled by stripping to plain text and flagging nested Markdown. These updates improve threat mitigation while giving organizations consistent, policy-driven control.
  
  https://learn.microsoft.com/en-us/microsoft-copilot-studio/image-render-embedded-url

- **Security and governance**
  
  Introduced Microsoft Agent 365 as a centralized control plane for observing, governing, and securing Copilot Studio agents with Entra identities, Conditional Access, RBAC/ABAC, and unified policy enforcement. Expanded governance capabilities with usage visibility and Copilot credit controls, connector dependency insights, GitHub-backed source control with deploy-from-Git, real-time risk assessments, and Entra network controls (GA). Enhanced guidance on how Agent 365 complements runtime protections, Purview auditing, and Microsoft Sentinel by providing centralized inventory and telemetry, and clarified data policy controls including Azure Monitor Application Insights. Customer Lockbox guidance was revised to note explicit exclusions for Copilot Studio security audit logs and Agent 365 governance/audit events, with links to further reading.
  
  https://learn.microsoft.com/en-us/microsoft-copilot-studio/security-and-governance

## Moderate Changes

- **Share agents with other users and makers**
  
  Updated sharing guidance for the new agent experience: sharing now grants view/test access only, while edit rights require turning off the new experience and/or assigning environment roles. Added prerequisites (appropriate licensing and publishing to Teams + Microsoft 365 with the Microsoft 365 Copilot option) and refreshed steps, labels, and organization-wide access behavior to clarify that broad access enables use without view/edit, along with revised instructions for stopping sharing.
  
  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/authoring-share-agent