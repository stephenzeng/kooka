# Microsoft 365 Copilot connectors
**Date created:** 2026-08-09 UTC  
**Tags:** Administration, Agent, Governance, Security  

## Moderate Changes

- **Set up the Jira Cloud service for Jira Cloud connector ingestion**

  Added explicit callback URLs for Microsoft 365 GCC High and DoD when configuring the Customized Atlassian Jira OAuth 2.0 method. This enables proper authentication setup in US Government environments and reduces configuration errors.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/jira-cloud-admin-setup

- **Deploy the Jira Data Center connector**

  Clarified OAuth configuration by listing explicit Microsoft 365 environment names and distinct callback URLs for Enterprise, Government, GCC High, and DoD. This improves accuracy when setting Redirect URLs and helps prevent misconfigurations across environments.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/jira-data-center-deployment

- **Manage connector connections**

  Documented that if delete detection is unreliable due to connection failures, items not rediscovered for 28 days are automatically removed from the Microsoft 365 index. This clarifies index hygiene and compliance behavior so admins can monitor and remediate connection issues proactively.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/manage-connector

- **Manage federated connector availability**

  Announced retirement of the setFederatedConnectors CLI toggle by August 20, 2026, with governance now managed via the Allowed agent types setting in Agent 365. Admins should transition to the new tenant-wide setting to align connector and agent governance and update operational processes before retirement.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/manage-federated-connectors