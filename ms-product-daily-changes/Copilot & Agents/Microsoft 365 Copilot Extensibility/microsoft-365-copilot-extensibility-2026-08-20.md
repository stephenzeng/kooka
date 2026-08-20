# Microsoft 365 Copilot Extensibility
**Date created:** 2026-08-20 UTC  
**Tags:** Configuration, Governance, Guidance, Troubleshooting  

## Moderate Changes

- **Build agents by using Agent Builder in Microsoft 365 Copilot**

  Updated guidance by removing a resolved known issue about default response mode behavior when invoking agents via @mention from the main Copilot experience. This clarifies that the default response mode now applies consistently, helping builders rely on expected agent responses.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/agent-builder-build-agents

- **Adaptive Card response templates for API plugins for Microsoft 365 Copilot**

  Added guidance to list all domains in the app manifest’s validDomains, including those used by Action.OpenUrl, to prevent untrusted content warnings in Teams. Introduced a new requirement that image URLs returned in Adaptive Card responses must use domains listed in validDomains or images won’t render in Microsoft 365 Copilot.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/api-plugin-adaptive-cards

- **Declarative agent schema 1.8 for Microsoft 365 Copilot**

  Removed a resolved known-issue note about default response mode not applying when agents are invoked via @mention from the main Copilot experience. This streamlines the schema documentation and confirms consistent response-mode behavior.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/declarative-agent-manifest-1.8

- **Known issues**

  Added a new issue for Copilot Studio agents using third-party models that can trigger an “Agent Blocked” error if access to those AI providers isn’t enabled, particularly in EU tenants. Provided two workarounds: have an admin grant access to the provider in the Microsoft 365 admin center and wait for propagation, or switch the agent to the default Microsoft model for immediate availability.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/known-issues