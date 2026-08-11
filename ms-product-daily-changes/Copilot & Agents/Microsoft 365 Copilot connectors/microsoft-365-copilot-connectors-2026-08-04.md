# Microsoft 365 Copilot connectors
**Date created:** 2026-08-04 UTC  
**Tags:** Administration, AI  

## New Articles

- **Release history for Microsoft Graph connector agent**

  Introduced a comprehensive release history covering versions 1.1.0.0 through 4.0.2.0 for the Microsoft Graph connector agent. Highlights include support for newer .NET versions, GA of the Confluence On-premises connector, and expanded compatibility with Microsoft 365 Copilot Search and GitHub server connectors. The page details diagnostics (health checks, index stats), reliability and performance improvements, authentication updates (including OAuth 2.0 and government cloud support), parser/file handling fixes, and a critical security patch in 3.0.0.0 with deprecation guidance. This helps admins plan safe upgrades, ensure security posture, and troubleshoot deployments more effectively.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/connector-agent-releases

- **Deploy the Trello connector**

  Added a step-by-step deployment guide for the Trello Microsoft 365 Copilot connector. It covers prerequisites, setting up a Trello app, obtaining API credentials, configuring OAuth, deploying via the Microsoft 365 admin center, rolling out to a limited audience, and default sync settings. Optional guidance explains how to refine permissions, set up identity mapping, configure managed properties, and tune sync intervals for governance and performance. This enables faster, compliant onboarding of Trello data into Copilot experiences.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/trello-deployment

## Major Changes

- **Federated connectors overview**

  Reworked the page from a flat list into a categorized table that organizes available federated connectors by domain (such as Productivity, Sales and marketing, Development tools, and more). The categories now enumerate a broader set of data sources, improving coverage and clarity. Wording was updated to reflect a general catalog of federated connectors rather than only Microsoft-published options. This improves discoverability and helps admins quickly assess coverage and plan connector adoption.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/federated-connectors-overview

## Moderate Changes

- **Manage federated connector availability**

  Updated prerequisites and authentication guidance to require the Search Administrator role instead of AI Administrator for managing the tenant-wide availability toggle via PowerShell. This change ensures the correct permissions are used and helps avoid role-based deployment issues.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/manage-federated-connectors

- **Submit a federated connector**

  Clarified that post-submission validation is coordinated via email rather than through a Microsoft business development representative. This sets accurate expectations for follow-up, streamlining communication and next steps for publishers.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connectors/submit-federated-connector