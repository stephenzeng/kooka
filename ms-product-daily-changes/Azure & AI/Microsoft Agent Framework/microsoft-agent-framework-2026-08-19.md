# Microsoft Agent Framework
**Date created:** 2026-08-19 UTC  
**Tags:** Configuration, Guidance, Security  

## Major Changes

- **https://learn.microsoft.com/en-us/agent-framework/hosting/self-hosting/**

  Reorganized and expanded self-hosting guidance to improve discoverability and end-to-end setup. Added an ASP.NET Core integration example to expose an agent via OpenAI Responses, including required packages and route mapping, so teams can stand up endpoints faster. Introduced detailed guidance for persisting hosted sessions, clarifying that persistence is opt-in, outlining DI patterns for development vs. production, and providing a session store implementation skeleton with isolation and data protection best practices. Clarified how session stores relate to history providers to prevent configuration mistakes. Enhanced security guidance for session continuation with IsolationKeyScopedAgentSessionStore, new package references, and claims-based isolation to enforce tenant and user boundaries.

## Moderate Changes

- **OpenAI-Compatible Endpoints**

  Added guidance on continuing responses using either previous_response_id for chaining or conversation for stable threads, and documented how storage and snapshots work with MapOpenAIResponses and AgentSessionStore. Clarified that IDs must be treated as opaque and ownership must be verified before accepting continuation values, and recommended enabling session isolation to secure multi-tenant workflows.  
  https://learn.microsoft.com/en-us/agent-framework/hosting/self-hosting/openai-endpoints