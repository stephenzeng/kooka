# Microsoft Purview
**Date created:** 2026-09-03 UTC  
**Tags:** Analytics, Configuration, Deprecation, Guidance, Monitoring, Security, Troubleshooting  

## Major Changes

- **Data risk graph in Data Security Investigations**

  Announced deprecation of the Data risk graph (Explore insights) in Microsoft Purview Data Security Investigations. Configuration will be disabled starting September 30, 2026, and the feature will be fully retired on November 30, 2026. Plan to transition investigations and reporting to alternative experiences before retirement to avoid gaps in visibility.

  https://learn.microsoft.com/en-us/purview/data-security-investigations-data-risk-graph

- **Always-on diagnostics for endpoint DLP**

  Expanded Always-on diagnostics to support macOS in addition to Windows, including prerequisites for Intune, JAMF Pro, and other MDMs. Added supported macOS version guidance (latest three releases; build 101.26042.xxxx+ required) and clarified processor support (x64 and Apple Silicon). Updated workflows, role terminology, and storage guidance to reflect cross-platform enablement, improving troubleshooting consistency across endpoints.

  https://learn.microsoft.com/en-us/purview/dlp-always-on-diagnostics

- **Install the AIPService PowerShell module for the Azure Rights Management service**

  Updated prerequisites to support both Windows PowerShell 5.1 and PowerShell 7.4+ (AIPService 3.1.0.0 or later), and clarified .NET requirements. Introduced a PowerShell editions section explaining dual Desktop/Core support from a single package, authentication differences, and how to verify CompatiblePSEditions. Noted separate per-user module folders and the need to install from a PowerShell 7 session when targeting PowerShell 7, streamlining setup across environments.

  https://learn.microsoft.com/en-us/purview/install-aipservice-powershell

## Moderate Changes

- **Automatically apply a sensitivity label to Microsoft 365 data**

  Clarified that policy-level labeling progress, Insights enforcement metrics, and the Labeled items view report only on SharePoint and OneDrive files and exclude Exchange email. Advised using Activity explorer to verify Exchange email labeling, with a 60–90 minute delay before events appear. Explained that Content explorer is a snapshot that may take up to seven days to reflect counts and doesn’t show which policy applied a label, making Activity explorer the preferred source for recent activity.

  https://learn.microsoft.com/en-us/purview/apply-sensitivity-label-automatically

- **Use the Insights tab to analyze auto-labeling policies in Microsoft Purview**

  Clarified that Insights enforcement metrics and the Labeled items view exclude Exchange email; only SharePoint and OneDrive files are included. Recommended using Activity explorer to validate Exchange email labeling and noted a 60–90 minute ingestion delay.

  https://learn.microsoft.com/en-us/purview/auto-label-insights-tab

- **Microsoft Purview Information Protection client - Release management and supportability**

  Added preview releases: Windows client/scanner 3.2.170.0 with fixes for sign-in reset, PowerShell cmdlet behavior, offline state, connectivity/policy retrieval, classification bar sublabel paths, Windows 11 context menu reliability, Activity Explorer audit entries for .xlsx, custom permissions, and security updates; and macOS client 1.0.125 with an updated authentication library, accessibility improvements, and security fixes. Updated the lifecycle table to mark versions 3.1.310.0 and 3.1.251.0 as retired, guiding administrators to supported builds.

  https://learn.microsoft.com/en-us/purview/information-protection-client-relnotes

- **Bring your own key for the Azure Rights Management service root key**

  Updated BYOK guidance to confirm the AIPService module runs on PowerShell 7.4+ when using version 3.1.0.0 or later, in addition to Windows PowerShell 5.1. This clarifies prerequisites and procedural notes for modern PowerShell environments.

  https://learn.microsoft.com/en-us/purview/rights-management-byok