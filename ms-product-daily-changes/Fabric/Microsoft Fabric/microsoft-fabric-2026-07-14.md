# Microsoft Fabric
**Date created:** 2026-07-14 UTC  
**Tags:** Administration, Analytics, Security  

## New Articles

- **Outbound Access Protection for Operations Agent (Preview)**

  Introduced a new concept article explaining how Workspace Outbound Access Protection (OAP) governs an operations agent’s outbound actions during preview. It outlines which actions are governed versus not governed, and highlights preview limitations such as blocked cross-workspace actions and dependencies on tenant Teams settings. The article details user-facing indicators when actions are blocked, configuration settings that influence outcomes, and how to monitor and troubleshoot via Activity Log. An FAQ clarifies expected behavior, scope, and admin remediation via allowlists.

  https://learn.microsoft.com/en-us/fabric/security/workspace-outbound-access-protection-operations-agent

## Major Changes

- **Fabric IQ in Microsoft 365 Copilot Cowork**

  Substantially updated to reflect Copilot Cowork general availability and the Fabric IQ plugin’s preview status for all Power BI customers. Added capabilities include referencing reports in workspace apps, value search across row-level data, native conversational analytics, and improved grounding via enhanced semantic signals. Guidance now clarifies sensitivity label behavior and updates prerequisites to usage-based Copilot Cowork licensing (no extra Fabric capacity/PPU), removing Frontier-specific references. The article also improves performance and tooling guidance, and refreshes limitations to align with current preview scope.

  https://learn.microsoft.com/en-us/fabric/iq/connectors/cowork-overview

## Moderate Changes

- **Direct Lake overview**

  Updated the feature matrix to state that calculated columns for Direct Lake are not supported, changing prior “Yes (preview)” to “No (coming soon).” This sets clearer expectations for modeling capabilities and planning.

  https://learn.microsoft.com/en-us/fabric/fundamentals/direct-lake-overview

- **Fabric Runtime 1.2 (EOS)**

  Expanded cautions to note Runtime 1.2 has reached end of support, highlight ongoing operational and security risks, and announce phased disablement of jobs. Strongly recommends upgrading to Runtime 1.3 to maintain support and reliability.

  https://learn.microsoft.com/en-us/fabric/data-engineering/runtime-1-2

- **Fabric Runtime 2.0 (Preview)**

  Updated Delta Lake references to 4.2 and announced a Python runtime upgrade that causes breaking changes for Environment artifacts using Python/wheel libraries. Provides required actions to republish environments by removing and re-adding libraries, and links to Delta Lake 4.2 release notes; removed the WASB deprecation note.

  https://learn.microsoft.com/en-us/fabric/data-engineering/runtime-2-0

- **Workspace outbound access protection for graph**

  Renamed and refocused the article on graph, clarified enablement behavior, and expanded scope notes. It now specifies that Fabric IQ supports OAP for both graph (this article) and operations agent, with a link to the related article.

  https://learn.microsoft.com/en-us/fabric/security/workspace-outbound-access-protection-graph

- **Workspace outbound access protection**

  Expanded the Fabric IQ coverage to include the Operations agent under data connection rules. This broadens the documented scope of workloads governed by workspace outbound access protection.

  https://learn.microsoft.com/en-us/fabric/security/workspace-outbound-access-protection-overview