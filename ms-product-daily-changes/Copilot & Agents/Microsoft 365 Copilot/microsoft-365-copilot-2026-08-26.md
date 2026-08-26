# Microsoft 365 Copilot
**Date created:** 2026-08-26 UTC  
**Tags:** Configuration, Governance, Guidance, Security  

## Moderate Changes

- **Choose a model for Copilot Cowork**

  Added configurable effort levels (Light through Max, with Medium as default) to help balance response quality, speed, and cost. Clarified that higher effort increases processing time and usage, and that both model and effort can be set directly in the compose box. Provides guidance on when to select each level to optimize outcomes.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/cowork-models

- **Build plugins for Copilot Cowork**

  Clarified how to identify Cowork traffic using the case-insensitive “copilot-cowork” User-Agent prefix and MCP initialize clientInfo, with guidance on choosing per-request versus per-session identification. Explained that software identity includes only the software name and contract version, not tenant, user, session, or connector details, and recommended enforcing those distinctions via authorization. Noted that custom plugins aren’t supported on mobile.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/cowork-plugin-development

- **Manage scheduled prompts for Microsoft Copilot**

  Updated governance guidance to reflect scheduled prompts moving from Optional Connected Experiences to Connected Experiences effective August 2026. Admin policy references now use “Allow the use of connected experiences in Office,” with aligned controls and terminology, while confirming that user creation, editing, and execution of existing scheduled prompts are unchanged.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/scheduled-prompts