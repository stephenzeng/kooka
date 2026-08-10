# Microsoft Copilot Studio
**Date created:** 2026-07-16 UTC  
**Tags:** Administration, AI, Agent, Security  

## New Articles

- **Fix Copilot Studio License Errors Blocking Access and Publishing**

  Introduced a troubleshooting guide for licensing issues that block publishing agents or accessing Copilot Studio. Details common causes, including missing Copilot Studio authors group configuration for pay-as-you-go, absent per-user licenses, viral trial conflicts with tenant settings, and missing tenant-level enablement that triggers error code 7604. Provides step-by-step fixes: configure tenant settings and groups, assign the Copilot Studio Per User license, remove viral trial licenses and enable “Publish bots with AI features,” and set up tenant-level licensing via credits, message pack, or pay-as-you-go. Advises signing out and back in after changes and links to related licensing and tenant settings resources.

  https://learn.microsoft.com/en-us/troubleshoot/power-platform/copilot-studio/licensing/publish-license-error

## Moderate Changes

- **Fix Copilot Studio Agent Not Responding in Test Your Agent Panel**

  Expanded troubleshooting for agents that don’t respond in the Test your agent panel, especially for Copilot Studio agents, Microsoft Fabric Data agents, Microsoft Foundry agents, computer-using agents, flows, and certain connectors. Clarifies the root cause as SSE traffic on the /subscribe endpoint being buffered or inspected by firewalls/proxies over TLS, which breaks real-time updates. Adds concrete diagnostics (check request size/state and EventStream/Response) and recommends allow/bypass/exempt rules for the request path to restore streaming.

  https://learn.microsoft.com/en-us/troubleshoot/power-platform/copilot-studio/authoring/agent-test-no-response

- **Bring your own model for your prompts**

  Added a “Supported models and limitations” section clarifying that only chat completion endpoints are supported, requiring an endpoint that ends with /chat/completions. Explains that using the Responses API (/openai/v1/responses) results in “Resource not found” and that GPT-5 family and later models aren’t supported.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/bring-your-own-model-prompts