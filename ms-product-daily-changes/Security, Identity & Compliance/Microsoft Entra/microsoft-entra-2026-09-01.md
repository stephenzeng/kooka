# Microsoft Entra
**Date created:** 2026-09-01 UTC  
**Tags:** Compliance, Configuration, Guidance, Governance, Identity, Security  

## New Articles

- **How to configure custom HTTP headers in Global Secure Access**

  Introduced a how-to guide for injecting custom HTTP headers into outbound web traffic using Web Content Filtering v2 policies (preview). The article outlines prerequisites such as onboarding to Microsoft Entra Internet Access, enabling TLS inspection with trusted roots, and configuring client/proxy routing and destination identifiers. It provides step-by-step procedures to set up TLS inspection, create a Web Filtering v2 policy, add rules with destination matching and header name/value pairs, and link the policy to a security profile enforced via Conditional Access. It includes example header requirements for common services (e.g., GitHub, Google Workspace, Slack) and notes propagation timelines, while recommending universal tenant restrictions for Microsoft Entra tenants over custom headers.

  https://learn.microsoft.com/en-us/entra/global-secure-access/how-to-configure-custom-headers

- **Tutorial - Provision groups to Active Directory Domain Services (AD DS) by using Microsoft Entra Cloud Sync**

  Added a comprehensive tutorial for provisioning groups from Microsoft Entra to on-premises AD DS with Cloud Sync. It covers prerequisites, recommended scoping, and detailed source-of-authority scenarios, with step-by-step configuration and multiple methods to map target OUs (constant, custom expressions, scripts, and displayName-based routing). The guide shows how to validate changes with on-demand provisioning, explains behavior and logging for SOA-converted groups and nested memberships, and describes rollback behavior. It also introduces AD group enforcement (preview) to ensure only Cloud Sync can modify or delete synced groups, with links to related setup and governance guidance.

  https://learn.microsoft.com/en-us/entra/identity/hybrid/cloud-sync/tutorial-group-provisioning

## Major Changes

- **Configure AD group enforcement in Microsoft Entra Cloud Sync (preview)**

  The article now focuses solely on enforcing groups, with an updated overview of enforcement behavior and modes based on LDAP write interception and the msDS-ObjectSoa attribute. Prerequisites and rollout steps were clarified, including supported DC OS versions, required ntdsai.dll versions, and deployment via Known Issue Rollback Group Policy packages, plus the need to run Set-CloudSyncSOAPolicy.ps1 on the agent host. Configuration was simplified to marking groups for enforcement through attribute mappings, with a verification process using ADSI Edit and refreshed troubleshooting. Known limitations specify that only groups are supported in this preview and deletions aren’t prevented.

  https://learn.microsoft.com/en-us/entra/identity/hybrid/cloud-sync/how-to-ad-group-enforcement

- **Configure - Provisioning Microsoft Entra ID to Active Directory using Microsoft Entra Cloud Sync for Groups**

  The content was streamlined to focus on provisioning groups from Microsoft Entra ID to AD, with clearer configuration steps and scoping guidance. It summarizes attribute mapping considerations with references, on-demand provisioning for validation, and safeguards such as accidental deletion protection, quarantines, and restart procedures. Legacy user-focused scenarios and deep-dive mapping examples were removed to reduce complexity and improve discoverability.

  https://learn.microsoft.com/en-us/entra/identity/hybrid/cloud-sync/how-to-configure-entra-to-active-directory

- **Scenario - Using directory extensions with group provisioning to Active Directory**

  The tutorial was refocused to a group-only scenario demonstrating how a custom directory extension (for example, WritebackEnabled) can control which groups are written back to AD. It adds prescriptive steps to create the necessary Graph application and service principal, define a Group extension property, configure Cloud Sync scoping using the extension, and set the extension value on the selected group. The flow concludes with on-demand provisioning to validate that only the intended group is provisioned, while removing user-specific extension mapping content.

  https://learn.microsoft.com/en-us/entra/identity/hybrid/cloud-sync/tutorial-directory-extension-group-provisioning

## Moderate Changes

- **Access packages for Agent identities**

  Added guidance for requesting an access package on behalf of another user, including steps in the My Access portal and the US Government domain nuance (myaccess.microsoft.us). The update clarifies selection options, user search, and completion, supported by a new screenshot.

  https://learn.microsoft.com/en-us/entra/agent-id/agent-access-packages

- **Microsoft Entra Cloud Sync directory extensions for provisioning to Active Directory**

  Retitled and refocused to emphasize Cloud Sync usage for directory extensions, with a clearer introduction and updated references. The update clarifies support limitations (application identifier URI and Tenant Schema Extension App), refreshes the tutorial link to a group scenario, and streamlines methods while retaining PowerShell and Graph guidance.

  https://learn.microsoft.com/en-us/entra/identity/hybrid/cloud-sync/custom-attribute-mapping-entra-to-active-directory

- **On-demand provisioning - Active Directory to Microsoft Entra ID**

  The introduction was rewritten to clarify that the article covers Microsoft Entra Cloud Sync and focuses on provisioning from Microsoft Entra ID to Active Directory. This corrects prior orientation and aligns readers with the intended direction.

  https://learn.microsoft.com/en-us/entra/identity/hybrid/cloud-sync/how-to-on-demand-provision

- **On-demand provisioning - Microsoft Entra ID to Active Directory**

  The procedure was consolidated into a group-based workflow, allowing selection of a group and up to five members for validation without automatic provisioning. User-based instructions and tabs were removed, screenshots were updated, and references were streamlined into a Next steps section.

  https://learn.microsoft.com/en-us/entra/identity/hybrid/cloud-sync/how-to-on-demand-provision-entra-to-active-directory

- **Microsoft Entra Cloud Sync supported topologies and scenarios**

  Updated guidance for multi-forest group provisioning clarifies that AD-written groups can include only on-premises synchronized users and/or cloud-created security groups. It also specifies that all such users must have the onPremisesObjectIdentifier attribute set.

  https://learn.microsoft.com/en-us/entra/identity/hybrid/cloud-sync/plan-cloud-sync-topologies