# Microsoft Defender for Endpoint
**Date created:** 2026-08-22 UTC  
**Tags:** Configuration, Guidance, Security, Troubleshooting  

## Moderate Changes

- **Schedule antivirus scans using PowerShell**

  Clarified the DisableCatchupQuickScan parameter so admins understand that catch-up quick scans run after missed scans when a device powers on or resumes from sleep or hibernation. Corrected the documented default value to $false to prevent misconfigured scripts and unintended scans.

  https://learn.microsoft.com/en-us/defender-endpoint/schedule-antivirus-scans-powershell

- **Troubleshoot Microsoft Defender Antivirus scan issues**

  Updated guidance for the “Disable Catchup Full Scan” policy: because the setting name begins with “Disable,” Enabled turns off catch-up full scans and Disabled turns them on. Explained that a catch-up full scan runs after two missed scheduled full scans at next sign-in, requires a scheduled scan to be configured, and that Not configured uses the client default where catch-up full scans are disabled—reducing policy confusion.

  https://learn.microsoft.com/en-us/defender-endpoint/troubleshoot-mdav-scan-issues

- **Configure Microsoft Defender Antivirus using Microsoft Intune**

  Refined policy behavior for “Disable Catchup Full Scan” and “Disable Catchup Quick Scan”: Enabled disables catch-up scans and Disabled enables them. Documented defaults for Not configured (full-scan catch-up disabled by default; quick-scan catch-up enabled by default), when catch-up scans trigger (sign-in for full scans; power on/resume for quick scans), and that a scheduled scan must exist—helping ensure predictable scan behavior.

  https://learn.microsoft.com/en-us/defender-endpoint/use-intune-config-manager-microsoft-defender-antivirus