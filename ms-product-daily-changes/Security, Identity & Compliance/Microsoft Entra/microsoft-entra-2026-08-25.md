# Microsoft Entra
**Date created:** 2026-08-25 UTC  
**Tags:** Configuration, Guidance, Governance, Identity, Monitoring, Security  

## New Articles

- **SAM Account Name**

  Introduced public preview support to synchronize the Security Account Manager account name (sAMAccountName) in Microsoft Entra Domain Services. Explains prerequisites, when to enable the feature, and how synchronization sources onPremisesSamAccountName. Highlights benefits such as improved compatibility, reduced identity drift, and simpler migrations with fewer authentication issues. Provides step-by-step instructions to enable the setting in the Entra admin center and validate outcomes for hybrid and cloud-only users.

  https://learn.microsoft.com/en-us/entra/identity/domain-services/security-account-name

## Major Changes

- **Lifecycle workflows execution conditions and scheduling**

  Introduced preview support for relative time-based comparisons with a Time based attribute V2 (Preview) option, adding operators (Exactly, Between, Less than or equal to) and expanded day offsets (0–365) including Days to event for Between. Clarified event timing behavior (Before/After and Exactly 0 days for On), listed supported event attributes, and noted that V2 preview does not include the three-day catch-up window. Documented that workflows created during preview will move to a unified experience at GA and removed LastSignInDateTime as a valid user attribute for leaver workflows.

  https://learn.microsoft.com/en-us/entra/id-governance/lifecycle-workflow-execution-conditions

## Moderate Changes

- **Request access package on-behalf-of other identities**

  Added guidance for enabling designated users (for example, project leads or help desk) to request access packages on behalf of others. Clarifies how to select the target user, choose the package, provide request details, and that all requests still follow existing approvals and lifecycle policies to maintain oversight.

  https://learn.microsoft.com/en-us/entra/id-governance/entitlement-management-request-behalf

- **Install the Global Secure Access Client for macOS**

  Added an important note that version 1.1.26060207 includes com.microsoft.autoupdate2, which can conflict with Intune detection rules if already present. Updated deployment guidance to optionally exclude com.microsoft.autoupdate2 in detection rules to prevent conflicts.

  https://learn.microsoft.com/en-us/entra/global-secure-access/how-to-install-macos-client

- **Microsoft Entra Connect Health: Version Release History**

  Added the August 2026 release entry for agent version 4.5.2614.0. Highlights stronger credential security with key rotation, improved cloud compatibility and telemetry resilience, and reliability and quality improvements across installation and registration.

  https://learn.microsoft.com/en-us/entra/identity/hybrid/connect/reference-connect-health-version-history

- **Global Secure Access Client for macOS Release Notes**

  Documented version 1.1.26060207, adding Home Network traffic controls, a new Connections page, and agentic detection support for policy enforcement. Noted improved connectivity checks, Secure DNS bypass support, multiple fixes (MSAL sign-in, cache reset policy clearing, restarts, macOS 27 beta partial connections, tunnel establishment after wake), and inclusion of com.microsoft.autoupdate2 with optional Intune detection adjustments.

  https://learn.microsoft.com/en-us/entra/global-secure-access/reference-macos-client-release-history

- **Understanding lifecycle workflows**

  Announced that relative time-based comparisons for time-based triggers are in public preview and that the admin center shows both “Time based attribute” and “Time based attribute V2 (Preview)” representing the same capability, which will consolidate at GA. Clarified trigger descriptions to cover point-in-time and relative comparisons and explained that the standard trigger’s three-day catch-up does not apply to V2 during preview.

  https://learn.microsoft.com/en-us/entra/id-governance/understanding-lifecycle-workflows