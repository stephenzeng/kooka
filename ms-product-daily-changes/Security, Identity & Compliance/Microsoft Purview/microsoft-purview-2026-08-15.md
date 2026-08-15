# Microsoft Purview
**Date created:** 2026-08-15 UTC  
**Tags:** Compliance, Governance, Guidance, Monitoring, Security  

## Moderate Changes

- **Audit log activities**

  Added new audit activities covering Dragon Copilot role definition listing/viewing and Microsoft Fabric (Power BI) operations including warehouse alias assignments, tenant relocation consent/execution, and SQL connection mode changes. These additions expand visibility into administrative and workspace actions, improving monitoring, investigations, and compliance reporting.

  https://learn.microsoft.com/en-us/purview/audit-log-activities

- **Use the Insights tab to analyze auto-labeling policies in Microsoft Purview**

  Clarified that enforcement metrics include only SharePoint and OneDrive files, and that Exchange email activity should be reviewed in Activity explorer. Updated the “Total labeled to date” description to prevent misinterpretation of labeling counts.

  https://learn.microsoft.com/en-us/purview/auto-label-insights-tab

- **Minimum versions for sensitivity labels in Office apps**

  Added a new OneNote section with a capabilities matrix and minimum supported versions across Windows, Mac, iOS, Android, and Web, detailing available and unsupported labeling features. Includes an admin note that tenant opt-in is required, helping organizations plan rollout and set user expectations.

  https://learn.microsoft.com/en-us/purview/sensitivity-labels-versions

- **What's new in Microsoft Purview**

  Introduced simulation mode for auto-labeling policies to assess match results and source distribution before enforcement. Added an Insights tab that provides performance views for policies in both simulation and enforcement modes, improving policy tuning and governance.

  https://learn.microsoft.com/en-us/purview/whats-new