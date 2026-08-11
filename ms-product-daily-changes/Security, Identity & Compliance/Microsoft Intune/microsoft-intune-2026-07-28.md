# Microsoft Intune
**Date created:** 2026-07-28 UTC  
**Tags:** AI, Administration, Analytics, Governance, Monitoring, Security  

## Major Changes

- **Manage antivirus settings with endpoint security policies in Microsoft Intune**
  Introduced Controlled configuration for Microsoft Defender settings (preview), allowing Intune to become the authoritative source for Defender settings and override local, Group Policy, and Configuration Manager changes. Added guidance for enabling the feature via the Windows Security experience profile, with clear scope, exclusions, and behavior for non-configured settings. Updated reporting behavior and precedence handling, including Not applicable for overlapping settings and renaming the Tamper protection column to Controlled configuration in relevant reports.
  https://learn.microsoft.com/en-us/intune/device-configuration/endpoint-security/antivirus

- **Collect Device Properties With Intune Properties Catalog**
  Expanded from hardware-only to comprehensive Windows device property inventory, including configuration, registry keys, and security signals. Added prerequisites, category-to-required-property mapping (including Local AI Agent and Registry), and detailed policy creation, assignment, and check-in behavior. Introduced Local AI Agent discovery with mitigation guidance and registry inventory with collection methods, sensitivity filters, HKLM-only initial scope, and limits, plus steps to view data and stop collection per category. Included data retention details (28 days after deletion), troubleshooting guidance, and links to schema and device query documentation.
  https://learn.microsoft.com/en-us/intune/device-configuration/collect-device-properties

## Moderate Changes

- **Using Azure Virtual Desktop with Intune**
  Clarified that cross-cloud enrollments (public to sovereign) are not supported and provided concrete examples. Noted that Azure China and Azure Government instances cannot enroll into a Public Cloud Intune tenant.
  https://learn.microsoft.com/en-us/intune/solutions/azure-virtual-desktop

- **China endpoints for Microsoft Intune**
  Updated the Experimentation and Configuration Service (ECS) endpoint for Intune operated by 21Vianet to https://mooncake.ecs.office.com. This ensures customers allow the correct endpoint for service configuration and feature rollout.
  https://learn.microsoft.com/en-us/intune/fundamentals/endpoints-china

- **Manage endpoint security in Microsoft Intune**
  Replaced the Tamper protection benefit with Controlled configuration (preview), which enables Intune to enforce Defender security settings over other management channels. Added a reference to detailed documentation for configuration and behavior.
  https://learn.microsoft.com/en-us/intune/device-security/endpoint-security-policies

- **Internet access requirements**
  Clarified that when the management point uses a proxy, it must be configured in the Local System context for Microsoft Entra token validation in version 2603. Proxies set in site system properties or WinHTTP-only are not used; guidance links to proxy configuration steps.
  https://learn.microsoft.com/en-us/intune/configmgr/core/plan-design/network/internet-endpoints

- **Monitor results of your device compliance policies in Microsoft Intune**
  Added details on Windows devices that support client-driven compliance evaluation, which can proactively trigger re-evaluation based on local changes. Clarified how this affects reporting refresh frequency and the role of device check-in.
  https://learn.microsoft.com/en-us/intune/device-security/compliance/monitor-policy

- **Protect data and devices with Microsoft Intune**
  Expanded Defender for Endpoint integration to include Controlled configuration for Microsoft Defender settings (preview), which also supports tamper protection scenarios. Added coverage of client-driven compliance evaluation on Windows, enabling proactive compliance checks outside normal intervals.
  https://learn.microsoft.com/en-us/intune/device-security/overview

- **Proxy server support in Configuration Manager**
  Provided detailed steps for configuring the management point proxy for Microsoft Identity Service Essentials (MISE) in version 2603 using the Local System account’s WinINET settings. Included registry/Internet Options configuration via PsExec, required service restart, verification and troubleshooting steps, a PowerShell connectivity test, and noted future support for site system proxy.
  https://learn.microsoft.com/en-us/intune/configmgr/core/plan-design/network/proxy-server-support

- **Learn about using Intune to manage Microsoft Defender settings on devices that aren't enrolled with Intune**
  Added support for GCC High tenants. Reworked device protection guidance to introduce Controlled configuration, clarifying how Intune-delivered Defender settings take precedence over other management sources and how this relates to Tamper Protection.
  https://learn.microsoft.com/en-us/intune/device-security/microsoft-defender/security-settings-management

- **Service information for Microsoft Intune release updates**
  Added information about service configuration and controlled feature rollout (CFR) via the Experimentation and Configuration Service (ECS), including how payloads support service health and compliance. Noted that experiments are limited to CFR and cautioned that blocking required cloud communications can affect updates, reliability, security, and feature enablement.
  https://learn.microsoft.com/en-us/intune/fundamentals/servicing-information

- **Device Action: Sync**
  Added a Windows-focused description of on-demand sync, covering compliance evaluation, configuration processing, app state updates, and script/remediation processing. Introduced the Device sync status tab for progress tracking, noting it applies only to Windows devices.
  https://learn.microsoft.com/en-us/intune/device-management/actions/sync

- **What's new in version 2603 of Configuration Manager current branch**
  Clarified that the management point proxy must be set in the Local System context for token validation in version 2603. Site system proxy settings and WinHTTP-only proxies are not used; linked to detailed proxy configuration guidance.
  https://learn.microsoft.com/en-us/intune/configmgr/core/plan-design/changes/whats-new-in-version-2603