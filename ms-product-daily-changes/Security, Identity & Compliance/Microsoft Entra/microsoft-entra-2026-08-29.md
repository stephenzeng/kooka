# Microsoft Entra
**Date created:** 2026-08-29 UTC  
**Tags:** Configuration, Deprecation, Get Started, Governance, Guidance, Identity, Licensing, Monitoring, Performance, Security, Troubleshooting  

## New Articles

- **Microsoft Entra provisioning options (Preview)**

  Introduces deployment options for provisioning from Microsoft Entra ID to on-premises Active Directory using Cloud Sync, covering groups-only (GA), users-only (preview), and users-and-groups (preview). Explains when to choose each option, scoping approaches, and per-domain configuration limits (one per AD domain; up to 20 per tenant). Details performance and scale considerations, unsupported scenarios, and remediation steps when limits are exceeded, including methods to select more than 999 groups.

  https://learn.microsoft.com/en-us/entra/identity/hybrid/cloud-sync/concept-deployment-options-provision-to-active-directory

- **Microsoft Entra provisioning behavior (Preview)**

  Explains end-to-end provisioning behavior from Microsoft Entra ID to Active Directory, including scope evaluation, matching via msDS-ExternalDirectoryObjectId, attribute mapping, and write operations. Describes user and group scenarios, membership handling, and how the cloud remains the source of truth for updates. Clarifies delete behaviors, sync cadence, and key limitations such as no password writeback, helping admins anticipate operational outcomes.

  https://learn.microsoft.com/en-us/entra/identity/hybrid/cloud-sync/how-provisioning-to-active-directory-works

- **Microsoft Entra prerequisites for AD (Preview)**

  Outlines prerequisites and licensing for provisioning users and groups from Microsoft Entra ID to AD using Cloud Sync. Provides a consolidated prerequisites checklist and pointers to next steps for configuring scoping filters and attribute mappings so teams can plan deployments efficiently.

  https://learn.microsoft.com/en-us/entra/identity/hybrid/cloud-sync/how-to-prerequisites-provision-entra-to-active-directory

- **Preserve a group's organizational unit (Preview)**

  Describes how to keep a group’s original OU and CN in AD when converting its source of authority to Microsoft Entra ID. Guides you to create a GroupDN directory extension, map the group’s distinguishedName in Cloud Sync, verify the mapping, and then convert SOA. This preserves AD structure during cloud-driven management transitions.

  https://learn.microsoft.com/en-us/entra/identity/hybrid/cloud-sync/how-to-preserve-group-organizational-unit-entra-to-active-directory

- **Test Microsoft Entra provisioning (Preview)**

  Provides a step-by-step process to test and enable provisioning from Microsoft Entra ID to AD using on-demand provisioning for users and groups. Explains default protections (accidental deletes, notifications), initial and delta sync cycles, quarantine behavior, and how to restart or delete configurations. Helps ensure safe rollout and quicker validation before full enablement.

  https://learn.microsoft.com/en-us/entra/identity/hybrid/cloud-sync/how-to-test-and-enable-provisioning-entra-to-active-directory

- **Provision Microsoft Entra ID objects to AD**

  Offers a conceptual overview of provisioning users, security groups, and memberships from Microsoft Entra ID to AD via Cloud Sync. Clarifies preview/GA scope, matching and creation logic, OU behaviors, and unsupported scenarios (for example, mail-enabled and distribution groups, password writeback). Summarizes licensing based on configuration counts and links to next steps for deployment.

  https://learn.microsoft.com/en-us/entra/identity/hybrid/cloud-sync/overview-provision-entra-id-to-active-directory

- **Tutorial: Govern access to an on-premises app (Preview)**

  Presents an end-to-end tutorial to govern access to a Kerberos-based on-premises app by provisioning cloud-managed users and a security group to AD. Covers scoping choices, enabling membership write-back to on-premises users, target OU selection, and validation with on-demand provisioning. Explains authentication via Cloud Kerberos Trust, AD object enforcement, lifecycle management, and how to revert SOA when needed.

  https://learn.microsoft.com/en-us/entra/identity/hybrid/cloud-sync/tutorial-users-groups-provisioning-walkthrough

