# Microsoft Defender for Endpoint
**Date created:** 2026-07-17 UTC  
**Tags:** Security  

## Major Changes

- **Deploy Microsoft Defender endpoint security to Linux devices using the Defender deployment tool (preview)**

  Expanded deployment guidance with a new monitoring section in the Defender portal, including a stepwise event timeline and two advanced hunting KQL queries for device-level and fleet-wide status. Updated prerequisites to reference the required Defender build version and clarified the health check command, and refined onboarding to explicitly select Linux and the correct Download package path. Enhanced deployment scenarios by replacing the non-blocking check with a full --pre-req check, adding support for using a locally configured package repository (--use-local-repo), and clarifying channel usage. Consolidated troubleshooting into a single section with log locations and step-specific guidance across Download, Prerequisite check, Installation, and Sensor initialization, with references to deeper diagnostics. Minor terminology updates align connectivity/verification wording to Microsoft Defender XDR.

  https://learn.microsoft.com/en-us/defender-endpoint/linux-install-with-defender-deployment-tool