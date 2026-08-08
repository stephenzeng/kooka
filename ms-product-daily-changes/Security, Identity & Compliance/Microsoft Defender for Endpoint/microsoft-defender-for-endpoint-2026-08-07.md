# Microsoft Defender for Endpoint
**Change date:** 2026-08-07 UTC  
**Tags:** AI, Administration, Monitoring, Security  

## Major Changes

- **Discover local AI agents with Microsoft Defender for Endpoint (Preview)**

  Overhauled prerequisites/licensing references and substantially reworked the KQL guidance. The query logic was reorganized to improve how criticality and sensitive data are handled and to shift the analysis and outputs for clearer exposure insights. These updates help security teams focus investigations and interpret results more reliably.

  https://learn.microsoft.com/en-us/defender-endpoint/discover-local-ai-agents

- **Microsoft Defender for Endpoint release notes**

  Added new release entries across platforms and expanded details for July/August 2026. Highlights include Linux fixes for on-demand scan responsiveness and signature verification defaults, macOS updates with extended network diagnostics, and Windows AV improvements for archive scanning, cache builds on newer CPUs, and HTTPS stability under Network Protection. Android and iOS entries include performance and reliability fixes. The summary table and platform sections were updated to reflect the latest versions and changes.

  https://learn.microsoft.com/en-us/defender-endpoint/microsoft-defender-endpoint-releases

## Moderate Changes

- **Deploy Microsoft Defender endpoint security to Windows devices using the Defender deployment tool**

  Updated instructions to rename the configuration file from DefenderDTconfig.txt to MdeConfig.txt/MDEConfig.txt across examples and Group Policy steps. Clarifies when full paths are required to prevent deployment errors.

  https://learn.microsoft.com/en-us/defender-endpoint/defender-deployment-tool-windows

- **Test controlled folder access with an untrusted app**

  Revised the test procedure and notes to ensure CFA blocks and detections occur as expected, clarifying where to run the tool to avoid antivirus exclusions. The article title was updated to better reflect the test scenario.

  https://learn.microsoft.com/en-us/defender-endpoint/defender-endpoint-demonstration-controlled-folder-access-block-app

- **Overview of Microsoft Defender for Endpoint Plan 1**

  Updated the Licensing section to clarify availability (standalone and via Microsoft 365 E3), server licensing for Plan 1, and potential discounts when combined with Defender for Servers in Defender for Cloud. Cross-references were added for easier navigation.

  https://learn.microsoft.com/en-us/defender-endpoint/defender-endpoint-plan-1

- **Manage endpoint security policies in Microsoft Defender for Endpoint**

  Clarified that Endpoint security policy management isn’t supported on devices using the Microsoft Monitoring Agent (MMA) sensor and advised upgrading with the Defender deployment tool. Also specified that only Microsoft Defender Antivirus policy is supported on Windows 7 SP1 and Windows Server 2008 R2 SP1.

  https://learn.microsoft.com/en-us/defender-endpoint/endpoint-security-policies-configure

- **Get vulnerability by ID**

  Refreshed the example API response to use a different CVE and adjusted severity and metrics accordingly. The sample payload was streamlined by removing several fields and updating dates and counts to reflect the new example.

  https://learn.microsoft.com/en-us/defender-endpoint/api/get-vulnerability-by-id

- **Create indicators for IPs and URLs/domains**

  Added an IMPORTANT note that indicator policy propagation can take up to 48 hours, though most changes apply within two hours. This helps set operational expectations when creating or updating indicators.

  https://learn.microsoft.com/en-us/defender-endpoint/indicator-ip-domain

- **Manage event-based forced updates**

  Corrected the PowerShell example for pre-scan signature checks to use the cmdlet switch without an explicit value, reflecting accurate Set-MpPreference usage. This prevents configuration errors in automation scripts.

  https://learn.microsoft.com/en-us/defender-endpoint/manage-event-based-updates-microsoft-defender-antivirus

- **Manage tamper protection for your organization using Microsoft Intune**

  Removed a caution about editing registry keys when viewing tamper protection status. Clarified that registry changes don’t affect whether tamper protection applies to exclusions, reducing confusion during troubleshooting.

  https://learn.microsoft.com/en-us/defender-endpoint/manage-tamper-protection-intune

- **Microsoft Defender Antivirus production ring deployment using Group Policy and network share**

  Updated the Group Policy instruction to select “Define file shares for downloading security intelligence updates,” aligning text and alt text with the correct setting. This reduces misconfiguration when using file shares as update sources.

  https://learn.microsoft.com/en-us/defender-endpoint/microsoft-defender-antivirus-ring-deployment-group-policy-network-share

- **Phishing trends and techniques**

  Added coverage for QR code (quishing) and CAPTCHA-gated phishing, and expanded download-based lures to include more attachment types and multistage flows. Modernized spear phishing guidance to emphasize credential theft and malware-enabled remote control.

  https://learn.microsoft.com/en-us/defender-endpoint/malware/phishing-trends

- **Run the client analyzer on Linux**

  Expanded guidance for running the XMDE Client Analyzer when Defender is installed, providing two paths with ready-to-use scripts (binary and Python). Includes script contents and example commands to streamline Live Response execution.

  https://learn.microsoft.com/en-us/defender-endpoint/run-analyzer-linux

- **Use Microsoft Intune to configure and manage Microsoft Defender Antivirus**

  Updated guidance for SignatureUpdateFallbackOrder to use a pipe-separated string that defines the update source order. Clarifies valid values and simplifies configuration via Intune.

  https://learn.microsoft.com/en-us/defender-endpoint/use-intune-config-manager-microsoft-defender-antivirus

- **New features in Microsoft Defender for Endpoint**

  Updated the July 2026 section with a macOS GA release (Build 101.26062.0009) and introduced the Defender Deployment Tool for Linux. The new tool simplifies Linux deployment and management, supports custom paths and channel/version selection, validates prerequisites, and improves visibility via Device Timeline and Advanced Hunting.

  https://learn.microsoft.com/en-us/defender-endpoint/whats-new-in-microsoft-defender-endpoint