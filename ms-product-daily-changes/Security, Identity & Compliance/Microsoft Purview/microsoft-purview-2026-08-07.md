# Microsoft Purview
**Change date:** 2026-08-07 UTC  
**Tags:** Security  

## New Articles

- **Use the Insights tab to analyze auto-labeling policies in Microsoft Purview**

  Introduced a new article covering the Insights tab for auto-labeling policies, available for active policies in the Purview portal. It explains simulation insights such as policy details, rule matches, source breakdowns (Exchange, SharePoint, OneDrive), and sensitive info types, noting that Exchange counts are estimates. It also details enforcement-mode operational metrics over 30 days, including labeling outcomes, failure reasons, and label distribution by source, with caveats for non-Microsoft locations. The article links to related guidance on simulation results, monitoring, resolving failures, and deployment best practices.

  https://learn.microsoft.com/en-us/purview/auto-label-insights-tab

- **Review simulation results for auto-labeling policies in Microsoft Purview**

  Added guidance on reviewing auto-labeling simulation results, including prerequisites and roles. The article explains key metrics (policy status, duration, matched and sample items, rule-level matches, source breakdowns, and detected sensitive info types), with context on sampling and estimated counts. It outlines how to assess sample items and recommends next steps to either turn on the policy or refine settings and rerun.

  https://learn.microsoft.com/en-us/purview/auto-label-simulation-results

## Moderate Changes

- **Enable sensitivity labels for files in SharePoint and OneDrive**

  Added a limitation clarifying that external tenant users cannot open files protected with a user-defined permissions label when access is granted to a group in the external tenant. Updated guidance recommends granting permissions directly to the external user within the label or adding the user to a group in the hosting tenant and assigning permissions to that group to ensure access works reliably.

  https://learn.microsoft.com/en-us/purview/sensitivity-labels-sharepoint-onedrive-files