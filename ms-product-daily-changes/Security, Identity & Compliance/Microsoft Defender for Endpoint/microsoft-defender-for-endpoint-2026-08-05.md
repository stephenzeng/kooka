# Microsoft Defender for Endpoint
**Date created:** 2026-08-05 UTC  
**Tags:** Administration, Security  

## Moderate Changes

- **Attack surface reduction (ASR) rules overview**

  Added an important requirement that using Unblock to override an ASR rule in Warn mode now needs administrator approval starting with platform version 4.18.26060. Clarified that Unblock is only for temporary suppression and advised using per-rule exclusions for ongoing needs.

  https://learn.microsoft.com/en-us/defender-endpoint/attack-surface-reduction-rules-overview

- **Test controlled folder access with an untrusted app**

  Highlighted that the demo script adds c:\demo to Defender Antivirus exclusions, which can prevent expected CFA blocks, and updated steps to run CFAtool.exe from a non-excluded folder. Elevated the guidance to an important warning and clarified that extra downloaded test files aren’t used in this scenario.

  https://learn.microsoft.com/en-us/defender-endpoint/defender-endpoint-demonstration-controlled-folder-access-block-app

- **View and organize the Microsoft Defender for Endpoint Incidents queue**

  Updated the default Incidents queue time range from the last six months to the last week. This change focuses the view on more recent activity by default for faster triage.

  https://learn.microsoft.com/en-us/defender-endpoint/view-incidents-queue