# Microsoft 365 Copilot
**Date created:** 2026-07-30 UTC  
**Tags:** Administration, Agent, Programming  

## Major Changes

- **Build plugins for Copilot Cowork**

  Added a requirement for connectors to include an mcpToolDescription with a referenced file inside the ZIP package, with updated examples and validation rules to enforce it. Introduced a v1.28 manifest schema that blocks unsupported fields (additionalProperties: false), preventing use of fields like packageName. Updated packaging guidance to include a tools/ folder and revised cross-platform commands, and added instructions for local testing via Dev Tunnels with troubleshooting for 502 and IPv4/IPv6 binding issues. These changes tighten schema compliance, reduce packaging errors, and streamline testing and rollout.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/cowork-plugin-development

## Moderate Changes

- **Manage plugins for Copilot Cowork**

  Updated the manifest example to remove the deprecated packageName field and add mcpToolDescription with a file reference under remoteMcpServer. Replaced the “Sideloaded plugins” section with guidance for testing as the plugin author and tenant-wide distribution via the Microsoft 365 admin center. This improves clarity for internal testing and controlled rollouts before store publication.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/cowork-manage-plugins