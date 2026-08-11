# Microsoft Defender XDR
**Date created:** 2026-08-06 UTC  
**Tags:** Agent, AI, Analytics, Security  

## New Articles

- **GetAnomalousBehaviorsAbout() function in advanced hunting for Microsoft Defender XDR**

  Introduced a new function that filters UEBA behavior insights by multiple entity or context criteria listed in an About array. The article documents syntax, the filter object schema, and evaluation logic, and explains expected input and return behavior. It includes end-to-end Kusto examples and links to related UEBA and BehaviorInfo resources to help analysts apply it effectively.

  https://learn.microsoft.com/en-us/defender-xdr/advanced-hunting-getanomalousbehaviorsabout-function

- **GetAnomalousBehaviorsByKind() function in advanced hunting for Microsoft Defender XDR**

  Added documentation for a function that narrows UEBA behavior insights by entity kind and optional insight type. The page outlines syntax, parameters, input requirements, and return behavior with practical Kusto examples for common filtering scenarios. Related links guide readers to BehaviorInfo and advanced hunting concepts.

  https://learn.microsoft.com/en-us/defender-xdr/advanced-hunting-getanomalousbehaviorsbykind-function

- **GetAnomalousBehaviorsByValue() function in advanced hunting for Microsoft Defender XDR**

  Published a new reference describing a function that finds UEBA insights involving a specific entity or context value across behaviors. It details syntax, required and optional parameters, expected input, and output characteristics, plus example queries to accelerate usage. Cross-references to UEBA anomalies guidance and BehaviorInfo are provided.

  https://learn.microsoft.com/en-us/defender-xdr/advanced-hunting-getanomalousbehaviorsbyvalue-function

- **GetFirstSeenBehaviors() function in advanced hunting for Microsoft Defender XDR**

  Introduced a function that filters behaviors containing FirstSeen insights to highlight novel or rare activity. The article covers syntax, input requirements, and what the function returns, with an example query against BehaviorInfo to find recent behaviors. Related links help readers explore UEBA anomalies and hunting best practices.

  https://learn.microsoft.com/en-us/defender-xdr/advanced-hunting-getfirstseenbehaviors-function

- **GetHighVolumeAnomalyBehaviors() function in advanced hunting for Microsoft Defender XDR**

  Added a function reference for isolating behaviors that include HighVolumeAnomaly insights. The content explains how to invoke the function, input expectations, and return behavior, and provides a sample query using BehaviorInfo. Links to related topics support deeper exploration.

  https://learn.microsoft.com/en-us/defender-xdr/advanced-hunting-gethighvolumeanomalybehaviors-function

- **GetUncommonValueBehaviors() function in advanced hunting for Microsoft Defender XDR**

  Published documentation for a function that filters behaviors with UncommonValue insights to surface atypical entities or attributes. It clarifies syntax, input requirements, and preserved output columns, and includes an example Kusto query with BehaviorInfo. Related references to UEBA anomalies and advanced hunting are included.

  https://learn.microsoft.com/en-us/defender-xdr/advanced-hunting-getuncommonvaluebehaviors-function

## Major Changes

- **Microsoft Security Copilot in advanced hunting**

  Consolidated separate experiences into a single Threat Hunting Assistant with two modes: Rich insights for conversational investigation and Query only for natural language to KQL. Updated access instructions to select modes from the side pane, clarified default and active mode indicators, and added the ability to switch to the Security Analyst Agent. Expanded guidance on dynamic, schema-aware data discovery across relevant tables (including custom Microsoft Sentinel tables) with read-only, permission-respecting behavior, replacing static table lists. Best practices and terminology were refreshed to align with the new assistant model.

  https://learn.microsoft.com/en-us/defender-xdr/advanced-hunting-security-copilot

- **Deploy AI agents in Microsoft Defender**

  Updated terminology to rename Threat Hunting Agent to Threat Hunting Assistant across the article, aligning with the new experience. Removed the Data Security Triage Agent in Data Loss Prevention section and its entry from the agents list to reflect current scope and capabilities. These changes simplify the agent portfolio and reduce confusion about deprecated functionality.

  https://learn.microsoft.com/en-us/defender-xdr/security-copilot-agents-defender

## Moderate Changes

- **Microsoft Security Copilot advanced hunting query assistant**

  Updated the workflow for running generated KQL queries to a new Run query split-button. Users can now run queries directly, add them to the editor without execution, and view the logic behind the query, with revised labels and images to match the experience.

  https://learn.microsoft.com/en-us/defender-xdr/advanced-hunting-security-copilot-query-assistant

- **Microsoft Security Copilot Threat Hunting Assistant in advanced hunting**

  Rebranded the experience from Threat Hunting Agent to Threat Hunting Assistant and removed preview indicators. Content was expanded to highlight schema-aware data discovery and iterative refinement, with updated guidance across setup, key capabilities, getting started, interpreting responses, and feedback.

  https://learn.microsoft.com/en-us/defender-xdr/advanced-hunting-security-copilot-threat-hunting-assistant

- **Configure Microsoft Sentinel scoping (row-level RBAC)**

  Clarified permissions by requiring both Data Operations (Manage) and Alerts (Manage) for Table Management. Added instructions to tag data via a DCR transformation using a SentinelScope_CF column and enable scoped access, including notes on column creation behavior and CI/CD deployment considerations.

  https://learn.microsoft.com/en-us/defender-xdr/scoping

- **Microsoft Security Copilot Security Analyst Agent**

  Updated how to switch to the Security Analyst Agent using the More actions menu and added steps to switch back to the Threat Hunting Assistant. Included a note that switching between experiences resets the conversation and refreshed imagery accordingly.

  https://learn.microsoft.com/en-us/defender-xdr/security-analyst-agent

- **What's new in Microsoft Defender XDR**

  Removed the July 2026 announcement for the Advanced hunting sign-in table migration. Updated the Microsoft Security Copilot natural language threat hunting entry to GA and renamed it from Threat Hunting Agent to Threat Hunting Assistant, with aligned links and labels.

  https://learn.microsoft.com/en-us/defender-xdr/whats-new