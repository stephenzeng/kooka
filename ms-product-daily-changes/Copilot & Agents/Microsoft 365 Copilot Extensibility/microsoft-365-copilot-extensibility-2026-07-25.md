# Microsoft 365 Copilot Extensibility
**Date created:** 2026-07-25 UTC  
**Tags:** Administration, Agent, Programming  

## Moderate Changes

- **Build Microsoft 365 Copilot connectors for people data**

  Removed the beta label for the personWorkPositions field and updated the schema to reflect its standard availability. Added guidance that Microsoft Graph skips accounts without an Exchange Online mailbox, helping avoid indexing gaps and ingestion errors.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/build-connectors-with-people-data

- **Use developer mode in Microsoft 365 Copilot to test and debug agents**

  Documented Agent ID prefixes (U_ for user-scoped/sideloaded, T_ for tenant-scoped, P_ for public) to make agent scope easier to recognize during testing. Linked to publishing guidance for sideloading, organization catalog submission, and public release to streamline the path from development to distribution.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/debugging-agents-copilot-studio

- **Declarative agent schema 1.6 for Microsoft 365 Copilot**

  Removed the prior limitation stating that using local files packaged with the app was not available, indicating the capability is now supported. This enables agents to reference files included in the app package for more reliable and self-contained deployments.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/declarative-agent-manifest-1.6

- **Declarative agent schema 1.7 for Microsoft 365 Copilot**

  Updated documentation to reflect availability of using files packaged locally with the app, removing the previous “not yet available” note. Teams can now bundle required resources directly in the package to simplify setup and reduce external dependencies.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/declarative-agent-manifest-1.7

- **Declarative agent schema 1.8 for Microsoft 365 Copilot**

  Clarified that embedded knowledge files in app packages are now supported by removing the earlier limitation notice. This improves agent reliability and portability by allowing essential knowledge assets to ship with the app.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/declarative-agent-manifest-1.8