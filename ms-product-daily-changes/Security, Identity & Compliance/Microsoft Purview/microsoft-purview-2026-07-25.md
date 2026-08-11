# Microsoft Purview
**Date created:** 2026-07-25 UTC  
**Tags:** Governance, Security  

## Moderate Changes

- **Automatically apply a sensitivity label to Microsoft 365 data**

  Updated guidance clarifies how simulation differs from enforcement, including that enforcement resolves conflicts across multiple policies. Clarified that auto-labeling evaluates content against the latest sensitive information types only for items created or modified after those updates, recommending on-demand classification for older unchanged files. Also specified that Exchange simulations only assess messages sent or received during the simulation window, helping admins interpret results and plan rollouts.

  https://learn.microsoft.com/en-us/purview/apply-sensitivity-label-automatically

- **Disposition of content**

  Added a Disposition timelines section detailing permanent deletion within 15 days after approval, an optional auto-approval window of 7–365 days (default 14), and configuration change propagation of up to 7 days. These timelines improve predictability for review processes and change management.

  https://learn.microsoft.com/en-us/purview/disposition

- **Minimum versions for sensitivity labels in Office apps**

  Expanded the support matrix to indicate that label inheritance from email attachments is now available on an additional platform. This helps admins validate minimum client requirements and plan deployment accordingly.

  https://learn.microsoft.com/en-us/purview/sensitivity-labels-versions