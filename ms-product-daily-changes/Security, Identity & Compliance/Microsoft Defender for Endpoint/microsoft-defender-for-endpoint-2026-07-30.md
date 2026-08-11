# Microsoft Defender for Endpoint
**Date created:** 2026-07-30 UTC  
**Tags:** Administration, Analytics, Automation, Monitoring, Security  

## Major Changes

- **Address false positives/negatives in Microsoft Defender for Endpoint**

  Introduced comprehensive guidance for investigating and mitigating false negatives, including step-by-step use of device timeline and advanced hunting with sample Kusto queries. Added detailed evidence collection procedures and submission options via the Defender portal and Microsoft Security Intelligence. Provided mitigation steps using custom indicators while analysis is pending, and expanded health checks with PowerShell commands to verify engine/signature versions and key protection settings.

  https://learn.microsoft.com/en-us/defender-endpoint/defender-endpoint-false-positives-negatives

## Moderate Changes

- **Review and assess devices in Microsoft Defender for Endpoint**

  Added a prerequisites section and refined advanced hunting guidance, including clearer examples for network exploration and discovered devices. Clarified SeenBy usage, network event context, and provided a sample query to validate recent connection attempts.

  https://learn.microsoft.com/en-us/defender-endpoint/assess-devices

- **Onboarding devices using streamlined connectivity for Microsoft Defender for Endpoint**

  Clarified streamlined connectivity by listing the consolidated domains (*.endpoint.security.microsoft.com and *.endpoint.security.microsoft.us) and noting that OneDsCollector consolidation is URL-only. Emphasized separate configuration when using IP-based methods.

  https://learn.microsoft.com/en-us/defender-endpoint/configure-device-connectivity

- **Step 1: Configure your network environment for connectivity to the Defender for Endpoint service**

  Added SSL inspection requirements for streamlined connectivity and instructed bypassing inspection for *.endpoint.security.microsoft.com. Clarified IP-allowlist-only environments should permit Microsoft ranges via firewall or gateway devices.

  https://learn.microsoft.com/en-us/defender-endpoint/configure-environment

- **Configure and validate Microsoft Defender Antivirus network connections**

  Expanded troubleshooting for cloud connectivity validation with detailed ValidateMapsConnection behavior and sample error outputs. Highlighted missing WinHTTP proxy and CRL retrieval as common causes and recommended configuring a system-wide WinHTTP proxy or disabling SpyNet CRL checks as an alternative.

  https://learn.microsoft.com/en-us/defender-endpoint/configure-network-connections-microsoft-defender-antivirus

- **Configure device proxy connectivity to the Defender for Endpoint service**

  Clarified Group Policy locations for static proxy settings and explained the scope of the WinHTTP proxy. Refined procedures to set, verify, and remove WinHTTP proxy settings.

  https://learn.microsoft.com/en-us/defender-endpoint/configure-proxy-internet

- **Create and manage custom data collection rules in Microsoft Defender for Endpoint**

  Expanded overview of capturing targeted endpoint events beyond default telemetry and routing to Microsoft Sentinel. Clarified end-to-end lifecycle: create, edit, monitor, and delete rules.

  https://learn.microsoft.com/en-us/defender-endpoint/create-custom-data-collection-rules

- **Deploy Microsoft Defender endpoint security to Windows devices using the Defender deployment tool**

  Added a prerequisite emphasizing SSL inspection bypass requirements for streamlined connectivity. This helps prevent connectivity issues during deployment.

  https://learn.microsoft.com/en-us/defender-endpoint/defender-deployment-tool-windows

- **Microsoft Defender for Endpoint Exploit protection (EP) demonstrations**

  Added an Overview and expanded setup with clearer steps to apply, customize, and verify mitigations using XML and PowerShell. Improved scenario guidance for EMET conversion and self-hosted XML configurations, and retitled related links for clarity.

  https://learn.microsoft.com/en-us/defender-endpoint/defender-endpoint-demonstration-exploit-protection

- **Network protection demonstrations**

  Clarified enablement and verification steps across Windows and macOS/Linux, including enforcement levels, expected blocking behavior, and cleanup steps post-testing. Added explicit commands and status checks to validate outcomes.

  https://learn.microsoft.com/en-us/defender-endpoint/defender-endpoint-demonstration-network-protection

- **Turn on network protection**

  Listed supported deployment methods and added registry-based verification steps for enforcement and audit modes. Clarified Configuration Manager workflow and updated references for server configuration.

  https://learn.microsoft.com/en-us/defender-endpoint/enable-network-protection

- **Evaluate exploit protection**

  Clarified audit mode purpose and usage with updated headings and anchors. Added compatibility notes (EMET vs. Oracle Java with large heap sizes) and refined PowerShell examples for configuring and validating mitigations.

  https://learn.microsoft.com/en-us/defender-endpoint/evaluate-exploit-protection

- **Create indicators for IPs and URLs/domains**

  Added an Important note that indicator propagation can take up to 48 hours (typically under two). This sets expectations for enforcement timing across devices.

  https://learn.microsoft.com/en-us/defender-endpoint/indicator-ip-domain

- **Configure and validate exclusions for Microsoft Defender for Endpoint on Linux**

  Clarified exclusion configuration across console and CLI with explicit add/remove examples and wildcard usage. Improved output explanations and reorganized content with anchors and related content updates.

  https://learn.microsoft.com/en-us/defender-endpoint/linux-exclusions

