# Microsoft Teams
**Change date:** 2026-08-07 UTC  
**Tags:** Administration, Governance, Security  

## New Articles

- **Collaborate with guests from other Microsoft 365 cloud environments**

  Introduced a step-by-step guide for enabling cross-cloud guest collaboration in Microsoft 365/Teams, including prerequisites and network readiness. The article walks through configuring cross-tenant connections and B2B collaboration settings in Microsoft Entra ID and adding external organizations. It details key limitations (for example, no connections between Azure Government and Azure China, and cross-cloud requires B2B guest rather than B2B member) and VDI support differences (SlimCore supported, WebRTC not supported). It also provides tips for finding tenant IDs and links to environment-specific endpoint requirements and related configuration guidance.

  https://learn.microsoft.com/en-us/microsoftteams/collaborate-guests-cross-cloud

## Major Changes

- **Limits and specifications for Microsoft Teams**

  Increased the private channel member limit from 250 to 5,000 to accommodate larger, more flexible collaboration. Removed the separate cap of 30 private channels per team and clarified that all channel types collectively count toward the existing 1,000 channels per team limit. Updated footnotes to state any combination of standard, private, and shared channels can total up to 1,000, simplifying capacity planning.

  https://learn.microsoft.com/en-us/microsoftteams/limits-specifications-teams

## Moderate Changes

- **Transitioning Teams Android Device Management from Teams Admin Center to the Teams Rooms Pro Management Portal**

  Expanded FAQs to outline the phased deprecation of device management in the Teams Admin Center through September 2026 and the move to the Teams Rooms Pro Management Portal (PMP). Clarified PMP benefits (unified device management, proactive incident handling, granular RBAC, update rings) and prerequisites, and explained how to import existing configuration profiles as Settings Templates; confirmed the PMP URL remains unchanged for now.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/aboutunifieddevicemanagement-pmp1

- **Teams Rooms on Android certified devices**

  Added new GCCH-certified entries for AudioCodes devices (RXV81, RX-Pad, RXV200) with current and minimum firmware and app versions, effective August 7, 2026. This helps government customers validate supported devices and plan firmware alignment.

  https://learn.microsoft.com/en-us/microsoftteams/devices/certified-hardware-android

- **Transition to Password-less Teams Shared Space device Resource Accounts**

  Documented a known issue where Crestron Teams Rooms on Windows devices are not compatible with password-less resource accounts and may require factory reset with continued password-based sign-in. Clarified that password-less credentials are lost on reset or reimage and provided updated guidance for device replacement and re-migration steps using a passworded account first.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/passwordlessentraresourceaccounts

- **Set as a Resource Accounts for Shared Devices in Teams Rooms Pro Management**

  Updated the benefits to note that resource accounts are removed from meeting chats after a call ends, reducing post-meeting exposure. Refined how Microsoft 365 distinguishes resource accounts and removed redundant guidance for greater clarity.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/set-as-resource-account-for-shared-teams-devices