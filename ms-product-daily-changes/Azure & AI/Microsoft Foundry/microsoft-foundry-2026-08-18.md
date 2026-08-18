# Microsoft Foundry
**Date created:** 2026-08-18 UTC  
**Tags:** Analytics, Automation, Compliance, Configuration, Deprecation, Guidance, Monitoring, Security  

## New Articles

- **Content provenance**

  Introduced a new concept article outlining how content provenance is implemented for Microsoft Foundry models, why it matters, and Microsoft’s commitments to build these capabilities and make them available to customers. Explains the use of C2PA Content Credentials and invisible watermarks and how to detect and interpret signals via a website and an API. Details current coverage for image and audio modalities across supported model families and notes format and deployment nuances. Clarifies limitations—provenance is not the same as trustworthiness or authorship—and sets expectations for customer transparency responsibilities.

  https://learn.microsoft.com/en-us/azure/foundry/responsible-ai/content-safety/provenance-disclosure

## Major Changes

- **Available tools and example prompts for Foundry MCP Server (preview)**

  Expanded the reference to 50 tools across 12 categories, adding toolbox management capabilities to create, version, update, set defaults, and delete toolboxes and versions. Clarified and extended model catalog and deployment management for Managed Compute, including new indicators in listing and details APIs and new deployment operations for Azure-sold models and Managed Compute, while marking the legacy model_deploy as a deprecated alias. Added Managed Compute accelerator quota to monitoring and provided related prompts. Introduced a new continuous evaluation section with tools to configure, schedule, and manage evaluations for prompts and hosted agents, plus example workflow steps to operationalize evaluation.

  https://learn.microsoft.com/en-us/azure/foundry/mcp/available-tools

## Moderate Changes

- **Hosted agents in Foundry Agent Service**

  Updated conceptual guidance to clarify that compute is provisioned per session at runtime with dedicated endpoints and agent identities, and that the platform manages scaling, state, observability, and lifecycle. Added an architecture diagram and a protocol selection decision tree with details on payloads and lifecycle for Responses, Invocations, and WebSocket Invocations, and emphasized that agents can expose multiple protocols. Enhanced session lifecycle guidance to note that compute follows the session and that $HOME and /files persist and are restored on resume, with a new request flow sequence diagram.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/hosted-agents

- **Language support for Language features**

  Updated language support indicators to add coverage for French, German, and Spanish, improving clarity on where features are available. Also updated the Conversation PII GA language list to include German, expanding multilingual PII detection. No other content changes were made.

  https://learn.microsoft.com/en-us/azure/ai-services/language-service/concepts/language-support