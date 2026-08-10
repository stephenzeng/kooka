# Microsoft Intune
**Date created:** 2026-07-16 UTC  
**Tags:** Administration, Security  

## Major Changes

- **Create discovery scripts for custom compliance policy in Microsoft Intune**

  Added macOS support for custom compliance discovery scripts, bringing cross-platform parity. Clarified macOS scripting requirements, including Bash with a shebang, UTF-8 encoding, exit code behavior, and a 10-minute runtime limit, and provided a sample script. Updated admin center guidance with macOS options such as running as the logged-on user, enforcing signatures, and hiding notifications, while revising Windows-only configuration details to avoid confusion.

  https://learn.microsoft.com/en-us/intune/device-security/compliance/create-custom-script

## Moderate Changes

- **Use custom compliance settings in Microsoft Intune**

  Expanded custom compliance support to macOS and clarified script requirements: PowerShell for Windows and POSIX-compliant shell scripts for Linux and macOS. Reporting guidance now highlights per-setting compliance details across Windows, Linux, and macOS, and includes macOS user remediation via Company Portal. Removed outdated details about Microsoft Entra join/registration and WPJ script behavior to streamline guidance.

  https://learn.microsoft.com/en-us/intune/device-security/compliance/custom-settings

- **Create a compliance policy in Microsoft Intune**

  Added macOS to the supported platforms for custom compliance settings and updated the procedure to “For Linux and macOS.” Instructions were generalized to select the discovery script and rules JSON without Linux-only references, simplifying cross-platform setup.

  https://learn.microsoft.com/en-us/intune/device-security/compliance/create-policy

- **Use compliance policies to set rules for devices you manage with Intune**

  Updated the supported platforms list to include macOS for custom compliance settings. Clarified Linux coverage by listing Ubuntu Desktop (24.04 LTS, 26.04 LTS) and Red Hat Enterprise Linux (9, 10), keeping Windows unchanged for completeness.

  https://learn.microsoft.com/en-us/intune/device-security/compliance/overview

- **Custom compliance JSON files for Microsoft Intune**

  Added macOS support for using a custom JSON file in device compliance policies. This broadens coverage so organizations can apply consistent custom checks across Windows, Linux, and macOS.

  https://learn.microsoft.com/en-us/intune/device-security/compliance/create-custom-json