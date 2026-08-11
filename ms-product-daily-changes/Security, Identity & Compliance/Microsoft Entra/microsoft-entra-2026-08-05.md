# Microsoft Entra
**Date created:** 2026-08-05 UTC  
**Tags:** Administration, AI, Agent, Governance, Monitoring, Security  

## New Articles

- **Choose a telephony provider for SMS and voice authentication**

  Introduced a new conceptual guide to customer-managed telephony providers for SMS and voice authentication in Microsoft Entra ID, covering how providers integrate and what organizations must manage. Outlined timelines for availability (provider information on Sep 18, 2026 and configuration on Oct 30, 2026) and recommended prioritizing phishing-resistant methods such as passkeys. Provided planning guidance to assess user needs, validate phishing-resistant alternatives, evaluate providers (coverage, channels, pricing, support, security, compliance), meet procurement/privacy/regulatory requirements, run a pilot, and prepare fallback methods. References related retirement plans, FAQs, and passkey deployment resources to support transition planning.

  https://learn.microsoft.com/en-us/entra/identity/authentication/concept-phone-providers

## Major Changes

- **Configure an automatic assignment policy for an access package in entitlement management**

  Added an important notice that the preview memberOf rule operator is ending and that automatic assignment policies using memberOf will be quarantined starting October 27, 2026. Included a Microsoft Graph PowerShell script and steps to find impacted automatic assignment policies and export results to CSV. Provided remediation guidance to rebuild rules using supported attribute-based operators or choose alternative assignment methods, and advised validating assignments after updates to avoid access disruption.

  https://learn.microsoft.com/en-us/entra/id-governance/entitlement-management-access-package-auto-assignment-policy

- **How to analyze the Microsoft Entra provisioning logs**

  Expanded guidance to include analyzing provisioning logs with Microsoft Graph and added a new section on Microsoft MCP Server for Enterprise (Preview). Clarified prerequisites, roles, and delegated permission (MCP.ProvisioningLog.Read.All) for MCP’s read-only access, and provided example natural-language prompts with the corresponding Graph API requests. Documented best practices and known limitations, and updated the overview to include MCP-based natural-language analysis options.

  https://learn.microsoft.com/en-us/entra/identity/monitoring-health/howto-analyze-provisioning-logs

## Moderate Changes

- **Create content policies for network content filtering**

  Added an optional Source type condition (preview) to scope content policy rules by traffic origin. You can select Agent to target AI agent–classified traffic, while non-agent traffic is treated as User; if not configured, rules apply to all traffic.

  https://learn.microsoft.com/en-us/entra/global-secure-access/how-to-network-content-filtering