# Microsoft Defender for Endpoint
**Date created:** 2026-08-19 UTC  
**Tags:** Guidance, Security, Troubleshooting  

## Moderate Changes

- **Attack surface reduction (ASR) rule demonstrations**

  Updated the demo to highlight that the setup adds c:\demo to antivirus exclusions and requires moving ASR test files to a non-excluded location before opening or running them. Steps were refined to avoid running tests from excluded paths and to add a cleanup task for any files copied outside c:\demo. These changes improve test accuracy and prevent false negatives when validating ASR rules.

  https://learn.microsoft.com/en-us/defender-endpoint/defender-endpoint-demonstration-attack-surface-reduction-rules

- **Demonstrate how controlled folder access (CFA) blocks ransomware**

  Strengthened guidance by elevating a warning about c:\demo being excluded from antivirus scanning and requiring the test executable to be run from a non-excluded folder. Clarified execution paths for both scripted and manual setups, including when CFA is disabled, and added a cleanup step for copied files. This ensures CFA behavior is measured correctly and avoids missed detections caused by exclusions.

  https://learn.microsoft.com/en-us/defender-endpoint/defender-endpoint-demonstration-controlled-folder-access-ransomware