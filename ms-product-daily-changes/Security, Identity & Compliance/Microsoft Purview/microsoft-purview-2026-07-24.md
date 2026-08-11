# Microsoft Purview
**Date created:** 2026-07-24 UTC  
**Tags:** Administration, Governance, Monitoring  

## Moderate Changes

- **Learn about archive mailboxes**
  
  Added guidance on auto-archiving that moves the oldest items to the archive mailbox when the primary mailbox nears capacity (default at 96%). Explains prerequisites and exclusions (requires a provisioned archive, skips “Never Move to Archive” and recent items) and how to configure the organization-wide threshold, including disabling by setting it to 100. Helps admins proactively manage storage while complementing time-based MRM policies.
  
  https://learn.microsoft.com/en-us/purview/archive-mailboxes

- **Learn about auto-expanding archiving**
  
  Clarified how the 1.5 TB archive limit is calculated, including Recoverable Items, and that additional storage is provisioned automatically but can take up to 30 days. Reiterated growth limits of up to 1 GB per day to set expectations for large archives. This helps plan capacity and avoid surprises when archives approach limits.
  
  https://learn.microsoft.com/en-us/purview/autoexpanding-archiving

- **Get started with activity explorer**
  
  Introduced timing expectations for when activities appear, noting 60–90 minute latency for core services and potentially longer for others, plus backfill behavior when devices come back online. Advises allowing time after enabling or changing policies and reminds readers of the 30‑day reporting window, with Audit search for recent verification. This helps teams interpret data freshness and troubleshoot perceived delays.
  
  https://learn.microsoft.com/en-us/purview/data-classification-activity-explorer

- **Onboard Windows devices into Microsoft 365 overview**
  
  Added a caution that device management currently supports Microsoft Entra roles only, not Purview roles. This clarifies role assignments required for onboarding and managing devices, reducing setup errors and access issues. Administrators can align permissions accordingly to streamline operations.
  
  https://learn.microsoft.com/en-us/purview/device-onboarding-overview

- **Learn about retention policies and retention labels**
  
  Clarified when retention periods start, covering creation time (default), last modified time for files, label application time, and event-based triggers. This helps organizations choose start conditions that match business and regulatory scenarios such as employee departures or contract expirations. Improves policy accuracy and predictability for records management.
  
  https://learn.microsoft.com/en-us/purview/retention