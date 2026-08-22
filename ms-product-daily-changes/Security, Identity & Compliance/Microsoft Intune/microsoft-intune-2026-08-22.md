# Microsoft Intune
**Date created:** 2026-08-22 UTC  
**Tags:** Configuration, Guidance, Security  

## Moderate Changes

- **Windows Antivirus policy settings for Microsoft Defender Antivirus for Intune**
  
  Updated guidance clarifies that settings prefixed with “Disable” use Yes to disable and No to enable catch-up scans. Defaults are corrected: catch-up full scans follow the client default to be disabled, while catch-up quick scans default to enabled. The article also specifies when catch-up scans occur (after two missed scheduled scans, at next sign-in or power/resume) and that a scheduled scan must be configured for catch-up to run.
  
  https://learn.microsoft.com/en-us/intune/device-configuration/endpoint-security/ref-antivirus-defender-settings-windows

- **Windows Antivirus policy settings from Microsoft Defender Antivirus for tenant attached devices**
  
  Clarifies the semantics of the “Disable Catch-up Full Scan” and “Disable Catchup Quick Scan” options, emphasizing that Yes disables and No enables the respective catch-up behavior. Documents the default behaviors (full scan catch-up defaulted to disabled; quick scan catch-up defaulted to enabled) and outlines the conditions that trigger catch-up after missed schedules at next sign-in or power/resume, requiring a scheduled scan to be configured.
  
  https://learn.microsoft.com/en-us/intune/device-configuration/endpoint-security/ref-antivirus-defender-settings-windows-tenant-attach