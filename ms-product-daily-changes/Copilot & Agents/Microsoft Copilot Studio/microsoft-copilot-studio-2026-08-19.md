# Microsoft Copilot Studio
**Date created:** 2026-08-19 UTC  
**Tags:** Configuration, Guidance, Governance, Identity, Security  

## Moderate Changes

- **Create a single response test set**

  Clarified SharePoint support for generating test cases: only individual SharePoint files are supported; folders aren’t supported. This reduces setup errors and ensures consistent test generation behavior. Terminology was updated to refer to “SharePoint files.”

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/analytics-agent-evaluation-create

- **App registration, agent identities, and authentication**

  Added guidance on skill validation and invocation, explaining that the system may obtain and present a token for the agent’s managed identity, scoped to the agent owner’s permissions to avoid privilege escalation. Emphasizes maker responsibility to configure and trust skill endpoints that can receive authenticated requests during validation and runtime, strengthening security and governance practices.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/requirements-certificates-configuration-values

- **Integrate voice agents with Teams Phone Agent (preview)**

  Expanded guidance showing how administrators can disable the Microsoft Teams Phone channel for Copilot Studio agents via the Agent access channels setting in the Power Platform admin center, with a link to related configuration. The note was reformatted for clarity, and the unsupported status of real-time voice agents remains unchanged.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/voice-teams-phone-agent