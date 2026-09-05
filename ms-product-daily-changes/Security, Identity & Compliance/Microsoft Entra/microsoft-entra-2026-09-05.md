# Microsoft Entra
**Date created:** 2026-09-05 UTC  
**Tags:** Best Practices, Configuration, Governance, Guidance, Identity, Security, Troubleshooting  

## New Articles

- **Configure HiBob to Active Directory hybrid user provisioning**

  Introduced a step-by-step tutorial to set up HiBob (Bob) to provision and update users in on-premises Active Directory using Microsoft Entra API-driven provisioning and the provisioning agent. Covers prerequisites, architecture and flow, tenant connection and permissions, AD domain/OU selection, scope and attribute mappings (including Lifecycle Workflows), and synchronization and approval rules. Includes guidance for testing, monitoring runs and logs, and troubleshooting common issues such as connectivity, authorization, attribute mapping visibility, and pending approvals. This helps HR-driven, hybrid identity environments automate user lifecycle with clearer setup and operational guidance.

  https://learn.microsoft.com/en-us/entra/identity/saas-apps/hibob-to-active-directory-user-provisioning-tutorial

## Major Changes

- **Run a Registration Campaign to Set Up a Passkey or Microsoft Authenticator**

  Overhauled guidance to clarify campaign scope, eligibility, and configuration, separating Authenticator and Passkey campaigns with detailed prerequisites. Introduced clear definitions and behaviors for Microsoft managed vs Enabled states, including snooze configuration, persistence, and how to effectively require setup. Expanded user experience flows with new screenshots and added a platform-based passkey nudge matrix to set expectations across OS and browsers. Updated admin center steps and Graph Explorer examples, and reorganized FAQs to address eligibility nuances, mobile/SSO behavior, Conditional Access interactions, and rollout considerations, enabling better planning and compliance outcomes.

  https://learn.microsoft.com/en-us/entra/identity/authentication/how-to-mfa-registration-campaign

## Moderate Changes

- **Microsoft Entra ID Governance integrations**

  Added HiBob to the HR integrations list for Microsoft Entra ID/Active Directory provisioning, including a link to its tutorial. This improves discoverability and accelerates setup for organizations adopting HiBob for HR-driven provisioning.

  https://learn.microsoft.com/en-us/entra/id-governance/apps

- **Configure assignment restriction for user-assigned managed identities (preview)**

  Clarified that Azure CLI and IaC templates must specify provider namespaces without the /* suffix (for example, use Microsoft.Storage), since the suffix is only a portal display convention. Added guidance on restricting to a single resource type (for example, Microsoft.Storage/storageAccounts) and updated CLI examples to ensure precise and error-free enforcement.

  https://learn.microsoft.com/en-us/entra/identity/managed-identities-azure-resources/configure-managed-identities-assignment-restriction

- **Assignment restriction for user-assigned managed identities (preview)**

  Added a warning to use only the resource provider namespace (for example, Microsoft.Storage) in CLI and IaC templates and explained how to target a specific resource type (for example, Microsoft.Storage/storageAccounts). This helps avoid deployment errors and ensures granular identity assignment controls.

  https://learn.microsoft.com/en-us/entra/identity/managed-identities-azure-resources/managed-identities-assignment-restriction