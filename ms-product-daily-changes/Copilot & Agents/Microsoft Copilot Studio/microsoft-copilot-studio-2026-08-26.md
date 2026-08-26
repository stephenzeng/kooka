# Microsoft Copilot Studio
**Date created:** 2026-08-26 UTC  
**Tags:** Analytics, Billing, Configuration, Consumption, Governance, Guidance, Monitoring, Troubleshooting  

## New Articles

- **Federated Knowledge Service Provisioning Error 0x80072042**

  Introduced a troubleshooting article for Federated Knowledge Service provisioning failures when the “Block unmanaged customizations” managed environment policy is enabled. It explains symptoms including error 0x80072042 during provisioning and 0x80048d0b during knowledge search, and traces the root cause to solution-aware DVFileSearch components being blocked from creating unmanaged records. The guidance instructs adding UnstructuredFileSearchSkill (DVFileSearch) and related DVFileSearchEntity and DVFileSearchAttributes to the managed solution before export. It also provides step-by-step remediation, ALM prevention practices, and details to include in support cases.

  https://learn.microsoft.com/en-us/troubleshoot/power-platform/copilot-studio/lifecycle-management/block-unmanaged-customizations

## Moderate Changes

- **Bypass connector consent cards for an agent**

  Clarified that disabling connector consent applies only to agents using the standard harness and does not apply to the GitHub Copilot harness. This helps admins avoid misconfiguration by applying the setting only where it takes effect.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/admin-connector-consent-bypass

- **View agent's billing consumption**

  Updated navigation and UI terminology from Analytics to Monitor, including where to find Copilot Credits, billed sessions, and how to adjust the time range. This aligns guidance with the current product experience so readers can reliably locate billing and consumption insights.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/analytics-consumption

- **Monitor time and cost savings for agents**

  Retitled and refreshed UI references from Analytics to Monitor, updating labels like “Add to Monitor” and related instructions. The changes align terminology and screenshots with the Monitor experience without altering the underlying workflow.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/analytics-cost-savings

- **Monitor your agent with custom metrics (preview)**

  Renamed the article and steps from “Analyze” to “Monitor” and updated references to the Monitor page where custom metrics tiles reside. These adjustments ensure the instructions match the current navigation and labels while keeping the feature behavior unchanged.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/analytics-custom-metrics

- **Monitor conversational agents**

  Revised headings, terminology, and links from Analytics to Monitor, including updates to savings language and key insights phrasing. Readers can now follow Monitor-based navigation and labels to evaluate agent effectiveness.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/analytics-improve-agent-effectiveness

- **Monitor autonomous agents**

  Shifted the article’s context from Analytics to Monitor across the title, headings, and steps, including time-range selection on the Monitor page. This ensures guidance reflects where to review sessions and health insights in the current UI.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/analytics-improve-agent-health

- **Monitor overview**

  Rebranded the content from Analytics to Monitor, updating navigation, hybrid view descriptions, topic panel references, and availability/retention statements. These revisions align concepts and link text with the Monitor experience to reduce confusion.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/analytics-overview

- **FAQ for Monitor**

  Updated the H1, introduction, and related links to use Monitor terminology and reflect the Copilot Studio Monitor tab. This maintains consistency with the current UI without introducing new features.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/faqs-analytics