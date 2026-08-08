# Microsoft Defender for Cloud Apps
**Change date:** 2026-08-07 UTC  
**Tags:** Monitoring, Security  

## Moderate Changes

- **Anomaly detection policies in Microsoft Defender for Cloud Apps**
  Clarified that the “Activity performed by terminated user” policy is disabled, migrated to the dynamic threat detection model, and renamed to “Activity by a deprovisioned user,” reducing confusion about current policy behavior. Updated guidance references integration with Microsoft Defender XDR for Exchange Online protections in the “Suspicious email deletion activity (Preview)” scenario. Wording and heading refinements improve readability and alignment with current capabilities.
  https://learn.microsoft.com/en-us/defender-cloud-apps/anomaly-detection-policy

- **Hunt for threats in app activities | Microsoft Defender for Cloud Apps**
  Updated Advanced Hunting limits to clarify default returns up to 1,000 results, with an adjustable cap up to 100,000 rows, and noted partial results when queries exceed a 64 MB threshold. Confirmed these limits do not apply to app governance, helping analysts tune large queries and set correct expectations for output size.
  https://learn.microsoft.com/en-us/defender-cloud-apps/app-activity-threat-hunting

- **US Government offerings**
  Removed several example risk indicators from suspicious OAuth app detections (such as phishing redirects, logo impersonation, and typosquatting). This streamlines the documentation for US Government offerings and better reflects the current detection catalog.
  https://learn.microsoft.com/en-us/defender-cloud-apps/editions-cloud-app-security-gcc

- **Migrate file policies to Microsoft Purview**
  Refined parity details and action mappings between Defender for Cloud Apps file policies and Microsoft Purview DLP, including clearer behavior for Admin and User quarantine and “Remove specific collaborator.” Added configuration guidance for Purview file quarantine in SharePoint and OneDrive, explaining how files are moved to an admin-controlled quarantine site, permissions are removed, and a notification file remains in the original location. These updates help admins plan migrations and understand containment outcomes.
  https://learn.microsoft.com/en-us/defender-cloud-apps/migrate-file-policies-to-purview

- **Troubleshoot access and session controls for admins | Microsoft Defender for Cloud Apps**
  Added troubleshooting steps for unexpected website blocks, including how to distinguish between Conditional Access App Control enforcement and unsanctioned-app blocks via Defender for Endpoint. Provided a procedure to locate the responsible policy using Entra sign-in logs and the Activity log, review matched conditions and defaults, and use Admin View to bypass or record sessions for diagnostics. The issues table now includes a dedicated entry to speed triage.
  https://learn.microsoft.com/en-us/defender-cloud-apps/troubleshooting-proxy