# Microsoft Entra
**Date created:** 2026-09-04 UTC  
**Tags:** Best Practices, Configuration, Get Started, Governance, Guidance, Identity, Monitoring, Security, Troubleshooting  

## New Articles

- **Microsoft Entra ID Entitlement Management integration with ServiceNow**

  Introduced a new tutorial detailing how to integrate Microsoft Entra ID Entitlement Management with ServiceNow, including roles of each system and required licensing (Entra ID P2 or Entra Suite). Provides installation via the ServiceNow Store with a link to the installation guide and explains end-user capabilities such as requesting access packages, viewing request history, and approving/denying requests in ServiceNow. Includes step-by-step walkthroughs for key actions and clarifies that Microsoft Entra remains the system of record. Screenshots illustrate the experience to help accelerate deployment and adoption.

  https://learn.microsoft.com/en-us/entra/id-governance/entitlement-management-servicenow-integration

- **Secure a Model Context Protocol (MCP) server with Microsoft Entra ID**

  Added comprehensive guidance for securing an MCP server as an OAuth 2.0 protected resource using Microsoft Entra ID. Covers app registration steps (enable v2 access tokens, set HTTPS Application ID URI, define scopes and optional app roles), publishing protected resource metadata and issuing WWW-Authenticate challenges, and validating tokens with recommended libraries and claims checks. Explains optional offload using Azure App Service Authentication and connecting MCP clients via Microsoft Entra Agent ID with appropriate identities, scopes, and roles. Includes FAQs and troubleshooting for token versions, resource/scope mismatches, and legacy configurations to reduce integration issues.

  https://learn.microsoft.com/en-us/entra/agent-id/secure-mcp-server-with-entra-id

## Major Changes

- **View audit log report for Microsoft Entra roles in Microsoft Entra PIM**

  Expanded guidance clarifies that PIM Resource audit logs are a subset of Microsoft Entra audit logs and recommends using Diagnostic Settings to route logs to Storage or Log Analytics. Introduces new correlation guidance that favors roleAssignmentRequestId over CorrelationId to link activation and deactivation events across the full lifecycle. Adds multiple Kusto query examples to retrieve activations, correlate related events, and analyze end-to-end activation/deactivation cycles, improving investigations and monitoring.

  https://learn.microsoft.com/en-us/entra/id-governance/privileged-identity-management/pim-how-to-use-audit-log

## Moderate Changes

- **Administrative relationships in Microsoft Entra Agent ID (Owners, sponsors, and managers)**

  Updated sponsor permissions to remove the ability to enable agent identities. Clarified that sponsors cannot re-enable or restore blueprints or identities and must work with a resource owner or admin to recover disabled or deleted resources, strengthening governance boundaries.

  https://learn.microsoft.com/en-us/entra/agent-id/agent-owners-sponsors-managers

- **Least privileged roles by task**

  Added a new task for performing identity containment actions during SOC incident response, mapped to the Entra SOC Identity Responder role. Updated guidance so Security Administrator is now also permitted to invalidate refresh tokens of non-admins alongside User Administrator, improving incident response options.

  https://learn.microsoft.com/en-us/entra/identity/role-based-access-control/delegate-by-task

- **Request access package on-behalf-of other identities**

  Revised configuration steps to select eligible requestors under “Who can request access” (for example, Manager or Users in your directory) instead of enabling new requests and toggling manager permissions. Clarifies how managers and designated users can request on behalf of others while preserving policy-driven approvals and lifecycle controls.

  https://learn.microsoft.com/en-us/entra/id-governance/entitlement-management-request-behalf

- **Microsoft Entra built-in roles**

  Added the new Entra SOC Identity Responder built-in role with description, privileges, and dedicated details via an include file. The roles table now reflects this role and its privileged designation, enabling clearer assignment and least-privilege planning.

  https://learn.microsoft.com/en-us/entra/identity/role-based-access-control/permissions-reference

- **Privileged roles and permissions in Microsoft Entra ID (preview)**

  Clarified that Security Administrator, along with Security Operator and Entra SOC Identity Responder, is limited to actions on non-administrative user accounts and cannot act on privileged accounts. This restriction is now reflected in two sections to reduce misconfiguration risk.

  https://learn.microsoft.com/en-us/entra/identity/role-based-access-control/privileged-roles-permissions

- **Publish your app to Microsoft Entra App Gallery**

  Updated prerequisites to require a Partner One ID (formerly MPN ID). Added a publishing workflow with states and business-day timelines, including examples, and guidance to complete metadata, testing, and validation to avoid delays.

  https://learn.microsoft.com/en-us/entra/identity/enterprise-apps/publish-app-gallery

- **What's new in Microsoft Entra RBAC documentation**

  Updated the June 2026 entry to include the new Entra SOC Identity Responder role and note updates to the Security Operator and AI Administrator roles. Helps readers quickly track RBAC capability and guidance changes.

  https://learn.microsoft.com/en-us/entra/identity/role-based-access-control/whats-new