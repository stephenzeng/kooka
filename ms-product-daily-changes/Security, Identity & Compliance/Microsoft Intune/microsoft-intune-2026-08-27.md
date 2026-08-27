# Microsoft Intune
**Date created:** 2026-08-27 UTC  
**Tags:** Analytics, Configuration, Guidance, Monitoring, Security, Troubleshooting  

## New Articles

- **App Settings Configuration for Apple Devices - Microsoft Intune | Microsoft Learn**

  Introduced guidance for configuring Apple Declarative Device Management (DDM) App Settings via the Intune settings catalog, with support for supervised iOS/iPadOS 27+ and macOS 27+. Documented iOS/iPadOS app launch controls (allow/deny lists) and macOS binary execution controls, including required identifiers and reliance on the Endpoint Security framework. Clarified precedence rules, critical system allowances, and that deny rules do not block app installation. Advised migrating from legacy iOS Restrictions keys deprecated in iOS 27 and outlined monitoring via the DDM status channel.

  https://learn.microsoft.com/en-us/intune/device-configuration/templates/apple-ddm-app-settings

## Major Changes

- **View device details with Microsoft Intune**

  Expanded Android Enterprise corporate-owned inventory details, especially for Android 15, to capture multi-IMEI, multi-ICCID, per-SIM phone numbers, and carrier names. Added new reported fields for each eSIM: Activation state and SIM origin, and clarified reporting differences by management mode (COBO, COSU, COPE) and OS version. Replaced legacy notes with precise behavior and referenced the Remove eSIM action to help identify the correct ICCID for management.

  https://learn.microsoft.com/en-us/intune/device-management/inventory-and-status/device-details

- **Review Android settings catalog settings in Microsoft Intune**

  Added new Android settings, including the ability to set how many days a work profile can be switched off (COPE) and an option to remove all eSIMs during a device wipe (Android 15+ for COBO, COSU, COPE). Introduced a Power section with screen timeout controls and options to keep the screen on while plugged in, with applicability by ownership model and OS version. Added a password setting to block using one lock for both device and work profile, enforcing separate locks.

  https://learn.microsoft.com/en-us/intune/device-configuration/settings-catalog/ref-android-settings

- **Manage eSIM plans in Microsoft Intune**

  Expanded from iOS-only activation to managing eSIM plans on both Apple and Android Enterprise devices, including activating an eSIM and removing an eSIM from a single device. Added prerequisites, RBAC requirements, and a support matrix across COBO, COSU, and COPE with Android version requirements. Provided step-by-step procedures, guidance on using the new device view, and instructions for supplying ICCID from hardware inventory for Android eSIM removal, plus notes on user experience and handling activation errors.

  https://learn.microsoft.com/en-us/intune/device-management/actions/update-cellular-data-plan

## Moderate Changes

- **Intune data platform schema**

  Added Android Enterprise personally owned work profile (BYOD with Android Management API) to supported platforms and clarified unsupported/limited entities on BYOD (for example, BiosInfo, SimInfo, and partial NetworkAdapter fields). Expanded supported platforms and properties, including DeviceStorage support for Inventory, Android support for SystemInfo, and new HardwareSerialNumber for Android.

  https://learn.microsoft.com/en-us/intune/advanced-analytics/ref-data-platform-schema

- **Set up automated device enrollment for iOS/iPadOS**

  Expanded the Setup Assistant screens table to include Accessibility appearance (iOS/iPadOS 17.0+) and Liquid glass (iOS/iPadOS 27.0+). This helps admins plan enrollment flows aligned with the latest OS experiences.

  https://learn.microsoft.com/en-us/intune/device-enrollment/apple/setup-automated-ios

- **Set up automated device enrollment for macOS**

  Added a new Setup Assistant entry describing the Liquid Glass pane for macOS 27.0 and later. This update helps admins anticipate enrollment screens and user experience changes.

  https://learn.microsoft.com/en-us/intune/device-enrollment/apple/setup-automated-macos

- **Wipe devices with Microsoft Intune**

  Added Android-specific guidance to choose whether to remove eSIMs during a single-device wipe from the new device view, clarifying that COBO, COSU, and COPE preserve eSIMs by default. Retitled and expanded the overview to better support device retirement, reuse, and recovery workflows.

  https://learn.microsoft.com/en-us/intune/device-management/actions/wipe