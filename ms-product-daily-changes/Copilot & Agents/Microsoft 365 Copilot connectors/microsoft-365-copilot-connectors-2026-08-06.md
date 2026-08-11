# Microsoft 365 Copilot connectors
**Date created:** 2026-08-06 UTC  
**Tags:** AI, Administration, Governance, Security  

## New Articles

- **Manage personal sync connector availability**

  Introduced a new admin guide for controlling the availability of Microsoft-published personal sync connectors in the Microsoft 365 admin center. It covers enabling or disabling connectors tenant-wide, staged rollouts to Entra ID groups, and tracking adoption metrics, with an initial admin-only review window to vet new connectors. The article clarifies prerequisites and security behaviors, including user-scoped identity, delegated OAuth 2.0, encrypted token storage, per-user indexing with ~90-day lookback, and automatic deletion of indexed content when access is revoked. FAQs explain how personal connectors differ from tenant-configured synced and federated connectors, coexistence rules, and expected indexing/latency, helping admins govern rollout with confidence.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/manage-personal-sync-connectors

- **Personal sync connectors overview**

  Introduced an overview of personal sync connectors that let individual users authenticate to external sources and index their own content into Microsoft Graph for Copilot in Chat and Search. It outlines supported sources (currently Confluence Cloud and Jira Cloud) with crawl scope and 90-day limits, and explains admin controls for enabling or disabling availability. The page walks through user setup, initial and incremental sync cadences, and disconnect behavior, helping organizations evaluate suitability and readiness. Related links point to management guidance and the broader connectors overview.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/personal-sync-connectors-overview

## Moderate Changes

- **Copilot connectors overview**

  Updated the overview to distinguish tenant-configured and personal-configured synced connectors, and expanded the comparison table to include both synced modes alongside federated connectors across data handling, access, setup, use cases, and connector availability. Added a dedicated section on personal configuration covering per-user indexing, identity/consent, permission enforcement, and removal behavior, with a link to the personal sync connectors overview to guide readers to detailed guidance.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/overview