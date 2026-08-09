# Microsoft Foundry
**Date created:** 2026-08-09 UTC  
**Tags:** Monitoring, Programming  

## Major Changes

- **Document translation SDKs**

  Expanded SDK coverage by adding JavaScript/TypeScript with installation commands, import patterns, and authentication examples for both batch and single document translation, plus a batch translation sample. Upgraded the .NET SDK to 3.0.0 and updated the default API version to 2026-03-01, with the language/version support table refreshed accordingly. Aligned Python and Java sections to the new structure to improve consistency and onboarding across languages.

  https://learn.microsoft.com/en-us/azure/ai-services/translator/document-translation/document-sdk-overview

- **Monitor agents with the Agent Monitoring Dashboard**

  Added Foundry portal-based configuration alongside Python and .NET, including steps to create agents and manage recurring evaluations (preview), with clearer distinctions between scheduled and continuous evaluation types. Renamed “Scheduled evaluations” to “Recurring evaluations (preview),” added a portal access prerequisite, updated UI imagery, and refreshed terminology across the article. Included substantial SDK examples in Python and C# for creating scheduled recurring evaluations (schedules) and continuous recurring evaluations (evaluation rules), referencing new scheduling classes and APIs to streamline setup.

  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/how-to-monitor-agents-dashboard

## Moderate Changes

- **What is Azure Translator document translation 2026-03-01?**

  Added JavaScript/TypeScript to the list of supported client libraries with a link to the SDK README and refined the .NET entry label. This clarifies available language options so developers can choose the right SDK more easily.

  https://learn.microsoft.com/en-us/azure/ai-services/translator/document-translation/latest/overview