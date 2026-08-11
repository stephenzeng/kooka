# Microsoft Defender for Endpoint
**Date created:** 2026-08-06 UTC  
**Tags:** Security  

## Moderate Changes

- **Configure offline security intelligence updates for Microsoft Defender for Endpoint on Linux**

  Deprecated the legacy offlineDefinitionUpdateVerifySig setting and updated configuration examples accordingly. Clarified that the antivirus engine’s digital signature is verified by default starting with version 101.26062.0005, and provided commands to check the verification state via mdatp health. Updated verification and troubleshooting guidance to use the new engine_signature_verification indicator.

  https://learn.microsoft.com/en-us/defender-endpoint/linux-support-offline-security-intelligence-update

- **Microsoft Defender for Endpoint release notes**

  Added new entries for the Windows Antivirus July 2026 and Linux August 2026 releases, including supported components and support phases. Improved performance and reliability with faster archive scanning via dynamic memory scaling and better cache builds on Lunar Lake CPUs, plus fixes for slow on-demand scans. Enhanced quality and protection by enabling default engine signature verification on Linux, preventing resubmission of excluded files, resolving HTTPS stalls in Network Protection Block mode, and correcting health reporting after offboarding.

  https://learn.microsoft.com/en-us/defender-endpoint/microsoft-defender-endpoint-releases