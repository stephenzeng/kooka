# Microsoft 365 Copilot connectors
**Date created:** 2026-08-28 UTC  
**Tags:** Configuration, Governance, Guidance  

## Moderate Changes

- **Deploy the Azure File Share connector**
  Clarified that the connector supports only full crawls and does not perform incremental crawls. Updated guidance to select sync intervals suitable for full daily crawls, helping admins plan schedules and system load accordingly.
  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/azure-file-share-deployment

- **Manage federated connector availability**
  Revised the deprecation timeline for the CLI toggle to August 25, 2026, and introduced governance via the Allowed agent types setting in the Microsoft 365 admin center with step-by-step instructions. Added transition guidance and FAQs, including behavior parity notes and persistence of previously disabled settings until October 20, 2026, to help organizations manage connector availability during the changeover.
  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/manage-federated-connectors