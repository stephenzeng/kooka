# Microsoft Intune
**Date created:** 2026-07-23 UTC  
**Tags:** Administration, Security  

## Moderate Changes

- **Intune App SDK for Android - MAM Integration Essentials**

  Expanded guidance on the WRONG_USER enrollment outcome, outlining two user remediation choices and their effects. Clarifies that removing the attempted account unregisters it locally without a selective wipe, reports UNENROLLMENT_SUCCEEDED, and stops retries for that account; if the second account remains registered, MAM continues periodic enrollment attempts.

  https://learn.microsoft.com/en-us/intune/developer/app-sdk/android-phase-4

- **Configure pre-cache content**

  Updated deployment guidance to advise against using “Download all content locally before starting task sequence” for OS image installations. This prevents task sequence failures when a disk wipe removes the client cache.

  https://learn.microsoft.com/en-us/intune/configmgr/osd/deploy-use/configure-precache-content

- **China endpoints for Microsoft Intune**

  Added the Experimentation and Configuration Service (ECS) endpoint pattern (*.ecs.gov.teams.microsoft.us) for Intune operated by 21Vianet. This ensures admins allow required connectivity for service functionality in China.

  https://learn.microsoft.com/en-us/intune/fundamentals/endpoints-china

- **US government endpoints for Microsoft Intune**

  Added the Experimentation and Configuration Service (ECS) endpoint pattern (*.ecs.gov.teams.microsoft.us) to the US Government cloud endpoints. This helps ensure required service connectivity in government environments.

  https://learn.microsoft.com/en-us/intune/fundamentals/endpoints-us-government

- **What's new in Microsoft Intune**

  Added a Week of July 13, 2026 item announcing support for multiple managed accounts in Microsoft Outlook for iOS/iPadOS (v5.2626.0+). The entry notes a gradual rollout and links to detailed guidance for configuring app protection policies.

  https://learn.microsoft.com/en-us/intune/whats-new/

- **Android template device settings list to restrict features using Intune**

  Corrected the COPE comparison table to show that Factory data reset does not provide factory reset protection. This helps admins set accurate expectations and plan reset scenarios appropriately.

  https://learn.microsoft.com/en-us/intune/device-configuration/templates/ref-device-restrictions-android-enterprise

- **Device compliance settings for macOS in Intune**

  Added a warning that enforcing a password via compliance policy immediately expires existing passwords for all device accounts, including LAPS and Platform SSO. Recommends managing device passwords with a settings catalog policy and setting Change At Next Auth to False to avoid unintended password expirations.

  https://learn.microsoft.com/en-us/intune/device-security/compliance/ref-macos-settings

- **Set up automated device enrollment for tvOS**

  Introduced a Setup Assistant screen reference detailing which tvOS enrollment screens can be shown or hidden and their minimum OS versions. This improves planning for user experience during automated device enrollment.

  https://learn.microsoft.com/en-us/intune/device-enrollment/apple/setup-automated-tv-os

- **Set up automated device enrollment for visionOS**

  Added a Setup Assistant screen reference for visionOS 26+, outlining available enrollment screens and whether they can be shown or hidden. This helps admins standardize and streamline the visionOS enrollment experience.

  https://learn.microsoft.com/en-us/intune/device-enrollment/apple/setup-automated-vision-os