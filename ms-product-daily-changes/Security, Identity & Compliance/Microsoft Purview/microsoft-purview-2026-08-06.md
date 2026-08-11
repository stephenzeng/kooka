# Microsoft Purview
**Date created:** 2026-08-06 UTC  
**Tags:** Administration, Governance, Security  

## Major Changes

- **Delete an inactive mailbox**

  Added end-to-end guidance on delay holds, a common reason mailboxes remain inactive after other holds are removed. Introduced a new section explaining what delay holds are, how to detect them (Get-Mailbox | FL *Delay*), their automatic 30‑day expiration, and how to remove them early using Set-Mailbox with RemoveDelayHoldApplied and RemoveDelayReleaseHoldApplied (requires the Legal Hold role). Clarified that recalculation does not remove holds and advised checking for all remaining holds, including delay holds, before forcing recalculation to avoid unnecessary delays.

  https://learn.microsoft.com/en-us/purview/delete-an-inactive-mailbox

## Moderate Changes

- **Audit log activities**

  Added a new Teams audit event, SecurityRiskInCallDetected, to surface potential security concerns in external calls. Clarified that Meeting Participant Detail records can be shared across participating tenants and updated availability for a related event to include GCC, GCC-High, DoD, and air-gapped environments, improving coverage and compliance awareness.

  https://learn.microsoft.com/en-us/purview/audit-log-activities

- **Learn about inactive mailboxes**

  Explained that Microsoft 365 automatically applies a delay hold after removing a hold to prevent immediate content purging. Clarified that mailboxes under a delay hold remain on hold and inactive until the delay hold expires or is removed, with references to managing and removing delay holds.

  https://learn.microsoft.com/en-us/purview/inactive-mailboxes-in-office-365

- **Learn about the Microsoft Purview portal**

  Clarified the exact permission required to view release notes (microsoft.office365.messageCenter/messages/read) and which roles include it (Message Center Reader, Global Reader, Global Administrator). Refined troubleshooting steps when expected release notes are not visible to ensure admins can verify access and configuration quickly.

  https://learn.microsoft.com/en-us/purview/purview-portal

- **Learn about sensitive information types**

  Added guidance on detection differences for the same sensitive information type across Exchange, SharePoint/OneDrive, and Endpoint DLP. Highlighted that Endpoint DLP evaluates files against all tenant SITs and that using bundled SITs in endpoint policies requires Advanced classification scanning and protection, with advice to test custom SITs per workload and consider content-extraction limits.

  https://learn.microsoft.com/en-us/purview/sit-sensitive-information-type-learn-about