## Major Changes

- **Microsoft Entra AD object enforcement (Preview)**

  Renamed and expanded coverage from group-only enforcement to include both users and groups, with detailed prerequisites and rollout steps across writable domain controllers. Added SOA policy creation and management guidance, attribute mappings for marking users and groups, and verification and troubleshooting tools. Clarified behaviors for enforced and audit modes, break-glass setup, preview limitations, and operational requirements across DCs.

  https://learn.microsoft.com/en-us/entra/identity/hybrid/cloud-sync/how-to-active-directory-object-enforcement

- **Microsoft Entra provisioning setup (Preview)**

  Reworked setup guidance to support provisioning users and groups (not just groups) from Microsoft Entra ID to AD DS. Adds comprehensive scoping options, target container configuration with expression-based routing, and examples to preserve original OUs and CNs. Expands attribute mapping customization, verification, post-provisioning operations, and organizes navigation to testing and enablement content.

  https://learn.microsoft.com/en-us/entra/identity/hybrid/cloud-sync/how-to-configure-entra-to-active-directory

- **On-demand provisioning - Microsoft Entra ID to Active Directory**

  Substantially updated to cover testing both users and groups with clear UI steps and tabbed guidance. Introduces a results review model across import, scope, match, and action with status insights and retry options. Reinforces group testing limits and clarifies that members aren’t provisioned automatically, aligning expectations for targeted validation.

  https://learn.microsoft.com/en-us/entra/identity/hybrid/cloud-sync/how-to-on-demand-provision-entra-to-active-directory

- **Use directory extensions when provisioning to Active Directory**

  Expanded from group-only scenarios to cover both users and groups using directory extensions. Adds clear prerequisites, service principal checks, and supported identifier URI, plus end-to-end steps to create and set extension values via Graph tools. Provides corrected PowerShell syntax, security notes, and thorough testing and verification workflows to ensure reliable attribute flow.

  https://learn.microsoft.com/en-us/entra/identity/hybrid/cloud-sync/tutorial-directory-extension-group-provisioning

## Moderate Changes

- **Microsoft Entra Cloud Sync troubleshooting**

  Removed the section for repairing the Cloud Sync service account using AADCloudSyncTools, reflecting changes in supported remediation steps. This streamlines guidance and reduces reliance on deprecated tooling.

  https://learn.microsoft.com/en-us/entra/identity/hybrid/cloud-sync/how-to-troubleshoot

- **Microsoft Entra Cloud Sync supported topologies and scenarios**

  Clarifies write-back behavior so only members with AD accounts are included and narrows attribute requirements to on-premises synchronized users needing onPremisesObjectIdentifier matching objectGUID. Improves accuracy of topology guidance and image descriptions for planning deployments.

  https://learn.microsoft.com/en-us/entra/identity/hybrid/cloud-sync/plan-cloud-sync-topologies

- **Configure custom extensions for Privileged Identity Management role activation (Preview)**

  Updated token validation requirements by changing the calling application claim value that identifies PIM. Adjusted example authentication configuration with a new resourceId GUID to align with current validation patterns.

  https://learn.microsoft.com/en-us/entra/id-governance/privileged-identity-management/privileged-identity-management-custom-extensions

- **Microsoft Entra Cloud Sync error codes and descriptions**

  Removed two error codes related to Cloud Sync service account credentials (invalid and expired). This aligns the reference with current behavior and supported remediation paths.

  https://learn.microsoft.com/en-us/entra/identity/hybrid/cloud-sync/reference-error-codes

- **AADCloudSyncTools PowerShell module for Microsoft Entra Cloud Sync**

  Removed documentation for the Repair-AADCloudSyncToolsAccount cmdlet, reflecting deprecation of that repair approach. Other reference content remains unchanged.

  https://learn.microsoft.com/en-us/entra/identity/hybrid/cloud-sync/reference-powershell

- **Microsoft Entra private network connector: version release history**

  Added an advisory directing customers on versions 1.5.612.0 or earlier to update immediately and marked several versions as Deprecated. This strengthens guidance for staying current and secure.

  https://learn.microsoft.com/en-us/entra/global-secure-access/reference-version-history