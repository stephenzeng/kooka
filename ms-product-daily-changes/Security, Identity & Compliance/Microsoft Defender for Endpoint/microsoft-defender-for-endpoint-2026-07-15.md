# Microsoft Defender for Endpoint
**Date created:** 2026-07-15 UTC  
**Tags:** Administration, Security  

## Moderate Changes

- **Test your attack surface reduction (ASR) rules deployment**

  Updated planning and testing guidance by defining a small pilot “ring 1,” clarifying prerequisites, and noting that Plan 2 surfaces ASR recommendations via Defender Vulnerability Management. Expanded the review phase with plan-specific reporting options: ASR rules report and device timeline (Plan 2 or Defender for Business), Advanced hunting (Plan 2), and Windows Event Viewer (any plan). These clarifications help teams roll out ASR rules safely and measure impact with the right tools.

  https://learn.microsoft.com/en-us/defender-endpoint/attack-surface-reduction-rules-deployment-test

- **Turn on block at first sight**

  Expanded instructions for enabling and managing the feature via Intune and Group Policy, including precise navigation, configuration values (including hex options), and important notes about prompting and sample submission behavior. Added clearer steps for turning the feature off without altering prerequisite policies, and refined explanations of how it works. These updates help administrators configure the setting consistently and avoid unintended prompts or data collection gaps.

  https://learn.microsoft.com/en-us/defender-endpoint/configure-block-at-first-sight-microsoft-defender-antivirus

- **Microsoft Defender for Endpoint release notes**

  Added the Windows Antivirus June 2026 release with platform version 4.18.26060.3008, engine 1.1.26060.3008, and security intelligence 1.455.25.0. The update fixes repeated Controlled Folder Access notifications from AMD driver injection, improves Endpoint DLP enforcement for Chrome uploads to Google Drive, resolves timing issues with custom JIT notifications in Chrome and Firefox, and addresses CVE-2026-50656. These changes improve stability, user experience, and security.

  https://learn.microsoft.com/en-us/defender-endpoint/microsoft-defender-endpoint-releases