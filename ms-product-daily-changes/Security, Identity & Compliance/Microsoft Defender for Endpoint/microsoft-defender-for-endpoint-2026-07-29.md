# Microsoft Defender for Endpoint
**Date created:** 2026-07-29 UTC  
**Tags:** Administration, Security  

## Moderate Changes

- **Overview of Microsoft Defender for Endpoint Plan 1**
  Added licensing guidance detailing availability of Plan 1 as a standalone subscription or via Microsoft 365 E3, with separate server licensing and potential discounts when combined with Microsoft Defender for Servers. This helps administrators choose the right licensing and optimize costs with clear references to related documentation.
  https://learn.microsoft.com/en-us/defender-endpoint/defender-endpoint-plan-1

- **Device control policies in Microsoft Defender for Endpoint**
  Clarified that the ComputerSid policy field supports Microsoft Entra group object IDs only, and does not support device object IDs. This ensures accurate targeting of device control policies and reduces configuration errors.
  https://learn.microsoft.com/en-us/defender-endpoint/device-control-policies

- **Create an app to access Microsoft Defender for Endpoint without a user**
  Expanded step-by-step guidance for app-only access, including app registration, granting permissions, and acquiring tokens via the OAuth 2.0 client credentials flow. Added clearer explanations for multi-tenant consent, token contents, validation steps, and applying bearer tokens in API requests to streamline setup and reduce authentication issues.
  https://learn.microsoft.com/en-us/defender-endpoint/api/exposed-apis-create-app-webapp

- **Investigate entities on devices using live response**
  Clarified a 5 MB default library size limit in US Government clouds with guidance to request higher limits. Updated background file retrieval to use “getfile <file_path> &” and corrected the “-auto” flag syntax to prevent command errors. These changes improve reliability and accuracy for live response operations.
  https://learn.microsoft.com/en-us/defender-endpoint/live-response

- **Microsoft Defender for Endpoint overview**
  Added a server licensing section explaining discount eligibility when Defender for Endpoint on servers is used with Microsoft Defender for Servers, with links to overviews and FAQs. This helps customers understand cost implications and licensing options for server workloads.
  https://learn.microsoft.com/en-us/defender-endpoint/microsoft-defender-endpoint

- **Microsoft Defender for Endpoint release notes**
  Added the macOS July 2026 release (101.26062.0009) with bug/performance fixes and expanded diagnostics via “mdatp health --details network_configuration.” Introduced a Linux note on a nine‑month product version expiration policy, how to check expiration, and confirmed the end of the RHEL 6 exception. These updates help admins plan upgrades and leverage improved diagnostics.
  https://learn.microsoft.com/en-us/defender-endpoint/microsoft-defender-endpoint-releases

- **Submit or Update Indicator API**
  Corrected request schema by changing rbacGroupNames to String[] and generateAlert to Boolean. This aligns client payloads with expected types and prevents API validation issues.
  https://learn.microsoft.com/en-us/defender-endpoint/api/post-ti-indicator

- **Advanced hunting API**
  Added a deprecation warning and migration guidance to the Microsoft Graph security API, citing benefits like broader data coverage and improved consistency. Retirement began in January 2026, and the API will stop working after retirement completes; links to timeline and migration resources are included to help teams transition promptly.
  https://learn.microsoft.com/en-us/defender-endpoint/api/run-advanced-query-api

- **Run live response commands on a device**
  Updated the example response code from 200 OK to 201 Created to reflect resource creation on success. This sets accurate expectations for integrations and monitoring logic.
  https://learn.microsoft.com/en-us/defender-endpoint/api/run-live-response

- **Microsoft Defender for Endpoint standard connectivity URLs - commercial**
  Adjusted a table entry to mark the Microsoft Office CDN product updates (ChannelURL) as Mac-only rather than Common (Mac/Linux), updating requirement indicators accordingly. This ensures accurate allowlist and connectivity planning for macOS environments.
  https://learn.microsoft.com/en-us/defender-endpoint/standard-device-connectivity-urls-commercial

- **New features in Microsoft Defender for Endpoint**
  Updated the July 2026 section and added a new macOS release entry (Build 101.26062.0009, GA) with a link to details. This keeps customers informed about current platform updates while retaining existing iOS and AI agent runtime protection items.
  https://learn.microsoft.com/en-us/defender-endpoint/whats-new-in-microsoft-defender-endpoint