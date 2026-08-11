# Microsoft Intune
**Date created:** 2026-08-01 UTC  
**Tags:** Administration, Automation, Governance, Monitoring, Security  

## New Articles

- **Clients fail to download content with HTTP 405 errors**

  Introduced a troubleshooting guide for Configuration Manager distribution points where clients encounter HTTP 405 responses during content downloads when WebDAV is enabled. Explains typical symptoms seen in DataTransferService.log and IIS logs with PROPFIND requests. Provides root cause analysis (WebDAV Publishing role enabled) and prescriptive steps to remove the role service and validate successful retries.

  https://learn.microsoft.com/en-us/troubleshoot/mem/configmgr/app-management/issues/clients-fail-download-content-http-405-errors

- **Database Replication Service activation internals**

  Added a deep-dive reference on DRS activation managed by RCM, including how handler targets are computed and maintained based on capacity, site roles, and MaxHandlers. Details queue enablement behavior, handler lifecycle, and how to interpret RCMCtrl.log and SQL read-only queries to assess queue activity and activation health. Outlines a supported recovery approach that prioritizes Replication Link Analyzer and infrastructure validation over manual manipulation.

  https://learn.microsoft.com/en-us/troubleshoot/mem/configmgr/data-transfer-sites/troubleshoot/drs-activation-internals

- **Database Replication Service reinitialization internals**

  Published a comprehensive walkthrough of the DRS reinitialization lifecycle, control messages, and package flow across export, transfer, validation, and completion. Includes status and progress markers, publisher-side request states, and diagnostic SQL queries for tracking requests and SSB transmission queues. Provides guidance on interpreting related logs and a supported recovery path emphasizing RLA usage and avoidance of unsupported actions.

  https://learn.microsoft.com/en-us/troubleshoot/mem/configmgr/data-transfer-sites/troubleshoot/drs-reinitialization-internals

- **Troubleshoot DRS Service Broker certificate and endpoint errors**

  Added a focused troubleshooting guide for SSB-related DRS failures, covering endpoint identities, certificate mappings, permissions, routes, and transmission queue issues. Offers read-only diagnostics using spDiagDRS/spDiagDRSCertInfo and targeted SQL queries to pinpoint common error states and directional failures. Recommends an evidence-driven recovery path that uses RLA and Microsoft Support for product-managed SSB object repair.

  https://learn.microsoft.com/en-us/troubleshoot/mem/configmgr/data-transfer-sites/troubleshoot/drs-ssb-certificate-errors

- **Database Replication Service synchronization internals**

  Introduced a detailed reference to the end-to-end DRS synchronization process, from scheduling and extraction through SSB message transmission and acknowledgment. Explains replication group types, throttling safeguards, dialog handling, and version validity checks. Provides diagnostic queries, log interpretation tips, and a decision framework to isolate failures before considering reinitialization.

  https://learn.microsoft.com/en-us/troubleshoot/mem/configmgr/data-transfer-sites/troubleshoot/drs-synchronization-internals

## Major Changes

- **What's new in Microsoft Intune**

  Added a new “Week of July 27, 2026 (Service release 2607)” section with broad feature updates across device configuration, enrollment, management, security, and app catalog regions. Highlights include Samsung Knox E‑FOTA for Android Enterprise, Windows registry data collection, fuller on-demand sync for Windows, custom compliance for macOS, preview Controlled Configuration for Defender AV, and regional discovery for Microsoft Store apps. Also expanded Windows settings catalog options (camera behavior, Keyboard Filter for Insider builds, WSL), refreshed Microsoft Edge policy coverage (Edge 148/149 and Copilot-related controls), new OneDrive policies, the ability to disable the Get Started app, a subsetting to remove default Store packages, and an updated Visual Studio ADMX with a policy to disable MCP.

  https://learn.microsoft.com/en-us/intune/whats-new/

- **In development - Microsoft Intune**

  Removed several previously listed in‑development items, including Samsung Knox E‑FOTA management, Windows Registry data collection, improved Windows on-demand sync, custom compliance for macOS, Controlled Configuration for Defender AV settings, and regional support for Microsoft Store apps. This cleanup reflects items that have shipped or changed status, helping readers focus on the remaining roadmap.

  https://learn.microsoft.com/en-us/intune/whats-new/in-development

