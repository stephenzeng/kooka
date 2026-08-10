# Microsoft Purview
**Date created:** 2026-07-15 UTC  
**Tags:** Security  

## Moderate Changes

- **Search the audit log for specific email messages**

  Removed a note implying the MailItemsAccessed operation requires a Microsoft 365 E5 license. This streamlines licensing guidance and reduces confusion for admins configuring audit searches.

  https://learn.microsoft.com/en-us/purview/audit-log-search-email

- **Collection policy reference**

  Clarified detection behavior for unmanaged cloud apps by tightening wording and removing an outdated explanation about cross-app request detection. The update sets clearer expectations for how policies match targeted apps and improves accuracy of policy design.

  https://learn.microsoft.com/en-us/purview/collection-policies-policy-reference

- **Learn about Data Loss Prevention for Cloud Apps in Edge for Business**

  Documented automatic activation of DLP for unmanaged apps in Edge for Business when admins save relevant Purview policies, and clarified required admin permissions. Expanded enforcement guidance on app catalog coverage, destination-traffic-based detection, and encoded/dynamic endpoints, and noted that Endpoint DLP policies take precedence over inline browser DLP for the same context. These updates help admins predict policy behavior and resolve conflicts more reliably.

  https://learn.microsoft.com/en-us/purview/dlp-browser-dlp-learn

- **Configure endpoint data loss prevention settings**

  Expanded and reorganized printer assignment parameters with explicit Windows and macOS support details, and clarified USB printer enforcement. Added guidance on obtaining and converting Device Instance paths for USB Product and Vendor IDs and refined definitions for corporate, universal, local, and print-to-file options. This improves policy accuracy and reduces configuration errors.

  https://learn.microsoft.com/en-us/purview/dlp-configure-endpoint-settings

- **Get started with data loss prevention protections for Recall**

  Removed the preview designation for DLP protection of Recall snapshots, indicating general availability. This signals readiness for production use without preview caveats.

  https://learn.microsoft.com/en-us/purview/dlp-recall-get-started

- **Learn about Endpoint data loss prevention**

  Updated the capabilities table to mark certain printer-group parameters—Print to file, Universal Print deployed on a printer, Corporate printer, and Print to local—as Windows-only. This clarifies OS-specific support to avoid misconfiguration.

  https://learn.microsoft.com/en-us/purview/endpoint-dlp-learn-about

- **Microsoft Purview Information Protection client - Release management and supportability**

  Added a Windows section for version 3.2.147.0 Preview with fixes and improvements over 3.2.146.0. Updated to Microsoft Information Protection SDK 1.18.128 and refreshed third-party components, removing obsolete libraries. These updates improve stability and compatibility.

  https://learn.microsoft.com/en-us/purview/information-protection-client-relnotes