# Microsoft Defender XDR
**Date created:** 2026-07-20 UTC  
**Tags:** Security  

## New Articles

- **AI agent posture risk in Microsoft Defender (Preview)**

  Introduced a new article explaining how Microsoft Defender evaluates AI agent posture risk, including how risk indicators and their states drive overall risk levels. Details the calculation of likelihood, impact, and severity, with special handling for Critical Resource and Active Threat scenarios. Provides a comprehensive catalog of enterprise-agent and local-agent risk indicators and explains how Active Threat is derived from qualifying alerts. Clarifies when security recommendations appear and how they relate to, but are distinct from, risk levels.

  https://learn.microsoft.com/en-us/defender-xdr/security-for-ai/ai-agent-risk-assessment

## Moderate Changes

- **Discover AI agents and assess security posture using Microsoft Defender**

  Reorganized guidance to center on reviewing AI agent risk in the Defender portal, with expanded steps for using the AI Agents page and clearer navigation. Clarified that risk levels come from active indicators (separate from recommendations) and improved Advanced Hunting guidance to use the AgentsInfo table and return the latest agent state with arg_max. Standardized terminology from “AI Assets” to “AI Agents” and streamlined the discovery-to-assessment flow, with refined investigation and protection links.

  https://learn.microsoft.com/en-us/defender-xdr/security-for-ai/ai-agent-inventory