- **Use Multi Admin Approval in Intune**

  Expanded guidance to cover enforcement for both delegated admin actions and app-authenticated Microsoft Graph API calls, with direction to update automation and a link to the dedicated Graph API article. Added support for excluding specific enterprise apps from MAA (up to 50 per policy) with details on scope, auditing, and security implications. Clarified approver prerequisites (required read permissions, direct RBAC role assignment, and nested group caveats) and updated the policy workflow to include app exclusions and a Review + submit step that captures business justification.

  https://learn.microsoft.com/en-us/intune/fundamentals/role-based-access-control/multi-admin-approval

- **Maintain the Windows Server Update Services (WSUS) database manually or automatically**

  Enhanced WSUS maintenance with new options to toggle MaxXMLPerRequest and delete test detectoids, backed by new PowerShell functions and SQL operations. Integrated these into the interactive menu and default run sequence, improved logging and flow, and noted operational requirements like performing an IISRESET after configuration changes. These additions streamline upkeep and reduce manual troubleshooting for performance and catalog hygiene.

  https://learn.microsoft.com/en-us/troubleshoot/mem/configmgr/update-management/wsus-automatic-maintenance

## Moderate Changes

- **Using Azure Virtual Desktop with Intune**

  Clarified prerequisites for Azure Virtual Desktop VMs by removing the region requirement and specifying that VMs must be deployed in an Azure subscription associated with the same Entra ID tenant as Intune. This reduces deployment friction and prevents misconfiguration tied to region constraints.

  https://learn.microsoft.com/en-us/intune/solutions/azure-virtual-desktop

- **What's new in previous months in the Microsoft Intune**

  Added two historical “What’s new” entries: support for using a PowerShell script as a Win32 app installer with return-code reporting, and ACME-based enrollment certificates for Apple platforms replacing SCEP for new enrollments. Also documented new ADE Setup Assistant screens that can be shown or hidden, with OS/version guidance and references.

  https://learn.microsoft.com/en-us/intune/whats-new/archive

- **Troubleshoot Database Replication Service**

  Expanded the overview to emphasize DRS and SQL Server–related issues and added cross-references to new internals and certificate/endpoint troubleshooting articles. Replaced older blog links with a consolidated, symptom-based guide and refined the overview diagram’s alt text for clarity.

  https://learn.microsoft.com/en-us/troubleshoot/mem/configmgr/data-transfer-sites/troubleshoot/overview

- **Prerequisites for the Microsoft Tunnel in Intune**

  Updated supported Linux distributions by removing Ubuntu 22.04 and adding Ubuntu 26.04 (Docker CE). This ensures prerequisites align with current platform support for Tunnel deployments.

  https://learn.microsoft.com/en-us/intune/device-security/microsoft-tunnel/prerequisites

- **Troubleshoot the SQL Server instance configuration**

  Reframed the article as a troubleshooting guide for SQL Server Service Broker issues that impact DRS, adding a clear process overview and scoping statements. Updated headings, remediation guidance, and cross-references for diagnostics covering endpoints, certificates, permissions, routes, and transmissions, plus instructions for tracing SSB events with SQL Server Profiler.

  https://learn.microsoft.com/en-us/troubleshoot/mem/configmgr/data-transfer-sites/troubleshoot/sql-configuration

- **Troubleshoot DRS reinitialization**

  Added a summary and a guided troubleshooting process aligned to a decision-tree diagram, clarifying how to identify incomplete reinitialization across replication groups. Introduced a Next steps link to reinitialization internals and refined headings and alt text for better readability.

  https://learn.microsoft.com/en-us/troubleshoot/mem/configmgr/data-transfer-sites/troubleshoot/sql-replication-reinit

- **Upgrade Microsoft Tunnel for Microsoft Intune**

  Added release notes for version 20260624.1 dated July 27, 2026, including agent and server image SHA‑256 digests. Notes minor bug fixes to inform upgrade planning and validation.

  https://learn.microsoft.com/en-us/intune/device-security/microsoft-tunnel/upgrade