- **Configure security settings in Microsoft Defender for Endpoint on Linux**

  Reworked configuration guidance with clearer dictionary details, verification steps, and unmonitoredFilesystems configuration examples. Added pre-deployment validation tips, including JSON syntax checks and tools for validation.

  https://learn.microsoft.com/en-us/defender-endpoint/linux-preferences

- **Schedule security intelligence updates for Microsoft Defender for Endpoint on Linux**

  Enhanced cron scheduling guidance with time zone handling (CRON_TZ), verification through logs, and safer management practices. Added context for using Ansible and Chef and warned about commands that remove all crontab entries.

  https://learn.microsoft.com/en-us/defender-endpoint/linux-update-mde-linux

- **Create and manage device groups in Microsoft Defender for Endpoint**

  Retitled and added an Overview, introduced prerequisites for Entra groups with RBAC, and clarified matching rules and propagation delays. Noted that Devices filters may lag after configuration changes.

  https://learn.microsoft.com/en-us/defender-endpoint/machine-groups

- **Set up the Microsoft Defender for Endpoint on macOS policies in Jamf Pro**

  Expanded end-to-end setup across required profiles and policies, distinguishing GUI and legacy methods. Clarified identifiers, bundle IDs, signing considerations, and deployment sequencing to avoid dependency issues.

  https://learn.microsoft.com/en-us/defender-endpoint/mac-jamfpro-policies

- **Set preferences for Microsoft Defender for Endpoint on macOS**

  Clarified admin-focused configuration via Jamf and Intune, expanded dictionary keys for exclusions and threat settings, and provided plist validation tips. Added cautions on preference domains and step-by-step Intune deployment guidance.

  https://learn.microsoft.com/en-us/defender-endpoint/mac-preferences

- **Configure offline security intelligence updates for Microsoft Defender for Endpoint on macOS**

  Added Overview and prerequisites, clarified mirror server and endpoint flows, and improved scripts and execution guidance. Enhanced verification and troubleshooting with expected outputs and diagnostic steps.

  https://learn.microsoft.com/en-us/defender-endpoint/mac-support-offline-security-intelligence-update

- **Manage system extensions using Jamf**

  Expanded guidance for approving system extensions, granting Full Disk Access, and configuring the network extension with validation steps. Included code requirements, corrected XML examples, and signing instructions for profiles.

  https://learn.microsoft.com/en-us/defender-endpoint/manage-sys-extensions-using-jamf

- **Microsoft Defender for Endpoint plug-in for Windows Subsystem for Linux (WSL)**

  Added purpose, prerequisites, and an installation validation checklist. Expanded troubleshooting for proxy, DNS, and networking configurations across Windows versions and improved support bundle generation steps.

  https://learn.microsoft.com/en-us/defender-endpoint/mde-plugin-wsl

- **Microsoft Defender for Endpoint release notes**

  Merged updates: adjusted macOS support to 14 (Sonoma) or newer and marked 13 (Ventura) as unsupported; updated Linux July 2026 release from 101.26052.0011 to .0012 with a new bug fix for WordPress Core visibility in software inventory. Anchor references and release version were updated accordingly.

  https://learn.microsoft.com/en-us/defender-endpoint/microsoft-defender-endpoint-releases

- **Microsoft Defender Offline scan in Windows**

  Clarified behavior and risks of Start-MpWDOScan, including immediate reboot into an isolated environment. Added warnings to save work, and refined WMI description and legacy OS boot media guidance.

  https://learn.microsoft.com/en-us/defender-endpoint/microsoft-defender-offline

- **Migrate devices to use the streamlined connectivity method**

  Restructured content for clarity across OS platforms, added anchors, and clarified restart requirements after onboarding. Enhanced Intune notes on policy application and expanded hunting guidance for ConnectivityType insights.

  https://learn.microsoft.com/en-us/defender-endpoint/migrate-devices-streamlined

- **Offboard machine API**

  Updated supported OS to include macOS 14+ and clarified that Linux is not supported. Added a reference to macOS release notes for alignment with platform support.

  https://learn.microsoft.com/en-us/defender-endpoint/api/offboard-machine-api

- **Microsoft Defender for Endpoint streamlined connectivity URLs - commercial**

  Expanded introduction and notes for devices with partial support, and clarified that static IP ranges do not replace other required services. Added guidance for alternatives like ConfigMgr/WSUS/file shares and ensuring supported OS/component levels.

  https://learn.microsoft.com/en-us/defender-endpoint/streamlined-device-connectivity-urls-commercial

- **Web content filtering in Microsoft Defender for Endpoint**

  Added operational guidance on policy propagation delays, audit-only deployments, removal latency, and cautions about blocking Uncategorized. Clarified prerequisites for subscription, OS, browser, and protection requirements.

  https://learn.microsoft.com/en-us/defender-endpoint/web-content-filtering

- **Web protection in Microsoft Defender for Endpoint**

  Added an introductory summary of capabilities, browser support, policy precedence, and hunting scope. Clarified advanced hunting examples for identifying SmartScreen web content filtering blocks.

  https://learn.microsoft.com/en-us/defender-endpoint/web-protection-overview