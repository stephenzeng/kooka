# SharePoint
**Date created:** 2026-08-20 UTC  
**Tags:** Automation, Best Practices, Compliance, Configuration, Governance, Guidance  

## Major Changes

- **Manage inactive sites using inactive site policies**

  Expanded governance guidance to explain how overlapping policies behave and how notifications are suppressed for 30 days when policies of the same type overlap, including reporting as “Notified by another policy.” Clarified that different policy types track notifications independently and that enforcement precedence can remove sites from other policy scopes (for example, read-only or archive states). Detailed what happens when policies are disabled or deleted—future actions stop, past actions aren’t reversed, and site-level notification history persists (with same-type history naturally expiring after 90 days). Emphasized recommendations to avoid overlapping policies of the same type to ensure predictable outcomes.

  https://learn.microsoft.com/en-us/sharepoint/inactive-site-policy

- **Trim existing versions**

  Overhauled version-trimming guidance to cover tenant-level trimming (private preview) alongside site, library, and OneDrive scenarios, with prerequisites and known limitations. Introduced clear workflows for What-If impact analysis, trim modes, and step-by-step execution to help admins plan and mitigate risk. Expanded PowerShell coverage, including tenant-level cmdlets for data collection, impact estimation, policy application, progress tracking, and cancellation, and clarified site/library cmdlets. Strengthened cautions that trimmed versions are not recoverable without backups and reorganized the content for easier role-based execution.

  https://learn.microsoft.com/en-us/sharepoint/trim-versions

## Moderate Changes

- **Request recurring site attestations for SharePoint sites**

  Updated lifecycle guidance to clarify how overlapping attestation policies work, including 30-day suppression for same-type duplicates and independent tracking across different policy types. Explained enforcement precedence and what happens when a policy is disabled or deleted, including history retention and natural 90-day resets (with the option to contact Microsoft Support for earlier clearing). Recommended avoiding overlapping policies of the same type to prevent unpredictable notifications or enforcement.

  https://learn.microsoft.com/en-us/sharepoint/request-site-attestations

- **SharePoint site lifecycle management**

  Added guidance on overlapping lifecycle policies: same-type overlaps suppress duplicate notifications for 30 days, while different types track and enforce independently. Clarified effects of disabling or deleting policies, retention of notification history per policy type, and the natural 90-day reset (with an option to contact Microsoft Support to clear earlier). Advised avoiding overlapping policies of the same type for consistent, predictable outcomes.

  https://learn.microsoft.com/en-us/sharepoint/site-lifecycle-management

- **Create a SharePoint site ownership policy**

  Expanded policy interaction guidance, including 30-day duplicate-notification suppression for same-type overlaps and independent histories and enforcement for different types. Clarified that ownership notification recipient categories are cumulative eligible sets, not a fallback chain, and documented how disabling or deleting a policy affects future actions and notification history retention/reset. Consolidated prior overlapping-policy content into detailed, easier-to-follow sections.

  https://learn.microsoft.com/en-us/sharepoint/site-ownership-policy

- **IT Admins - Use OneDrive policies to control sync settings**

  Added a new Group Policy setting (EnableODIgnoreFolderListFromGPO) to block uploads of specified folder names via the OneDrive sync app. Documented exact-match, case-insensitive behavior, limitations (no wildcards, no retroactive removal, moving already-syncing files not supported), operational requirements (sync app restart), and the registry path for configuration.

  https://learn.microsoft.com/en-us/sharepoint/use-group-policy