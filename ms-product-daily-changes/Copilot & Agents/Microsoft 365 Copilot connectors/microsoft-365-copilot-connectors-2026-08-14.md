# Microsoft 365 Copilot connectors
**Date created:** 2026-08-14 UTC  
**Tags:** Compliance, Configuration, Get Started, Governance, Guidance, Identity, Security  

## Moderate Changes

- **Microsoft Graph connector agent**

  Expanded the network allowlist to include U.S. DoD endpoints and refined GCCH entries, improving clarity for sovereign cloud deployments. Updated installation prerequisites to require .NET Core Desktop Runtime 10.0 (x64), ensuring admins install the correct runtime. These changes help streamline secure setup and reduce connectivity issues.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/connector-agent

- **File Share connector**

  Updated limitations to state that symlinks, NTFS junctions, and volume mount points aren’t indexed. This clarification helps admins plan crawls accurately and avoid unexpected gaps in coverage.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/fileshare-connector

- **Manage self-serve sync connector availability (preview)**

  Rebranded “personal sync connectors” to “self-serve sync connectors” across the article, adding a preview label and aligning terminology for admin controls and connector behavior. The changes improve consistency in naming without introducing new procedures.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/manage-personal-sync-connectors

- **Copilot connectors overview**

  Renamed “Personal configuration” to “Self-serve configuration” throughout, updating headings, feature lists, and comparison tables. Cross-references now use the “Self-serve sync connectors” naming to keep terminology consistent and easier to navigate.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/overview

- **Self-serve sync connectors overview**

  Rebranded the feature from “Personal sync connectors” to “Self-serve sync connectors,” marked as preview, and clarified that users configure connectors per user. Refreshed the step-by-step setup flow and added a dedicated “How to disconnect” section header, improving readability without changing existing steps. Related link text was aligned with the new terminology.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/personal-sync-connectors-overview

- **Set up ServiceNow Knowledge connector prerequisites by using background scripts**

  Added Federated Auth setup guidance, including a new federated_auth_setup.js script that configures OIDC provider settings, Application Registry, auth scopes, and a machine integration user. Introduced step-by-step instructions with required variables (SP_OBJECT_ID, TENANT_ID) and guidance to reuse the service principal object ID for the subsequent row_level_acl_setup.js script. These updates streamline secure OIDC configuration and reduce deployment errors.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/servicenow-knowledge-setup-scripts