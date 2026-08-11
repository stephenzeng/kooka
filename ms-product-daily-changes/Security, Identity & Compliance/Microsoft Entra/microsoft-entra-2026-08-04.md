# Microsoft Entra
**Date created:** 2026-08-04 UTC  
**Tags:** Administration, Automation, Governance, Security  

## New Articles

- **How to connect a remote network when your CPE is behind NAT - Microsoft Entra Global Secure Access**

  Introduced a how-to guide for configuring Global Secure Access remote networks when the customer premises equipment (CPE) is behind an upstream NAT using IKEv2 NAT Traversal. Explains the required topology and the key requirement to use the upstream router’s public IP for the device link while retaining the CPE’s BGP address and ASN. Provides prerequisites, NAT-T concepts (detection, UDP 4500 encapsulation, keepalives), and a step-by-step configuration checklist across VPN, BGP, firewall, and MTU/MSS settings. Includes troubleshooting guidance for IKE negotiation, idle session drops, BGP stability, packet/MTU issues, and public IP changes.

  https://learn.microsoft.com/en-us/entra/global-secure-access/how-to-create-remote-network-cpe-behind-nat

- **Configure Zscaler Provisioning for automatic user provisioning with Microsoft Entra ID**

  Added a step-by-step tutorial to set up automatic user and group provisioning to Zscaler via SCIM. Covers capabilities, prerequisites, and deployment planning; details Zscaler-side setup with OAuth2 client credentials; and walks through adding the app from the gallery, configuring provisioning scope, defining the tenant URL and secret, testing the connection, and starting provisioning. Provides guidance on attribute mappings, accidental deletion protection, scoping filters, monitoring, and includes references plus an optional PowerShell script for role assignments.

  https://learn.microsoft.com/en-us/entra/identity/saas-apps/zscaler-zidentity-provisioning-tutorial

## Major Changes

- **Reference for extending Microsoft Entra attribute mappings with custom call-outs using LCW extensibility workflows (preview)**

  Expanded the reference with end-to-end procedures for creating custom extensions and Lifecycle Workflows using both the Microsoft Entra admin center and Microsoft Graph. Added detailed Graph examples and required permissions for creating customTaskExtensions and Lifecycle Workflows, and for updating the synchronization schema. Clarifies how to map an extensibility workflow to target attributes (for example, userPrincipalName) with required fields and full request/response samples to accelerate implementation.

  https://learn.microsoft.com/en-us/entra/identity/app-provisioning/extend-application-attributes

## Moderate Changes

- **Passkeys by default and retirement of Microsoft-provided SMS and voice authentication**

  Reorganized content by moving the inline FAQ to a dedicated FAQ article and surfaced guidance on temporarily opting out of automatic passkey enablement, including how to set passkeyDynamicMigration via Microsoft Graph. Clarified enforcement timing and conditions for February 1, 2027, and emphasized that enforcement has no opt-out, helping administrators plan their transition.

  https://learn.microsoft.com/en-us/entra/identity/authentication/concept-sms-voice-retirement