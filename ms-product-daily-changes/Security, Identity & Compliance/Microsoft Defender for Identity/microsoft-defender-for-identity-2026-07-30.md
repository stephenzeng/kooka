# Microsoft Defender for Identity
**Date created:** 2026-07-30 UTC  
**Tags:** Administration, Security  

## Moderate Changes

- **Configure a gMSA directory service account for Defender for Identity**

  Updated guidance for multi-domain and multi-forest deployments with two supported patterns: a per-domain gMSA with Domain Local groups, or a shared gMSA paired with a Universal group at the forest root. Clarified that using a single gMSA at the forest root requires Enterprise Admin permissions and that the group scope should be Universal for cross-domain use. Content was reorganized for easier implementation.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/create-directory-service-account-gmsa

- **Microsoft Defender for Identity sensor v2.x prerequisites | Microsoft Defender for Identity**

  Clarified that CPU, RAM, and disk requirements are in addition to the resources consumed by the OS and domain controller services, helping avoid undersizing. Retained core sizing values and RODC support while removing platform phrasing that could be misconstrued.

  https://learn.microsoft.com/en-us/defender-for-identity/deploy/prerequisites-sensor-version-2

- **Defender for Identity VPN integration in Microsoft Defender**

  Updated product names and navigation text from “Microsoft Defender XDR” to “Microsoft Defender” to align with current portal terminology. No functional or procedural changes were made.

  https://learn.microsoft.com/en-us/defender-for-identity/vpn-integration