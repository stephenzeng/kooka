# Microsoft Defender for Endpoint
**Date created:** 2026-08-28 UTC  
**Tags:** Configuration, Guidance, Security  

## Major Changes

- **Configure Microsoft Defender for Endpoint on Android**

  Significantly expanded configuration guidance, introducing a consolidated Intune app configuration policy workflow with detailed keys and values for network protection, privacy, device tagging, and user controls. Clarified privacy options (for example, hiding URLs and app details) and noted they don’t affect compliance or Conditional Access, plus added a May 2025 behavioral change that shifts certain Wi‑Fi and certificate activities from alerts to device timeline events. Added new capabilities, including [Preview] non‑APK file scanning and a TVM privacy control for BYOD app inventory, and provided an option to hide the in‑app sign‑out button. Improved instructions for device tagging and clarified that web protection uses a local loopback VPN, with refined guidance and limitations for custom indicators.

  https://learn.microsoft.com/en-us/defender-endpoint/android-configure

## Moderate Changes

- **Configure the Microsoft Defender Antivirus cloud block time-out period**

  Updated guidance clarifies the default 10‑second cloud block time‑out, with up to 50 additional seconds (maximum 60), and outlines required prerequisites and licensing considerations. Configuration steps were refreshed across Intune, Microsoft Defender portal endpoint security policies, and Group Policy (allowed range now 0–50), and a new PowerShell option (Set-MpPreference -CloudExtendedTimeout) was added. These updates help standardize deployment and ensure consistent behavior across Windows clients and servers.

  https://learn.microsoft.com/en-us/defender-endpoint/configure-cloud-block-timeout-period-microsoft-defender-antivirus